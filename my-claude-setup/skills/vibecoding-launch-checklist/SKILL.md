---
name: vibecoding-launch-checklist
description: Checklist de seguridad, pagos, migraciones, CI/CD, legal y pulido de UX antes de lanzar o revisar una app construida mayormente con un agente de IA ("vibecoded"). Use when el usuario pide revisar si una app está lista para producción, pide un "security review" o "pre-launch checklist" de algo hecho con IA, va a lanzar/publicar un sitio o app, o pide "pulir"/arreglar detalles de algo armado rápido con un agente de código.
---

# Vibecoding launch checklist

Checklist acumulado de varios reels guardados sobre errores típicos de apps hechas rápido con agentes de IA. Repasar cada sección aplicable antes de dar el visto bueno a un lanzamiento.

## 1. Secretos y auth
- Ningún secreto/API key hardcodeado en el repo; todo en variables de entorno, nunca committeado. Ninguna key queda en código que corre en el browser (cualquiera puede verla con F12) — ni siquiera en el `.env` si ese archivo termina siendo servido por el sitio en producción.
- Auth real server-side, no solo validación en el cliente (los checks de permisos en frontend son decorativos, no seguridad).
- IDOR: que cambiar un ID en la URL o en un request (ej. el número de una factura/orden) nunca devuelva el recurso de otro usuario — validar siempre que el recurso pedido pertenece al usuario autenticado.
- 2FA o verificación de email en flujos sensibles; política de contraseñas mínima razonable.
- Rate limiting en login, reset de password y cualquier endpoint que llame a un modelo de IA (evita abuso y facturas inesperadas).
- Los links de reseteo de contraseña deben expirar.
- Sessions vs JWT: si se usa JWT, que sea de vida corta (~5 min) + refresh token guardado en base de datos — así sí es revocable (un JWT normal no se puede invalidar hasta que expira; ejemplo típico: usuario baneado que sigue operando con un JWT viejo).
- Panel de admin: que esté protegido con autenticación real, no solo "escondido" en una ruta no linkeada (seguridad por oscuridad no es seguridad).
- Tope de gasto (spend cap) + alertas en cualquier servicio de IA/cloud con costo variable. Si el agente de IA va a correr tests de integración, apuntarlo a un emulador local (tipo LocalStack para AWS: S3, DynamoDB, Lambda, SQS y 100+ servicios corriendo en `localhost`) en vez de a la cuenta real — evita que una corrida repetida de tests genere una factura real.

## 2. Inputs e infraestructura
- Sanitización de inputs contra XSS, SQL injection, CSRF.
- CORS configurado explícitamente (no "allow all" en producción).
- HTTPS forzado, headers de seguridad estándar, cookies con flags seguros (`httpOnly`, `secure`, `sameSite`).

## 2b. Si el backend es Supabase
- Row Level Security (RLS) activado en todas las tablas — si está apagado, cualquiera con la `anon key` puede leer cualquier tabla entera.
- Policies explícitas por tabla para que cada usuario solo acceda a sus propios datos.
- La `anon key` puede estar en el frontend sin problema (es pública por diseño) siempre que RLS y las policies estén bien puestas; la `service key` (la de admin, que ignora RLS) NUNCA debe estar en el frontend, en el repo ni en ningún lugar público — filtrarla anula toda la seguridad de RLS/policies de un saque.

## 3. Pagos
- Idempotencia en checkout: una "idempotency key" única por intento de compra, validada en el backend propio y pasada también al proveedor de pagos (ej. Stripe), para que un doble-click o reintento no cobre dos veces.
- Si se detecta un cobro duplicado, reembolso automático.

## 4. Base de datos
- Nunca dejar que el agente de IA corra migraciones directo en producción sin red de seguridad.
- Migraciones versionadas y testeadas primero en staging.
- Backups con restore probado (un backup que nunca se restauró no cuenta).
- Rollback / down migrations definidos para cada cambio de esquema.

## 5. CI/CD
- Tests, lint y build automáticos en cada push (CI).
- Despliegue vía artefacto empaquetado, no copiar archivos a mano.
- Paso por staging antes de producción; idealmente rollout gradual (canary) y rollback automático si falla.

## 6. Legal / compliance (pedirle esto a la IA antes de publicar)
Checklist de 20 puntos para que la IA lo verifique antes de lanzar (no es asesoría legal — qué aplica depende de dónde estén vos y tus usuarios): política de privacidad, términos de servicio, política de reembolso, política de cookies, banner de consentimiento de cookies, revisar los consentimientos de los formularios, no recolectar datos innecesarios, auditar SDKs de terceros, eliminar dark patterns, eliminar costos ocultos, eliminar reviews falsas, eliminar afirmaciones no respaldadas, texto alternativo de accesibilidad, ratio de contraste de color, navegación por teclado, datos de contacto del negocio visibles, consentimiento de edad si se recolectan datos de menores, link de "darse de baja" en emails, licencias de fuentes/imágenes en orden, opción de solicitud de borrado de datos.

## 7. Señales de "AI slop" a corregir (pulido de UX)
- Copy genérico que "suena a IA" sin voz propia, buzzwords vacíos, el patrón "no es X, es Y", em dash por todos lados.
- Paleta de colores morado/azul por defecto, gradientes en títulos, glassmorphism puesto en todo, orbes de fondo brillantes, bento grids vacíos, sparkle icons repetidos, badges arriba de cada título, cursor con estela.
- Favicon ausente o el placeholder por defecto — pedirle a la IA uno personalizado.
- Estados de carga mal manejados (nada, o un spinner genérico) — usar skeleton loaders.
- Tres feature cards en fila, pricing de tres niveles genérico, testimonios falsos, UI de chat sin personalizar, demos del producto ausentes (afirmaciones sin prueba real).
- Formularios que piden de más o no son accesibles por teclado; embeds de terceros rotos; información de negocio con datos placeholder.
- Checklist de 20 mejoras de producto: accesibilidad, estados de formularios (error/loading/success), navegación clara, performance percibida, detalles de UI que faltan en todo MVP recién salido de un agente.

## 8. Mega-prompt de seguridad para pedirle a la IA (punto de partida, no sustituto de este checklist)
"No quiero que mi sitio vibe-coded sea hackeado: escondé mis API keys, revisá mis variables de entorno, protegé mis rutas de admin, agregá autenticación correcta con acceso solo a lo que corresponde a cada usuario, sanitizá mis formularios, protegé contra XSS, asegurá mis endpoints de API, agregá rate limiting, revisá mis configuraciones core, apagá el modo debug, agregá security headers, actualizá mis dependencias, revisá archivos expuestos, asegurá mi base de datos, hasheá las contraseñas correctamente, revisá mi historial de Git por secretos filtrados, y corré una auditoría de seguridad completa." No confiar ciegamente en que el agente hizo todo bien solo porque dijo que lo hizo — pedir evidencia concreta de cada punto (o verificarlo manualmente) en vez de asumirlo.

## 9. Antes de instalar una skill/tool de terceros (supply chain)
No instalar a ciegas una skill o MCP solo porque la recomendaron en un reel o post: puede traer código malicioso que se ejecuta con los mismos permisos que el agente. Escanearla primero con una herramienta de seguridad dedicada (ej. Skill Spectre de NVIDIA) antes de dejar que toque el proyecto, e idealmente automatizarlo como un paso que corre solo ante cualquier descarga de skill/herramienta nueva, frenando y pidiendo confirmación si encuentra algo grave.

## Cómo usarlo
Repasar las secciones aplicables al proyecto y, para cada punto que falte, pedírselo directamente al agente de código en lenguaje natural (ej. "agregá rate limiting al login y un tope de gasto de $100/mes a los endpoints que llaman al modelo") — son todos cambios "vibecodeables", no requieren un plugin especial.

Fuente: análisis de reels guardados en `~/Downloads/reels-analysis/DOCUMENTO.md` (posts #13, #15, #22, #24, #25, #30, #31, #32, #37, #45, #46, #51, #59, #75, #86, #102, #108, #109, #119, #126 del documento).

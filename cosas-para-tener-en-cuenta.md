# Cosas para tener en cuenta — reels guardados

Lo que no se convirtió en skill (porque es conocimiento suelto, estrategia, o promocional) pero vale la pena no perder. Ver `DOCUMENTO.md` en esta misma carpeta para el análisis completo de los 113 reels (52 originales + 61 de la Tanda 4, agregados 2026-11-09; 2 posts de esa tanda no se pudieron descargar — `DcSf_TWyrtO` y `DdOamnsSBAM`, borrados o privados).

## Reglas de cómo debería escribir código un agente de IA
(Ya anotado como regla directa en `~/.claude/CLAUDE.md` — la dejo acá también de referencia.)
Errores típicos de "vibe coding" a evitar: sobre-generar código de más, asumir intenciones sin preguntar, borrar código que no se entiende, "arreglar" bugs sin verificación real.

## Workflow de Claude como editor/diseñador de video o marca
- Dar a la IA: proyectos de referencia open source, música propia con indicaciones de sync a los beats, un "archivo de marca" (colores/tipografía/estilo de movimiento), y una librería de ejemplos con sus prompts.
- Flujo completo: carpetas + "signature style" → rough cut automático → dirección creativa/storyboard → apertura → edición final → guardar feedback/aprendizajes para la próxima iteración.
- Para co-diseñar identidad de marca con Claude Artifacts: generar opciones → iterar con feedback puntual → fijar preferencias finales como reglas persistentes para que las próximas generaciones ya respeten ese estilo.
- Describir "glassmorphism" bien para que la IA genere un shader fiel: un vidrio real refracta, capta luz y refleja — no es solo un filtro translúcido/blur.

## Glosario mínimo de IA/LLMs (para "saber de qué se habla")
tokens, context window, temperature, hallucination, system prompt, RAG, embeddings, vector databases, fine-tuning, tool calling, MCP, agents/subagents, prompt caching, context engineering.

## Estrategia / negocio
- En la era del vibecoding, el código ya no es la ventaja competitiva (se clona fácil) — el moat real es: efecto de red, costos de cambio, datos propios, o confianza/reputación.
- Ser "experto en IA" es ventaja competitiva de contratación en cualquier oficio (cita de Jensen Huang, reel con video editado con ayuda de Claude).

## Catálogo de alternativas open-source a SaaS pagos
Ya resuelto en `~/Downloads/open-source-alternatives/RESUMEN.md` — 7 repos clonados (Cal.com, Chatwoot, Cap, OpenProject, OpenWhispr, WeKnora, OpenHiggsfield), 2 salteados (VoiceStudio, OpenSEO).

## Cosas mencionadas pero sin contenido verificable (carruseles de imágenes no legibles, o gateadas por DM)
- Lista de "111 skills/herramientas" para pegar en Claude — contenido en imágenes de carrusel, no accesible.
- 7 plantillas de hook probadas con +1M de vistas — contenido en imágenes de carrusel, no accesible.
- HYPIT, Réplica, combo Playwright/OmniRoute/Headroom/Front Design, "mods" de Claude (multi-sesión + routing por costo + dashboard), lista de "320 skills ordenadas por GitHub stars" — todos gateados detrás de "comentá y te mando por DM". No se persiguieron (ver advertencia de seguridad ya dada).
- Tanda 4: "Blender Skills" (94 skills open-source para que Claude Code maneje Blender vía un plugin), "Graphify" (indexa el codebase en un knowledge graph para que Claude no relea todo cada sesión, hasta 71x menos tokens según benchmark propio), "The Instagram Agent Skill" (11 skills para manejar una cuenta de Instagram entera, incluida una de "viralidad" que analiza reels del nicho), "Sandcastles.ai" (plugin con 14 skills de redes sociales para Claude, incluido el comando `/analyze` para analizar videos en batch), "Skill Spectre" de NVIDIA (escáner de seguridad para skills/tools antes de instalarlas — ver sección de supply-chain ya agregada a `vibecoding-launch-checklist`), "Keyframes" (getkeyframes.com, producto pago que mejora el output de video de Claude), un ranking S-a-B tier de 10 modelos de IA (Claude/ChatGPT en S-tier) — todos vistos una sola vez, sin repo/link confirmado, evaluar antes de instalar.

## Vocabulario de prompts para generación de imagen/video con IA (Higgsfield, Magnific, etc.)
Nombrar el término técnico exacto en el prompt da mucho más control que describir el efecto en palabras propias.
- **Ángulos de cámara:** wide, medium, close up, macro, overhead, fish eye, profile, 3 quarter, over the shoulder, POV, dutch angle, low/high angle, worm's eye view, aerial, lens flare, silhouette.
- **Estilos de iluminación (34, cine clásico + estilizado):** high key, low key, Rembrandt, butterfly, split light, rim light, hard/soft light, golden hour, blue hour, day for night, practical light, volumetric light, neon light, teal and orange, chiaroscuro, silhouette, strobe light — pedir el nombre del estilo en vez de "que se vea cinematográfico".
- **Estilos de animación/motion:** pixel art, chalkboard, holographic foil, bauhaus shapes, neon glow, dithering, clay 3D, halftone dots, kinetic typography, particle swarm, risograph print, glitch, topographic lines, glass morphism, paper cutout, vaporwave grid, flow fields, metaballs, liquid morph, isometric, split flap display, retro VHS, neo-brutalism.
- Para "buen gusto" en diseño de sitios: un prompt genérico tipo "que se vea premium" hace que el modelo promedie hacia lo genérico (gradientes, grids, fade-ins); mejor guardar/escribir prompts ultra-detallados de referencias que ya gustan (layout exacto, timings, jerarquía) y adaptarlos a marca propia, en vez de pedir el adjetivo suelto.

## Teoría de color para web/branding (confirmado por 3 reels independientes con el mismo principio)
Dos colores base neutros/armoniosos hacen el 90% del trabajo (fondo, texto, estructura); un tercer color de alto contraste y acento se reserva EXCLUSIVAMENTE para el botón/CTA que se quiere que el usuario presione — no esparcirlo por todo el diseño. Esparcir el color raro en vez de concentrarlo en el CTA es el error más común.

## Principios de motion/UI design mencionados (ya cubiertos por skills existentes: impeccable, taste-skill, motion-effects)
- Animar con `transform` en vez de cambiar `position`/layout — corre en GPU, no causa reflow, por eso no se traba en mobile.
- Ley de Hick: más opciones visibles = más tiempo de decisión = más abandono → una sola acción principal clara por pantalla.
- Easing: ease-out para elementos que entran, ease-in para los que salen, spring para elementos interactivos — nunca velocidad constante.
- Microinteracciones premium (estilo iOS): lo que hace que una interfaz "se sienta bien" sin que el usuario sepa explicar por qué.
- Timing/reglas concretas de microinteracción (Tanda 4): dropdowns 150-250ms; stagger de filas de lista cada 30ms; botones a `scale(0.97)` al presionar; salidas ~20% más cortas que las entradas; popovers que inician en `scale(0.95)`; transiciones que entran/salen del elemento que las dispara (el trigger), nunca con fade al centro; nada de "spring" en transiciones cotidianas de UI; reusar el mismo layout ID entre elementos compartidos para animaciones de layout fluidas (shared element transition).
- Catálogo de 13 principios para pulir un componente interactivo generado por IA hasta que "se sienta bien" (no solo "funcione"): Fitts's law (targets grandes), jerarquía visual clara, Von Restorff effect (un solo color de acento), object constancy (los valores deslizan, no se reemplazan de golpe), snapping, motion blur en la transición, natural mapping, tabular figures (dígitos de ancho fijo), animar solo el delta que cambió, inercia, feedback multimodal (visual + sonoro), pistas de hover antes de interactuar, skeuomorfismo cuando ayuda a que se entienda sin instrucciones.

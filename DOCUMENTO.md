# Análisis de Reels de Instagram — Documento final

135 reels guardados, analizados con `yt-dlp` (video/caption) + Groq Whisper (transcripción de audio). (3 posts no se pudieron descargar — borrados o privados: 2 de la Tanda 4, 1 de la Tanda 5 — ver `links.md`.)

---

### 1.
## thelandingweb — https://www.instagram.com/p/DcSfP2luzsy/

**Caption:** Comment "SEO" do you know exactly what to do after you publish your website #webdesign #businessowner #entrepreneur #webdesigner

**Transcripción:** 10 things you should do right after publishing your website: set up Google Search Console, submit your sitemap, set up Google Analytics, create a Google Business profile, add your keywords, fix your page titles and descriptions, make sure it looks good on mobile, check your website speed, start building backlinks, and keep your website updated.

**Qué dice / enseña:** Checklist de 10 pasos post-lanzamiento de un sitio web, enfocado en SEO técnico básico y presencia online (Search Console, Analytics, Google Business, sitemap, metadata, mobile, velocidad, backlinks, mantenimiento).

**Herramientas/skills que menciona:** Ninguna skill de IA/código — es un checklist de marketing/SEO manual, no hay comando ni herramienta de agente para "instalar".

**Cómo aplicarlo:** Si tenemos un sitio propio, usar esto como checklist de lanzamiento (no requiere ninguna skill nueva; son pasos manuales en Google Search Console / Analytics / Business Profile).

---

### 2.
## Arastoo — https://www.instagram.com/p/DfKPFDwz2aA/

**Caption:** Glassy Dashboard V8 Modern & Minimal UI ✨. A stunning glassmorphism dashboard featuring elegant translucent elements, smooth visuals, and a premium dark interface. 💎 Modern Glassmorphism Design, Premium Dark UI, Smooth Animations & Effects, Beautiful Blue Glow Accents, Responsive Layout. Built with React.js & CSS3. Comment "Code" to get the code link. #webdevelopment #reactjs #frontend #javascript #css

**Transcripción:** El audio detectado es solo una palabra suelta ("you"), sin contenido hablado real — el reel es puramente visual (showcase del dashboard).

**Qué dice / enseña:** Muestra (visualmente, sin narración) un dashboard con estética glassmorphism: elementos translúcidos, fondo oscuro premium, animaciones suaves y acentos de glow azul. Es una pieza de showcase/portfolio de UI, no un tutorial paso a paso en el propio video — el código se comparte por DM a quien comente "Code".

**Herramientas/skills que menciona:** React.js y CSS3 como stack de construcción. No menciona herramientas de IA ni comandos de agente; es diseño de interfaz hecho a mano/con código tradicional.

**Cómo aplicarlo:** Tomar como referencia visual de estilo (glassmorphism, dark UI, glow accents) para dashboards propios en React/CSS. Si se quiere reproducir, se puede pedir a un asistente de código que genere un dashboard con las mismas características (translucidez vía backdrop-filter, paleta oscura, acentos de color) en lugar de depender del código que regala el autor por DM.

---

### 3.
## CJ — https://www.instagram.com/p/DekASnnAK3z/

**Caption:** Some of my favourite visual hooks I've used this year! Cuando pensás en "hook" es fácil pensar automáticamente en algo verbal (una pregunta, afirmación, etc.) para detener el scroll, pero un hook es en realidad cualquier cosa que capture la atención del viewer lo suficiente para que se detenga en medio del scroll. Y los hooks son importantes, como seguro ya te dijeron hasta el perro. Pero lo que hacés después para que alguien quiera ver el resto del video es igual de importante. Así que divertite con los hooks, pero no gastes toda tu energía solo en ellos.

**Transcripción:** Post sin audio (carrusel de imágenes); se analiza solo con el caption.

**Qué dice / enseña:** Reflexión sobre "hooks" visuales (no solo verbales) en contenido de video corto: un hook es cualquier elemento que capture la atención y detenga el scroll (puede ser visual, no solo una frase o pregunta). Advierte no gastar toda la energía creativa en el gancho inicial — lo que sigue después también importa para retener la atención.

**Herramientas/skills que menciona:** Ninguna herramienta de IA/código — es consejo de creación de contenido/edición de video (técnica narrativa/visual), no técnico.

**Cómo aplicarlo:** Al armar reels o contenido corto, diseñar ganchos visuales (no solo texto o preguntas habladas) en los primeros segundos, y planificar también el desarrollo posterior del video para no depender únicamente del hook inicial.

---

### 4.
## NextWork | Learn AI — https://www.instagram.com/p/DbV3uAZiIxx/

**Caption:** CSS vs. Javascript 🫨. Follow and comment "projects" for hands-on projects to add to your resume (step-by-step guide included)! #ai #coding #vibecoding

**Transcripción:** Sketch de un "jefe" y un desarrollador sobre por qué una animación de menú (slide-in) hecha con "vibe coding" funciona bien en laptop pero traba en el celular. El punto técnico: no es un tema de CSS vs JavaScript como lenguaje, sino de *cómo* se anima. Hay dos formas de mover un elemento que se ven iguales en pantalla: animar la **posición** (cambiar dónde está ubicado realmente en la página) o animar con **transform** (desplazar visualmente el elemento ya pintado, sin mover su posición real). Al animar por posición, el browser tiene que volver a medir (layout) y repintar (paint) todo el layout 60 veces por segundo — algo que un celular no llega a hacer en los ~10ms por frame disponibles, lo que genera el "stutter"/freeze. Al usar `transform`, el navegador no tiene que remedir ni repintar: la GPU simplemente desliza la imagen ya pintada, por eso es mucho más fluido. También aclara que ahí sí importa el lenguaje: tu código JS, el layout y el paint comparten un mismo "carril" (el hilo principal) — si tu JS lo tapona, la animación se traba con él. En cambio, una animación CSS con `transform` corre en su propio carril (compositor), por lo que sigue fluida incluso si el JavaScript está bloqueado. Cierra invitando a crear un proyecto gratis en nextwork.ai con documentación del tema.

**Qué dice / enseña:** Explica la diferencia de performance entre animar la posición de un elemento (layout/reflow + repaint costosos) versus animarlo con `transform` (que corre en la GPU/compositor sin reflow), y por qué eso causa que animaciones "vibe-codeadas" se vean fluidas en desktop pero traben en mobile.

**Herramientas/skills que menciona:** No menciona herramientas de IA/código específicas más allá de "vibe coding" como concepto general (generar código con asistentes de IA sin revisar el detalle de implementación) y la plataforma nextwork.ai para hacer proyectos guiados. No da comandos ni nombres de librerías concretas.

**Cómo aplicarlo:** Al pedirle a una IA que programe animaciones de UI (menús, modales, transiciones), priorizar que use `transform`/`opacity` en vez de propiedades que afecten el layout (`top`, `left`, `width`, `margin`, etc.), especialmente si el target incluye mobile. Es un buen criterio de revisión de código generado por IA: si una animación tiembla o va lenta en celular, revisar si está animando propiedades de layout en vez de `transform`.

---

### 5.
## Ian Tang — https://www.instagram.com/p/DeWzv0mMi8_/

**Caption:** (sin texto de caption)

**Transcripción:** Cuatro tips para diferenciar tus videos hechos con IA (Claude/herramientas de video por IA) de los de otros. Uno: usar efectos open source — como tu video es "frío" (sin estilo propio), la IA puede tomar proyectos existentes; ejemplos: pinceladas con textura, orbes de partículas animadas, entre otros — darle a la IA el link del proyecto y personalizarlo. Dos: usar tu propia música — la música define el ritmo y el mood, es la decisión de dirección de arte más importante; hay que decirle a la IA en qué beats deben caer los movimientos grandes. Tres: archivo de marca (brand file) — color, tipografía, movimiento; agregar tus propios trabajos o referencias antes de que empiece a generar. Cuatro: un sitio web que junta más de 400 videos más los prompts compartidos (no se menciona el nombre exacto del sitio en el audio).

**Qué dice / enseña:** Enseña cómo lograr que un video generado con IA no se vea "genérico" o igual al de cualquier otro, dándole a la herramienta: (1) proyectos/efectos de referencia open source, (2) música propia con indicaciones de sincronización de movimiento a los beats, (3) un archivo de marca con colores/tipografía/estilo de movimiento, y (4) explorar una librería de +400 videos de ejemplo con sus prompts para inspirarse.

**Herramientas/skills que menciona:** Habla genéricamente de "cloud" (probablemente refiriéndose a Claude como herramienta de generación/edición de video por IA, dado el contexto de la cuenta) y de usar un "brand file" (archivo de marca) como input. No da nombres concretos de comandos, repos o el sitio web específico de los 400 videos — queda implícito, no explícito en el audio.

**Cómo aplicarlo:** Antes de generar un video con una herramienta de IA (ej. Claude), preparar: (a) referencias de efectos/proyectos abiertos que quieras reutilizar, (b) la pista de música propia y notas de qué beats deben coincidir con los cortes/movimientos clave, y (c) un "brand kit" propio (paleta, tipografía, ejemplos de estilo de movimiento) para que el resultado no sea genérico. Esto es compatible con la skill `brand-intake` de este entorno, que justamente genera un `brand.md`/`MOTION.md` para que otras skills de video lean antes de animar.

---

### 6.
## Agentic Fact — https://www.instagram.com/p/DfKQ1d6o-r3/

**Caption:** Your AI writes 1,000 lines of code for a job that needs 100. Andrej Karpathy, who coined "vibe coding", asks it "couldn't you just do this instead?" and it happily cuts it down to 100 on the spot. And that's not even its most common mistake: it guesses what you meant and runs with it. So before it starts, tell your AI: list your assumptions first, and stop to ask me if anything is unclear. Write the minimum, nothing I didn't ask for, and if 200 lines could be 50, rewrite them. Only touch the lines this change needs (it sometimes deletes code it doesn't understand). And instead of "fix the bug", say "write a test that reproduces it, then make it pass". The 100 lines were always possible: ask before it starts, not after. Source: Andrej Karpathy's original post on AI coding mistakes, x.com/karpathy/status/2015883857489522876

**Transcripción:** Tu IA escribe mil líneas de código cuando cien alcanzarían. Andrej Karpathy, quien acuñó el término "vibe coding", le pregunta "¿no podrías simplemente hacer esto en su lugar?" y la IA al instante lo reduce a cien líneas. Ese ni siquiera es su error más común: adivina lo que querés y sigue adelante sin confirmar. Por eso hay que decirle a la IA: listá tus supuestos primero, y si algo no está claro, pará y preguntame. Decile: escribí lo mínimo, nada que no haya pedido, y si 200 líneas podrían ser 50, reescribilas. A veces borra código que no entiende, así que decile que toque solo las líneas que este cambio necesita. Y en vez de "arreglá el bug", decile "escribí un test que reproduzca el bug, y después hacelo pasar". Las cien líneas siempre fueron posibles, solo hay que pedirlo antes de que empiece, no después.

**Qué dice / enseña:** Da reglas concretas de prompting para que un asistente de IA (tipo Claude Code/Codex) escriba código más minimalista y seguro, basadas en errores comunes del "vibe coding" (sobre-generar código, asumir intenciones sin preguntar, borrar código que no entiende, "arreglar" bugs sin verificación real).

**Herramientas/skills que menciona:** No menciona herramientas de IA específicas por nombre (más allá de "AI" genérico) ni comandos concretos; es una cita/resumen de un post de Andrej Karpathy sobre errores de vibe coding, con las frases exactas a usar como prompt.

**Cómo aplicarlo:** Agregar estas instrucciones como reglas de prompting o incluso como reglas permanentes (ej. en un CLAUDE.md/AGENTS.md) al trabajar con un asistente de código: pedirle que liste sus supuestos y pregunte si algo no está claro antes de empezar, que escriba el mínimo código necesario, que solo toque las líneas que el cambio requiere, y que para bugs escriba primero un test que reproduzca el problema antes de "arreglarlo".

---

### 7.
## Austin Myers | AI Strategist for Brands and Business — https://www.instagram.com/p/DfKl-EPM0oI/

**Caption:** Follow and comment GUIDE for the step by step! Share with a friend ready to grow faster w AI. I'm leveling the playing field. Because I think people are tired of being TOLD they can edit videos with Claude and want to be shown HOW. So here's the entire thing. Every prompt. Every step to start editing your videos with Claude (or ChatGPT!). Because I want you to see HOW it's done. If you're building a business or a brand, but like me also between a 9-5, marriage, kiddos, and life. And just need to make the most of the time you have… My page is for you!

**Transcripción:** Flujo paso a paso para editar videos usando Claude (o ChatGPT/Codex) como editor de video:
1. Crear una carpeta en la computadora (ej. "AI Video Editor"); si usás Claude, abrir esa carpeta desde la tab de Code; si usás ChatGPT, usar Codex con el mismo esquema.
2. Darle a la IA un prompt que le indique qué herramientas necesita para editar videos, que también cree cuatro carpetas para organizar videos y ediciones.
3. Configurar un workflow limpio con otro prompt que simplifique cada paso siguiente.
4. Pasarle un prompt para que tenga una buena base de diseño de movimiento (motion design) para tus ediciones.
5. Crear tu "estilo de firma" (signature style) con un prompt, subiendo 3-4 videos propios, tus fuentes y colores de marca, y guardarlo.
6. Filmar el video y subirlo al chat, diciendo "let's edit this reel". Primero hace un "rough cut" (sacar tomas malas y silencios) y te lo presenta — hay que escucharlo con sonido para validar los cortes.
7. Si el rough cut está bien, dar dirección creativa (cómo querés que se sienta la historia del video); la IA genera un storyboard visual para revisar y ajustar.
8. Al aprobar el storyboard, la IA construye una apertura de 10-15 segundos para revisar.
9. Al aprobar la apertura, se edita el video completo siguiendo el storyboard; se puede pedir ajustes puntuales por timestamp (ej. "a los 6 segundos, hacé este cambio").
10. Al aprobar, decir "I approve this, make this final version" y queda lista para publicar, guardada en la carpeta de proyectos.
11. El feedback y los ajustes se guardan como "learnings" para que el editor de video mejore con el feedback futuro.
Menciona que convirtió todo esto en una guía completa (pedirla comentando "GUIDE").

**Qué dice / enseña:** Un workflow completo para usar Claude (o ChatGPT/Codex) como editor de video de extremo a extremo: desde armar la estructura de carpetas y el "signature style" de marca, hasta el rough cut automático, dirección creativa, storyboard, apertura, edición final y guardado de feedback/aprendizajes para iteraciones futuras.

**Herramientas/skills que menciona:** Claude (tab de "Code"), ChatGPT, Codex. Habla de crear carpetas específicas, prompts para configurar herramientas y "estilo de firma" (brand/motion style), y de un sistema de feedback que se guarda como "learnings". No da el texto literal de los prompts (dice que están en la guía que comparte por DM).

**Cómo aplicarlo:** Replicar el flujo en este entorno: crear una carpeta de proyecto con subcarpetas (raw footage, ediciones, assets de marca, outputs), definir un "signature style" (colores, fuentes, ejemplos de movimiento) similar a lo que hace la skill `brand-intake` (genera `brand.md`/`MOTION.md`), y pedirle a Claude que haga primero un rough cut, después un storyboard según dirección creativa, luego una apertura corta, y finalmente la edición completa — iterando por timestamp y guardando el feedback para mejorar futuras ediciones.

---

### 8.
## Byron — https://www.instagram.com/p/Dei6J0AvlXw/

**Caption:** Plenty of animation styles you can get Claude to do for you 🚀 #ai #aitools #claude #chatgpt #figma

**Transcripción:** Lista hablada (narración tipo catálogo) de estilos de animación/visuales que se le pueden pedir a Claude: Liquid Morph, ASCII Art, Holographic Foil, Bauhaus Shapes, Neon Glow, Dithering, Clay 3D, Halftone Dots, Kinetic Typography, Pixel Art, Particle Swarm, Risograph Print, Glitch Effect, Topographic Lines, Glass Morphism, Paper Cutout, Vaporwave Grid, Flow Fields, Metaballs ("Metabores" en el audio), Raymarched Fractals.

**Qué dice / enseña:** Es un catálogo/inspiración de estilos visuales y de animación (mayormente estéticas de motion design y shaders/efectos) que se pueden pedir como prompt a Claude para generar piezas visuales, sin explicar el "cómo" paso a paso ni mostrar código.

**Herramientas/skills que menciona:** Menciona Claude, ChatGPT y Figma en los hashtags como herramientas de IA/diseño con las que se pueden lograr estos estilos, pero no da prompts textuales ni instrucciones técnicas concretas — es solo la lista de nombres de estilos.

**Cómo aplicarlo:** Usar esta lista como banco de referencias/vocabulario al pedirle a Claude (o a las skills de motion de este entorno, como `motion-effects` o `motion-prompt-writer`) que genere un efecto visual específico — por ejemplo "hacé un título con estilo Kinetic Typography" o "animá esto como Particle Swarm" — en vez de describir el efecto desde cero.

---

### 9.
## Natalie Data Engineer — https://www.instagram.com/p/DehMUh_jdbK/

**Caption:** ok my reel was viral and i know you all want to paste this whole list into claude 😊 so i put all 111 in here (and text in the comments). go save it

**Transcripción:** Post sin audio — es un carrusel de imágenes (yt-dlp no encontró formatos de video en ninguna de sus slides; se recuperó solo la metadata/caption, no el contenido de las imágenes). No hay transcripción posible.

**Qué dice / enseña:** Por el caption, el post comparte una lista de "111" ítems (aparentemente datos/skills/herramientas, dado el contexto de la cuenta "Data Engineer") pensada explícitamente para pegar en Claude, pero el contenido real de la lista está en las imágenes del carrusel (no accesibles como texto desde acá) y/o en los comentarios del post original, no en el caption.

**Herramientas/skills que menciona:** Menciona a Claude como destino de la lista ("paste this whole list into claude"), pero no se puede ver qué lista es ni qué skills/herramientas concretas contiene, porque el contenido está en imágenes no legibles desde este análisis.

**Cómo aplicarlo:** No se puede aplicar el contenido concreto sin ver las imágenes del carrusel o los comentarios del post original (donde según el caption está el texto completo de los 111 ítems). Si se quiere aprovechar esta idea, habría que abrir el post manualmente en Instagram para copiar esa lista y recién ahí definir cómo usarla con Claude.

---

### 10.
## Mino Lee — https://www.instagram.com/p/DfIBHJ5iHI4/

**Caption:** comment "HOOKS" and i'll DM u all of my 255 viral hooks👇. i went through 738 of my reels and ranked every hook by real views. every one of these 7 has a reel over a million. steal the template, swap in ur own story. #1 is my best hook ever, 10 of the 37 reels i used it on went over 1M. and please stop opening with "today we're gonna be talking about…" mine got 2,191 views lol. comment "HOOKS" and i'll DM u all of my 255 viral hooks👇

**Transcripción:** Post sin audio — es un carrusel de imágenes (yt-dlp no encontró formatos de video en ninguna de sus slides; se recuperó solo la metadata/caption, no el contenido de las imágenes). No hay transcripción posible.

**Qué dice / enseña:** Por el caption, el post presenta 7 "hooks" (ganchos de apertura) para reels, cada uno probado en reels propios que superaron 1 millón de vistas (de un análisis de 738 reels propios). Advierte explícitamente que abrir un video con "today we're gonna be talking about…" es un hook débil (ejemplo propio con solo 2,191 vistas). El contenido real de las 7 plantillas de hook está en las imágenes del carrusel, no accesible desde este análisis.

**Herramientas/skills que menciona:** No menciona herramientas de IA/código — es consejo de guion/estructura narrativa para reels (copywriting de hooks), no técnico.

**Cómo aplicarlo:** No se puede replicar el contenido exacto de los 7 hooks sin ver las imágenes del carrusel (o pedírselos por DM comentando "HOOKS", como indica el autor). Como principio general aplicable igual: evitar aperturas tipo "hoy vamos a hablar de…" y en su lugar usar un gancho validado por datos propios (ver qué reels anteriores tuvieron mejor retención/vistas en los primeros segundos y reusar esa estructura).

---

### 11.
## Steven Law — https://www.instagram.com/p/DeqPXZguZOm/

**Caption:** how many do you know? 👇 #ai #claudecode #aiagents #learnai #buildinpublic

**Transcripción:** Veamos si realmente sabés de IA. LLMs, tokens, context windows, temperature, hallucination, system prompt, RAG, embeddings, vector databases, fine tuning, tool calling, MCP, agents, subagents, prompt caching, evals y context engineering. Si conocés eso, entonces sabés de IA. Así que vayan a construir algo, o seguime.

**Qué dice / enseña:** Es un "quiz"/checklist de conceptos clave del ecosistema de IA/LLMs que, según el autor, hay que conocer para decir que "sabés de IA": desde fundamentos (tokens, context window, temperature, hallucination, system prompt) hasta técnicas más avanzadas (RAG, embeddings, vector databases, fine-tuning, tool calling, MCP, agents, subagents, prompt caching, context engineering).

**Herramientas/skills que menciona:** Menciona MCP (Model Context Protocol) y "agents"/"subagents" como conceptos, y Claude Code en los hashtags (#claudecode), pero no da definiciones, comandos ni pasos concretos — es solo el listado de términos.

**Cómo aplicarlo:** Usar la lista como checklist personal de conceptos a dominar si se trabaja construyendo agentes o productos con IA (y como glosario de términos a buscar si alguno no es familiar: RAG, embeddings, vector databases, fine-tuning, tool calling, MCP, context engineering, prompt caching, evals).

---

### 12.
## Anthony Chávez | Usuarios para tu App — https://www.instagram.com/p/DfKRNMzRf13/

**Caption:** No construyas más features construyes tu moats defensivos que ningún otro Vibecoder te podrá quitar tan fácilmente.

**Transcripción:** Explica el concepto de "moat" (foso defensivo) aplicado a apps construidas con IA (Claude/Codex). Con herramientas como Claude, el código se puede replicar en una tarde, así que lo que protege un negocio ya no es la feature sino el foso. Da 4 tipos de moat: (1) Efecto de red (ej. WhatsApp: tus contactos ya están ahí), (2) Costo de cambiarte (ej. Spotify: perder tus playlists), (3) Datos propios (ej. Waze: datos de tráfico de millones de usuarios), (4) Confianza (ej. Mercado Libre: garantía de devolución). Ninguno de los cuatro se copia con un prompt. Recomienda elegir uno desde el día uno: que el usuario deje algo que se quede, invite a otros, o confíe en la app.

**Qué dice / enseña:** Que en la era del "vibecoding" (construir apps rápido con IA), la ventaja competitiva ya no está en el código (fácilmente replicable) sino en moats defensivos: efecto de red, costos de cambio, datos propios o confianza/reputación.

**Herramientas o skills de IA/código que menciona:** Menciona Claude y Codex como las herramientas de IA que permiten clonar código rápidamente (el contexto que hace necesario el moat), pero no enseña ningún comando, skill o workflow concreto de código — es un concepto de estrategia de producto, no un tutorial técnico.

**Cómo aplicarlo:** Antes de construir más features, identificar cuál de los 4 moats aplica al proyecto propio (red, switching cost, datos, confianza) y diseñar el producto para reforzar ese moat desde el inicio, en vez de competir solo en velocidad de desarrollo con IA.

---

### 13.
## Cooked Dev — https://www.instagram.com/p/DfFSwGNIyrU/

**Caption:** Anything I forgot? Drop it below 👇 #buildinpublic #ai #vibecoding #appsecurity #app

**Transcripción:** Lista de checklist de seguridad para una app antes de lanzarla: ocultar API keys, revisar variables de entorno, proteger rutas de admin, agregar autenticación correcta, revisar accesos de usuario, sanitizar formularios, proteger contra XSS, agregar rate limiting, asegurar endpoints de API, revisar configuración de CORS, agregar security headers, apagar debug mode, actualizar dependencias, quitar paquetes sin usar, revisar archivos expuestos, asegurar la base de datos, hashear passwords correctamente, revisar el historial de git por secretos filtrados, y correr una auditoría de seguridad completa.

**Qué dice / enseña:** Checklist de seguridad (security audit) pre-lanzamiento para una app "vibecodeada", cubriendo manejo de secretos, auth, sanitización de inputs, rate limiting, hardening de infraestructura y dependencias.

**Herramientas o skills de IA/código que menciona:** No menciona ninguna herramienta o skill específica de IA/código — es una checklist genérica de buenas prácticas de seguridad aplicable a cualquier stack, sin nombrar comandos ni productos concretos.

**Cómo aplicarlo:** Usar esta lista como checklist manual antes de publicar cualquier proyecto propio: revisar env vars/API keys, auth en rutas admin, sanitización de forms, rate limiting, headers de seguridad, dependencias actualizadas y grep del historial de git por secretos filtrados.

---

### 14.
## Gin Lee — https://www.instagram.com/p/DZI6s_dRoe6/

**Caption:** Why simple videos work best sometimes! If you're working in a b2b company, adding too much style/motion can bother your client reading the message. That's why the more complex the product, the more clear and simple your video should be.

**Transcripción:** Diálogo entre dos personas (cliente y diseñador) sobre un video comercial. El diseñador explica que, al ser un video para una empresa B2B (que vende a otros negocios con productos/problemas complejos), el video debe priorizar claridad por sobre estilo. Los comerciales estilizados funcionan mejor en B2C (productos simples para consumidores finales). La ventaja de un video simple en B2B es que permite producir más variaciones y campañas manteniendo leads consistentes.

**Qué dice / enseña:** Que el nivel de "styling"/motion en un video comercial debe ser inverso a la complejidad del producto: productos complejos (típico B2B) necesitan videos simples y claros; productos simples (típico B2C) permiten videos más estilizados y decorativos. Además, los videos simples facilitan producir más variaciones de campaña.

**Herramientas o skills de IA/código que menciona:** Ninguna — es un principio de estrategia de diseño/marketing de video, sin mencionar ninguna herramienta de IA o código.

**Cómo aplicarlo:** Al crear contenido de video para un producto o servicio B2B/técnico, priorizar claridad y simplicidad visual sobre motion/estilo elaborado, y aprovechar esa simplicidad para generar más variaciones de creatividades/anuncios con menos esfuerzo.

---

### 15.
## Vibe Coder — https://www.instagram.com/p/DfHz54iOso8/

**Caption:** How to avoid unexpected bills. #vibecoding #claudecode #ai

**Transcripción:** Historia de alguien que recibió una factura de servidor de $14,000 porque un bot encontró su app a las 2am y la golpeó 40 millones de veces; cada hit corría la IA y eso se cobraba. Explica 3 medidas que usan ingenieros reales para evitarlo: (1) Rate limiting — cada visitante tiene 100 requests por minuto, después de eso se bloquea, y un request bloqueado cuesta casi nada; (2) Rutas caras protegidas — cualquier endpoint que corre la IA debe requerir login (sin cuenta, no hay IA); (3) Tope de gasto — alerta por email a $50, corte automático a $100, así en el peor caso se pausa la app, no la cuenta bancaria. Termina con un prompt de ejemplo: "Claude, add rate limiting, require a login for the AI, and cap spending at $100."

**Qué dice / enseña:** Cómo evitar facturas de servidor/IA inesperadamente altas por ataques de bots o abuso, mediante rate limiting, requerir autenticación en endpoints que llaman a un modelo de IA, y configurar un tope de gasto (spend cap) con alertas.

**Herramientas o skills de IA/código que menciona:** Menciona Claude (Claude Code) como el agente al que se le pide implementar estas protecciones mediante un prompt directo ("Claude, add rate limiting, require a login for the AI, and cap spending at $100"), pero no detalla una skill o comando específico más allá de ese prompt.

**Cómo aplicarlo:** En cualquier app propia que use una API de IA, pedirle al agente de código (ej. Claude Code) que implemente rate limiting por visitante, requiera login para cualquier endpoint que invoque IA, y configure un tope de gasto con alertas (ej. aviso a $50, corte a $100) para evitar sorpresas de facturación.

---

### 16.
## Arthur — https://www.instagram.com/p/DfAZMAjseOQ/

**Caption:** How to make cuts like in the movies 🎬 Day 9/365 #storytelling #videoediting #filmmaking #editingtips #cinematic

**Transcripción:** Técnica de edición de video llamada "cortes invisibles": el siguiente plano debe comenzar exactamente en el mismo punto donde estaban los ojos del espectador al final del plano anterior. Mover la mirada del espectador hacia un nuevo punto de foco permite cortar sin incomodidad visual para la audiencia. Recomienda usar esta técnica en todos los videos.

**Qué dice / enseña:** Técnica de edición de video (match cut / continuidad de mirada): alinear el punto de foco visual entre el final de un plano y el inicio del siguiente para lograr transiciones fluidas e "invisibles" al espectador.

**Herramientas o skills de IA/código que menciona:** Ninguna — es una técnica de edición de video tradicional (cinematografía/montaje), sin mencionar herramientas de IA ni código.

**Cómo aplicarlo:** Al editar video (reels, contenido de marca, tutoriales), planear los cortes para que el nuevo plano arranque en el mismo punto donde el ojo del espectador quedó fijo en el plano anterior, logrando transiciones más profesionales y menos abruptas.

---

### 17.
## Ugoki AI — https://www.instagram.com/p/DfAvhRORrIB/

**Caption:** Want to learn AI-powered motion design? DM us UGOKI and we'll send you the link 🔥 #claude #motiondesign

**Transcripción:** Explica cómo lograr el efecto de "glass" (vidrio) estilo iOS 26 correctamente, en vez del error común (un rectángulo blanco algo transparente y borroso, que es solo un filtro, no vidrio real). El vidrio real hace 3 cosas: refracta (lo que está detrás se magnifica en el centro y se dobla en los bordes), capta la luz (un borde delgado brillante recorre su filo) y refleja (un destello se desliza mientras se mueve). Con esas tres palabras (refracción, borde, reflejo) Claude puede escribir el shader.

**Qué dice / enseña:** Cómo describir correctamente el efecto visual "glassmorphism" estilo iOS 26 para que una IA genere un shader fiel: diferenciando un vidrio real (que refracta, capta luz y refleja) de un simple filtro translúcido/blur.

**Herramientas o skills de IA/código que menciona:** Menciona a Claude como la IA que, a partir de las palabras clave "refracción, borde (rim), reflejo", puede escribir el shader del efecto de vidrio. No da el prompt completo ni un comando específico, solo el concepto/vocabulario a usar.

**Cómo aplicarlo:** Al pedirle a Claude (o cualquier IA generativa de código) un efecto de vidrio/glassmorphism, especificar explícitamente los tres componentes técnicos — refracción, brillo en el borde (rim light) y reflejo dinámico — en vez de describirlo solo como "transparente y borroso", para obtener un shader más realista.

---

### 18.
## Griffin Wooldridge — https://www.instagram.com/p/DfGCFq_KBl7/

**Caption:** AI slop vs. senior designer

**Transcripción:** Describe una tendencia donde diseñadores muestran antes/después de "AI slop" (diseño genérico de IA) transformado en interfaces de usuario pulidas. La tendencia la inició Damir Sokolovsky con un video en X mostrando los pasos exactos para convertir un dashboard genérico en una UI moderna que parece hecha por un diseñador senior; ese video superó 1 millón de views. Sokolovsky planea lanzar una "skill" que empaqueta sus principios de diseño. Otros diseñadores también publicaron antes/después similares en apps móviles, diseño web, etc.

**Qué dice / enseña:** Que existe una tendencia viral de mostrar cómo transformar interfaces genéricas generadas por IA ("AI slop") en diseños de nivel "senior designer" aplicando principios de diseño concretos, y que esos principios se están empaquetando como una "skill" reutilizable para mejorar el output de diseño de agentes de IA.

**Herramientas o skills de IA/código que menciona:** Menciona a Cloud Code (Claude Code) como uno de los agentes de IA cuyo output de diseño se busca mejorar, y menciona que Damir Sokolovsky va a lanzar una "skill" que empaqueta sus principios de diseño para ese fin — sin detallar aún el contenido de esa skill.

**Cómo aplicarlo:** Estar atento al lanzamiento de skills de diseño (como la que menciona Sokolovsky) para mejorar el output visual de agentes como Claude Code, y en el mientras, revisar ejemplos de antes/después de "AI slop" a UI pulida para identificar qué principios de diseño aplicar manualmente a los propios proyectos (jerarquía, espaciado, tipografía, etc.).

---

### 19.
## Ugoki AI — https://www.instagram.com/p/De_P7Y7RfrR/

**Caption:** Do you want to create this kind of motion design using AI? Comment UGOKI and we'll send you the link 🔥 #claude #motiondesign

**Transcripción:** El post no tiene narración hablada; la transcripción solo detectó "Music" (música de fondo), sin diálogo ni voz en off. Se analiza únicamente con el caption.

**Qué dice / enseña:** A partir del caption: promociona un tipo de motion design generado con IA (asociado a Claude), e invita a comentar "UGOKI" para recibir el link con más información/tutorial — es contenido promocional de la cuenta Ugoki AI, no explica una técnica específica en el propio post.

**Herramientas o skills de IA/código que menciona:** Menciona a Claude (vía el hashtag #claude) como la IA usada para el motion design mostrado, pero no explica ningún método, prompt o skill concreto en el contenido visible (caption/transcripción).

**Cómo aplicarlo:** No hay suficiente información técnica en este post para aplicar directamente; serviría como referencia visual de qué es posible lograr en motion design con Claude, pero habría que conseguir el link/guía mencionado en el caption para los detalles del método.

---

### 20.
## Opus Jake — https://www.instagram.com/p/De6vxpANdgK/

**Caption:** Comment MOD and I'll send you all 3 mods + the setup guide. Estos 3 "mods" ayudan a que Claude trabaje entre chats, optimice el gasto de tokens y den un dashboard totalmente personalizado: (1) Connected chats — sesiones de Claude que hablan entre sí y comparten contexto (una investiga prospectos mientras otra usa esos hallazgos para preparar el outreach); (2) Smarter model routing — asigna cada prompt al modelo más costo-efectivo (modelos livianos para tareas simples, modelos potentes para trabajo difícil); (3) Custom dashboard — personaliza la apariencia de Claude y organiza tareas, mensajes, calendario y widgets.

**Transcripción:** Presenta "mods" para Claude como la actualización más grande y poco conocida. Tres formas de usarlos: (1) Hacer que las sesiones de Claude hablen entre sí — una sesión hace prospecting, otra hace cold outreach, y otra puede actuar de manager coordinando; (2) Optimizar el uso/gasto configurando un mod que siempre use el modelo más costo-efectivo, para no gastar créditos de más en tareas simples; (3) Personalizar visualmente Claude con un dashboard integrado que incluya to-do list, mensajes pendientes, etc. Invita a comentar "mod" para recibir el setup.

**Qué dice / enseña:** Que existen "mods" (modificaciones/personalizaciones) para Claude que permiten: comunicación entre múltiples sesiones/chats de Claude compartiendo contexto, routing automático de modelo según costo-efectividad de la tarea, y un dashboard personalizado dentro de la interfaz de Claude.

**Herramientas o skills de IA/código que menciona:** Menciona "mods" para Claude (sesiones conectadas entre sí, model routing por costo, dashboard personalizado), pero no da detalles técnicos de implementación en el propio video — solo el concepto y una invitación a pedir la guía de setup por fuera.

**Cómo aplicarlo:** Evaluar si conviene configurar sesiones de Claude que se comuniquen entre sí para flujos de trabajo encadenados (ej. research → outreach), aplicar un criterio de selección de modelo según la complejidad de cada tarea para ahorrar costos, y personalizar el dashboard/interfaz de Claude para centralizar tareas y mensajes — aunque el setup concreto habría que conseguirlo por el canal que ofrece la cuenta.

---

### 21.
## Opus Jake — https://www.instagram.com/p/DfBm-FQN70S/

**Caption:** Comment "VIRAL" and I'll DM you the full setup. Claude Code puede convertir un video de referencia en un workflow de contenido editable para tu marca. La herramienta se llama HYPIT y le da a tu agente de IA las herramientas para reconstruir la estructura, captions, B-roll y efectos de un video. Le das una referencia, explicás qué querés cambiar, y construye una versión alrededor de tu propio producto, servicio o marca personal. Workflow: 1) elegir un video de referencia con un formato que encaje con tu audiencia; 2) darle a Claude Code el video, tus assets de marca y un brief claro usando la skill HYPIT; 3) adaptar mensaje y visuales a tu propia oferta; 4) crear variaciones con distintos hooks, captions y ángulos creativos; 5) revisar resultados, publicar las versiones más fuertes y usar el desempeño para guiar el próximo batch. HYPIT es gratis; el agente de código y los modelos de generación pagos pueden tener costos aparte.

**Transcripción:** Presenta "Hyped Skill" (HYPIT) como una skill gratuita para Claude que permite "robar" cualquier video viral: no solo da guiones, sino que genera videos completos. Le das un video de referencia y lo reconstruye toma por toma con la misma edición, animaciones, captions e incluso las personas, permitiendo clonar formatos de creadores virales y recrearlos con tu propio producto o servicio con un solo prompt. Una vez que encontrás un video que te gusta, podés generar 100 variaciones instantáneamente con distintos hooks, captions o animaciones. Para instalarlo: pegar el link en Claude y decir "install skill".

**Qué dice / enseña:** Cómo usar una skill llamada HYPIT en Claude Code para tomar un video de referencia viral y reconstruirlo automáticamente (estructura, captions, B-roll, efectos) adaptado a la marca/producto propio, generando además múltiples variaciones de hooks/captions/animaciones para testear qué formato funciona mejor.

**Herramientas o skills de IA/código que menciona:** Menciona explícitamente Claude Code y la skill "HYPIT" (también llamada "Hyped Skill" en la narración), que se instala pegando un link en Claude y escribiendo "install skill". Es una skill gratuita; los costos aparte son del agente de código y de los modelos de generación de video/imagen usados.

**Cómo aplicarlo:** Instalar la skill HYPIT en Claude Code (pegando el link del repo/skill y escribiendo "install skill"), elegir un video de referencia viral cuyo formato encaje con la audiencia propia, darle a Claude Code ese video + assets de marca + un brief claro, y usarlo para generar variaciones de contenido (distintos hooks/captions/ángulos) a partir de un mismo formato, iterando según el desempeño de cada batch publicado.

---

### 22.
## moe.dev — https://www.instagram.com/p/De9wgwxRnw8/

**Caption:** You tapped Pay twice. Did you get charged twice? Depends who built the checkout. 💳 Locked buttons + order IDs (devs call it an idempotency key) mean one tap = one charge. Invisible details, part 3. Follow for the next one.

**Transcripción:** Al tocar "Pay" si no pasa nada, la gente vuelve a tocar y termina pagando doble. Los checkouts bien hechos evitan esto con dos trucos: 1) Al tocar el botón, este se bloquea, se pone gris y dice "Processing", así un segundo tap no hace nada. 2) Cada orden recibe su propio ID (idempotency key); si el servidor recibe la misma orden dos veces, sabe que es un duplicado y cobra una sola vez.

**Qué dice / enseña:** Explica el patrón de idempotencia en checkouts de pago: bloqueo de botón tras el primer click + ID único de orden para evitar cobros duplicados cuando el usuario reintenta un pago.

**Herramientas o skills de IA/código que menciona:** No menciona ninguna herramienta o skill de IA/código específica. Es un concepto de arquitectura de backend (idempotency key), aplicable manualmente en cualquier stack.

**Cómo aplicarlo:** En cualquier flujo de pago o acción crítica (checkout, envío de formulario), implementar: (1) deshabilitar/cambiar el estado del botón inmediatamente al hacer click para prevenir doble envío, y (2) generar un idempotency key único por transacción en el backend para que, si la misma request llega duplicada, se ignore y no se cobre/ejecute dos veces.

---

### 23.
## Pramesh — https://www.instagram.com/p/DcvDIeAvkqN/

**Caption:** Stop Vibecoding fake sites. Do these instead

**Transcripción:** La transcripción de audio quedó casi vacía (solo se detectó la palabra "The"); el contenido real del video parece depender de texto/overlays visuales que el audio no capta, por lo que no se pudo recuperar el mensaje completo desde el audio.

**Qué dice / enseña:** Según la caption, el video advierte contra "vibecodear" sitios falsos/poco sólidos y propone alternativas, pero no se pudo determinar el contenido específico (los pasos o alternativas) porque la transcripción de audio no capturó el contenido real del reel.

**Herramientas o skills de IA/código que menciona:** No se puede determinar con certeza desde el audio disponible; la caption menciona "vibecoding" de forma genérica pero no nombra una herramienta o skill concreta.

**Cómo aplicarlo:** No se puede dar una aplicación concreta sin ver el contenido visual del reel (probablemente texto en pantalla). Recomendación: revisar el post directamente en Instagram para extraer los pasos, ya que el análisis automático por audio no fue suficiente en este caso.

---

### 24.
## Hayden Smith | Anti-Hype AI Educator — https://www.instagram.com/p/DZsXW-HonCi/

**Caption:** 5 ways your vibecoded login endpoint isn't secure #claudecode #vibecoder #vibecoding #startuphacks #aicoding

**Transcripción:** Cuando Claude Code agrega una pantalla de login a tu app "vibecodeada", esa pantalla suele ser lo más fácil de hackear. 5 fallas comunes (todas corregibles pidiéndoselo a la IA): 1) El session token vive en local storage, lo que lo expone a ataques de cross-site scripting (XSS). 2) La verificación de admin se hace en el cliente y no en el servidor. 3) No hay autenticación de dos factores (2FA) ni verificación de email, por lo que cualquiera puede registrarse como cualquiera. 4) El endpoint de login y el de reset de password no tienen rate limiting, lo que permite ataques de fuerza bruta. 5) No hay reglas de contraseña ni verificación de contraseñas filtradas (leaked password check).

**Qué dice / enseña:** Lista 5 vulnerabilidades típicas en pantallas de login generadas por IA/vibecoding: almacenamiento inseguro de tokens de sesión, validación de permisos solo en el cliente, falta de 2FA/verificación de email, falta de rate limiting en login/reset de password, y falta de políticas de contraseñas seguras.

**Herramientas o skills de IA/código que menciona:** Menciona Claude Code como la herramienta que generó el login, pero no nombra un plugin o skill específico para arreglar las fallas; dice que son "cambios vibecodeables" (se le pueden pedir directamente al agente de IA).

**Cómo aplicarlo:** Al revisar cualquier login hecho con IA, pedirle explícitamente al agente (ej. Claude Code) que: mueva el session token a un almacenamiento seguro (ej. httpOnly cookie) en vez de local storage, valide permisos de admin en el servidor (no solo en el cliente), agregue 2FA y verificación de email al registro, implemente rate limiting en los endpoints de login y reset de password, y agregue reglas de contraseña fuertes más chequeo contra listas de contraseñas filtradas.

---

### 25.
## Vibe Coder — https://www.instagram.com/p/De9o_48uz8N/

**Caption:** How do engineers safely deploy to prod? #claudecode #claude #vibecode

**Transcripción:** Muestra cómo desplegar a producción manualmente (SSH, git pull, npm install, build, restart) puede fallar fácilmente, por ejemplo si te olvidás de correr una migración de base de datos y el sitio se cae. La solución en equipos reales es automatizar con CI/CD: - Rollback: la última versión buena vuelve a estar en producción en segundos si algo falla. - CI (Continuous Integration): cada push dispara automáticamente los mismos checks (instalar dependencias, lint, tests, build, escaneo de vulnerabilidades); si un test falla, el pipeline se pone en rojo y bloquea el merge (así se detecta, por ejemplo, una migración faltante antes de llegar a prod). - CD (Continuous Delivery/Deployment): una vez que el CI está verde, la app se empaqueta una sola vez en un artefacto de release (ej. imagen Docker) que primero va a staging (una copia de producción) donde se corren health checks. Con Continuous Delivery un humano aprueba el pase a producción; con Continuous Deployment no hay botón, si está verde se despliega solo. El despliegue es gradual (canary): primero 5% de los usuarios, luego 25%, 50%, 100%; si los errores suben, se hace rollback automático sin intervención manual. Todo esto se define en un solo archivo del repo, con los mismos pasos y el mismo orden siempre.

**Qué dice / enseña:** Enseña el concepto de pipelines de CI/CD: por qué el despliegue manual a producción es riesgoso, y cómo CI (tests/lint/build automáticos en cada push) + CD (empaquetado en artefacto, paso por staging, despliegue gradual tipo canary y rollback automático) hacen que los deploys sean seguros y repetibles.

**Herramientas o skills de IA/código que menciona:** Menciona Claude (Claude Code) como el agente al que se le pide "configurar un pipeline y desplegar", pero no nombra un plugin o herramienta de CI/CD específica (tipo GitHub Actions, Docker, etc.) más allá de los conceptos genéricos.

**Cómo aplicarlo:** Para cualquier proyecto propio, en vez de desplegar a mano por SSH, configurar un pipeline de CI/CD (por ejemplo con GitHub Actions u otra herramienta) definido en un archivo del repo que: corra automáticamente lint, tests, build y escaneo de seguridad en cada push; bloquee el merge si algo falla; empaquete un artefacto único (ej. imagen Docker) que pase primero por staging; y despliegue gradualmente a producción (canary) con rollback automático si los errores aumentan. Se le puede pedir a un agente de IA como Claude que genere y configure ese pipeline.

---

### 26.
## Ben Broch | AI Saas builder — https://www.instagram.com/p/Derh6MRlvot/

**Caption:** Comment UX and I'll send you the checklist. Hick's Law is why Tinder, Snapchat and TikTok each want you to do just one thing: every extra option makes people slower to decide, and slow people leave.

**Transcripción:** Si estás construyendo una app, no le dés demasiadas opciones al usuario. Apps como Tinder, Snapchat y TikTok hacen que quieras hacer una sola cosa (swipear, enviar fotos, seguir scrolleando), siguiendo la Ley de Hick: cuantas más opciones le das a alguien, más tarda en decidir, y la gente que tarda se va. 5 reglas: 1) Cada pantalla debe tener una acción principal obvia. 2) El botón principal debe verse más importante que todo lo demás alrededor. 3) Esconder las opciones avanzadas hasta que alguien las necesite. 4) Nunca tener dos botones que se vean igual de importantes. 5) Si una opción no es relevante todavía, no mostrarla.

**Qué dice / enseña:** Explica la Ley de Hick (Hick's Law) aplicada a diseño de UX/UI: más opciones visibles = más tiempo de decisión = más abandono. Da 5 reglas concretas de jerarquía visual y simplicidad de interfaz para mantener una sola acción principal clara por pantalla.

**Herramientas o skills de IA/código que menciona:** No menciona ninguna herramienta o skill de IA/código específica. Es un principio de diseño UX aplicable manualmente en cualquier producto.

**Cómo aplicarlo:** Al diseñar cualquier pantalla de una app o sitio propio: definir una sola acción principal obvia por pantalla, hacer que el botón principal destaque visualmente por sobre el resto, ocultar opciones avanzadas o secundarias hasta que el usuario las necesite, evitar que dos botones compitan en importancia visual, y no mostrar opciones que todavía no son relevantes para el usuario en ese momento.

---

### 27.
## Santiago Remedio — https://www.instagram.com/p/De9s2N0RISw/

**Caption:** Comentá CLAUDE ⤵️

**Transcripción:** El creador recomienda nunca usar Claude Code antes de instalar 5 plugins: 1) Playwright — le da "ojos" a Claude para que pueda ver específicamente lo que está pasando en la pantalla (Claude no puede ver tu pantalla por sí mismo, así que básicamente adivina sin esto). 2) OmniRoute — cuando llegás al límite de uso te cambia automáticamente a otro modelo antes de que termines la tarea, para que nunca te quedes sin créditos. 3) Headroom — al armar un prompt, lee toda la información disponible, incluso la que no es necesaria; este plugin filtra esa información irrelevante para usar los tokens solo en lo que realmente importa. 4) Un plugin de "palacio mental" (memoria persistente) — evita tener que recrear el contexto del proyecto cada vez que abrís una ventana nueva, dejando una memoria permanente del proyecto. 5) Front Design — cuando Claude diseña algo, por defecto da un diseño genérico que se nota hecho con IA; este plugin hace que los diseños sean mucho más profesionales, como hechos por alguien con años de experiencia.

**Qué dice / enseña:** Recomienda 5 plugins/skills para mejorar el uso de Claude Code: dar visión de pantalla (Playwright), evitar quedarse sin créditos cambiando de modelo automáticamente (OmniRoute), optimizar el uso de tokens filtrando contexto irrelevante (Headroom), mantener memoria persistente del proyecto entre sesiones, y mejorar la calidad visual de los diseños generados (Front Design).

**Herramientas o skills de IA/código que menciona:** Sí menciona herramientas concretas: Playwright (para que Claude "vea" la pantalla), OmniRoute (cambio automático de modelo al llegar al límite), Headroom (filtrado de contexto/tokens), un plugin de memoria persistente tipo "palacio mental" (nombre exacto no aclarado en el audio), y Front Design (mejora de diseño visual con Claude).

**Cómo aplicarlo:** Si se usa Claude Code regularmente, evaluar instalar: Playwright para darle capacidad de ver la pantalla/navegador durante tareas de desarrollo; un gestor de modelos tipo OmniRoute para no perder trabajo al llegar a límites de uso; un plugin tipo Headroom para reducir el consumo de tokens filtrando contexto irrelevante; un sistema de memoria persistente por proyecto para no repetir contexto en cada sesión nueva; y Front Design (o una skill equivalente) para que los diseños generados por IA se vean más profesionales y menos genéricos.

---

### 28.
## Ugoki AI — https://www.instagram.com/p/De-LCYaRcC_/

**Caption:** Want to learn AI-powered motion design? DM us UGOKI and we'll send you the link 🔥 #claude #motiondesign

**Transcripción:** Si una animación se ve robótica, el problema suele ser su velocidad: en el mundo real nada se mueve a velocidad constante. Reglas de easing: para todo lo que entra en pantalla, usar "ease out" (llega rápido y luego frena de forma progresiva, como si lo depositara una mano firme). Para todo lo que sale de pantalla, lo opuesto, "ease in" (empieza lento y luego acelera). Para elementos de interfaz, usar un efecto "spring" (resorte): se pasa levemente de su posición final y luego se asienta. Se sugiere decirle esto a Claude textualmente para mejorar el nivel de las animaciones.

**Qué dice / enseña:** Enseña principios básicos de animación (easing) aplicados a motion design con IA: usar ease-out para elementos que entran, ease-in para elementos que salen, y un efecto spring para elementos de interfaz, en lugar de movimiento a velocidad constante (que se ve robótico).

**Herramientas o skills de IA/código que menciona:** Menciona a Claude como el agente al que se le puede pedir directamente estos efectos de animación (ease-in, ease-out, spring) para mejorar el resultado, aunque no nombra un plugin o skill técnica concreta más allá de esos términos de animación.

**Cómo aplicarlo:** Al pedirle a Claude (o a cualquier herramienta de motion design/código) que genere una animación, especificar explícitamente el tipo de easing: "ease out" para elementos que entran a la pantalla, "ease in" para los que salen, y un efecto "spring" (con ligero overshoot) para elementos de interfaz, en vez de dejar que use velocidad lineal/constante por defecto.

---

### 29.
## Marc Cleroux — https://www.instagram.com/p/Def9pj5TWtA/

**Caption:** Number 14 is my favorite. 😂 What's yours? Comment STUDIO and I'll send you the waitlist 👇 Follow for more AI tips. #claude #claudeai #videoediting #motiongraphics #contentcreator

**Transcripción:** La transcripción de audio es mayormente una lista corta de palabras sueltas (nombres de efectos: orbit, couch wall, ui world, frame break, digital zoom, phone mock-up, checklist, headline wall, zoom through cut, chart grow, pullback reveal, green screen, paper cut, doodle boy, vertigo, cover story, glass type), probablemente nombres/etiquetas de los 26 efectos de video mostrados visualmente uno por uno, sin explicación hablada de cada uno. El creador dice que va a lanzar 26 efectos de video distintos generados con "cloud" (Claude) en los próximos días, aclara que la última vez que lo hizo "rompió internet", e invita a comentar "STUDIO" para anotarse en la waitlist.

**Qué dice / enseña:** Es un teaser/anuncio de un pack de 26 efectos de video generados con IA (Claude) para edición y motion graphics (ej. orbit, zoom digital, mockup de teléfono, reveal con pullback, etc.), más que una explicación paso a paso de cómo lograrlos.

**Herramientas o skills de IA/código que menciona:** Menciona a Claude (referido como "cloud") como la IA usada para generar los efectos de video, pero no explica el prompt o la skill técnica exacta usada para cada efecto — es un anuncio/teaser, no un tutorial.

**Cómo aplicarlo:** No hay un paso a paso aplicable directamente desde este reel; sirve como inspiración de nombres/tipos de efectos de motion graphics (ej. "pullback reveal", "digital zoom", "frame break") que se podrían intentar reproducir pidiéndole a Claude que genere ese efecto visual específico, aunque la técnica exacta no se detalla en el audio.

---

### 30.
## Juan Jimenez Sieber — https://www.instagram.com/p/DeuyCGQO-dO/

**Caption:** 4 señales OBVIAS de que tu app fue hecha con IA, y cómo arreglarlas.

**Transcripción:** 4 señales obvias de que una app fue "vibecodeada" y cómo arreglarlas: 1) El copy/texto de marketing fue escrito por IA (frases tipo "no es esto pero lo otro" delatan esto); solución: escribir el copy uno mismo, usando la IA solo para pulir ideas propias, no para generarlo todo. 2) La interfaz usa morado y azul (o dos colores fuertes en degradé), porque toda la IA tiende a usar la misma combinación por defecto. 3) Falta un favicon personalizado (el ícono pequeño en la pestaña del navegador); solución: pedirle a la IA que genere uno personalizado, por ejemplo basado en el logo propio. 4) Mal manejo de los estados de carga (loading states): nada se carga visualmente o se usa un spinner infinito sin feedback; solución: pedirle al agente que use "Skeleton Loaders" (estados de carga bonitos) en vez de dejar una pantalla en blanco o un spinner que no da información.

**Qué dice / enseña:** Enseña a detectar y corregir 4 señales típicas de que una app fue hecha con IA/vibecoding: copy genérico escrito por IA, paleta de colores morado/azul por defecto, falta de favicon personalizado, y mal manejo de estados de carga (loading).

**Herramientas o skills de IA/código que menciona:** Menciona el concepto de "Skeleton Loaders" como solución técnica para los estados de carga, y sugiere pedirle a la IA/agente que genere un favicon personalizado; no nombra un plugin o herramienta específica más allá de estos conceptos genéricos aplicables con cualquier agente de código.

**Cómo aplicarlo:** Al revisar una app propia hecha con IA: escribir el copy de marketing uno mismo (usando la IA solo para mejorar redacción, no para generarlo entero), evitar o personalizar la paleta de colores morado/azul por defecto, agregar un favicon personalizado (basado en el logo propio), y reemplazar spinners infinitos o pantallas en blanco por Skeleton Loaders durante los estados de carga.

---

### 31.
## Alex Yates — https://www.instagram.com/p/DcNc-EszHJF/

**Caption:** 20 essential website security checks (give this list to Claude). If you vibecoded your website and don't have technical experience, you need to make sure you check all of these things. #vibecoding #vibecode

**Transcripción:** Lista de 20 chequeos de seguridad para un sitio "vibecodeado": ocultar las API keys, revisar las variables de entorno, revisar el historial de Git por claves expuestas, proteger las rutas de admin, agregar autenticación, revisar permisos de usuario, sanitizar el input del usuario, protegerse contra XSS, protegerse contra inyección SQL, revisar las reglas de la base de datos, agregar rate limiting, poner un tope de gasto (spend cap), asegurar la subida de archivos, agregar protección CSRF, revisar la configuración de CORS, habilitar HTTPS, agregar headers de seguridad, asegurar las cookies, deshabilitar el modo debug, y revisar la configuración de producción.

**Qué dice / enseña:** Da un checklist completo de 20 puntos de seguridad básica para cualquier sitio web, especialmente dirigido a quienes lo construyeron con IA/vibecoding sin experiencia técnica: desde manejo de secretos (API keys, variables de entorno) hasta protecciones estándar (XSS, SQL injection, CSRF, CORS, rate limiting, HTTPS, headers de seguridad, cookies seguras) y configuración de producción.

**Herramientas o skills de IA/código que menciona:** No menciona una herramienta o skill de IA específica; sugiere literalmente darle esta lista de 20 puntos a Claude para que la revise y aplique sobre el proyecto.

**Cómo aplicarlo:** Tomar este checklist de 20 puntos y pasárselo directamente a un agente de IA (ej. Claude) sobre el código del proyecto propio, pidiéndole que verifique y corrija cada ítem: ocultar claves y revisar el historial de git, proteger rutas de admin con autenticación y permisos adecuados, sanitizar inputs y protegerse contra XSS/SQL injection/CSRF, configurar rate limiting y tope de gasto, asegurar subida de archivos y cookies, revisar CORS, habilitar HTTPS y headers de seguridad, y deshabilitar modo debug en producción.

---

### 32.
## Vibe Coder — https://www.instagram.com/p/Deug6pAOzo4/

**Caption:** Claude deleted your customer data. What now? #vibecoding #claudecode #ai

**Transcripción:** Le piden a Claude que agregue un programa de referidos; Claude escribe código, actualiza el schema y corre la migración en producción — y borra la base de datos de producción con los 12,000 clientes. La solución: los ingenieros reales usan tres redes de seguridad. (1) Migrations: cada cambio de base de datos es un archivo chico y revisado que corre primero en staging antes de tocar producción. (2) Backups: el hosting puede sacar snapshot diario de toda la base; hay que activarlo y probar un restore (un backup no probado "es solo una esperanza"). (3) Rollbacks: cada migration viene con un "down step" para revertir el cambio malo, y el backup trae los datos de vuelta. Al final le piden a Claude: "backup primero, escribí una migration reversible y probala en staging" — resultado: backupeado, probado en staging, shippeado a prod, nada perdido.

**Qué dice / enseña:** Buenas prácticas de ingeniería al usar agentes de IA (Claude Code) para tocar bases de datos en producción: nunca dejar que el agente corra migraciones directo en prod sin red de seguridad. Enfatiza 3 controles concretos: migrations versionadas + testeadas en staging, backups con restore probado, y rollbacks (down migrations).

**Herramientas o skills de IA/código que menciona:** Claude Code (vibe coding) como agente que escribe y ejecuta migraciones de base de datos; no menciona un comando o skill instalable específico, es una práctica/flujo de trabajo (migration + backup + rollback) a aplicar al dar instrucciones al agente.

**Cómo aplicarlo:** Cuando le pidamos a Claude Code o cualquier agente que modifique esquemas o datos en producción, pedirle explícitamente: escribir la migration como archivo versionado, probarla primero en staging, confirmar que existe un backup reciente con restore testeado, e incluir siempre el paso de rollback/down-migration antes de aplicar en prod.

---

### 33.
## Sebastián Rivera — https://www.instagram.com/p/De5GRuOFWdK/

**Caption:** COMENTA IA ⤵️ y te envío el repositorio. ¿Pagas cada mes por una app? Replica son 11 skills gratis para Claude: una desmonta la app, otra la reconstruye, otra la prueba hasta romperla y otra le pone nota. La que cambia todo es la skill Emprendedor: lee reseñas reales de la original y arregla en la tuya lo que la gente odia. Ojo: copia lo que la app hace, no lo que tiene (ni su código, ni su logo, ni su contenido). #ia #inteligenciaartificial #claudecode #vibecoding #claude

**Transcripción:** Presenta "Réplica", un set de 11 skills gratis para Claude (Claude Code) pensado para reconstruir cualquier app de pago. Cada skill hace un trabajo: una estudia la app original por fuera (pantallas, botones, flujo de uso), otra la construye pieza por pieza, otra la prueba hasta romperla y registra cada fallo, y otra la compara contra la original y le pone nota/puntaje. La skill clave es la "Emprendedora": lee las reseñas reales de la app original (lo que la gente odia o le falta) y lo arregla en la versión propia, dando una ventaja competitiva real. Aclara que se debe copiar lo que la app *hace*, nunca su nombre, logo ni código, y que antes de publicar obliga a poner marca propia. Instalación: pegar el enlace del repo en Claude y escribir "Instala la Skill".

**Qué dice / enseña:** Cómo usar un conjunto de skills de Claude Code para hacer "reverse engineering" de producto: analizar una app de la competencia, reconstruirla, testearla automáticamente, compararla con el original, y mejorarla en base a reseñas reales de usuarios insatisfechos — todo antes de lanzar tu propia versión con marca propia.

**Herramientas o skills de IA/código que menciona:** "Réplica", un paquete de 11 skills para Claude/Claude Code (incluye al menos: skill de análisis/desmontaje de apps, skill de construcción, skill de testing/QA, skill de comparación/scoring, y skill "Emprendedor" de análisis de reseñas). Se instala pegando el link del repo en Claude y escribiendo "Instala la Skill".

**Cómo aplicarlo:** Si queremos clonar/mejorar una app de la competencia (o una herramienta SaaS que pagamos), conseguir el repo de "Réplica" (comentando "IA" en el post o buscando el link) e instalarlo como skill de Claude Code para automatizar: análisis de la competencia → reconstrucción → testing → comparación con reseñas reales → relanzamiento con marca propia, respetando no copiar nombre/logo/código.

---

### 34.
## Motion Ui Interface — https://www.instagram.com/p/De4B0UxPXIk/

**Caption:** Six details you feel but never see. iPhone doesn't feel smooth by accident. 01 Press feedback — moves the moment you touch, 0 ms, not 120 ms. 02 Springs — damping 0.8, a 1.5% overshoot, then it settles. 03 Momentum — a flick glides 1000 px after your finger lifts. 04 Rubber band — a 200 px pull stretches 86 px, then snaps back. 05 Interruptible — turns around mid-move, no 180 ms wait. 06 Continuous corners — the curve ramps in, no jump. #uidesign #uxdesign #productdesign #designsystem #uiux

**Transcripción:** Explica 6 detalles invisibles de microinteracción que hacen que iOS se sienta fluido: (1) Press feedback: el botón debe reaccionar en el instante del touch (0 ms), no al soltar (evitar delay de ~120ms). (2) Springs: animar con resortes (spring physics) en vez de timers lineales — ejemplo: rápido al inicio, overshoot de 1.5%, luego asienta, para que se sienta "real". (3) Momentum: un flick/swipe rápido debe seguir deslizando por inercia (hasta ~1000px) tras soltar el dedo, desacelerando gradualmente, en vez de detenerse en seco. (4) Rubber band: al hacer scroll más allá del límite (pull to refresh, por ej.), la lista debe "estirarse" (ej. 200px de pull = 86px de stretch) y rebotar, para indicar que se llegó al borde. (5) Interruptible motion: cualquier animación (ej. un panel abriéndose) debe poder revertirse a mitad de camino sin esperar que termine (nada de esperar 180ms a que acabe antes de reaccionar al siguiente input). (6) Continuous corners (squircles): las esquinas redondeadas deben tener una curva continua que entra gradualmente, no un empalme abrupto entre línea recta y círculo.

**Qué dice / enseña:** Principios de microinteracción y animación de UI/UX que hacen que una interfaz (como iOS) se perciba "premium" y fluida, aunque el usuario no pueda nombrar por qué. Son reglas de diseño de interacción, no código específico.

**Herramientas o skills de IA/código que menciona:** Ninguna skill de IA ni herramienta específica — es una explicación de principios de diseño de animación/UX (press feedback, springs, momentum, rubber band, interruptible motion, continuous corners), aplicables luego con cualquier motor de animación (ej. CSS/Framer Motion/SwiftUI springs, etc.) pero no se nombra ninguna herramienta concreta.

**Cómo aplicarlo:** Al diseñar o implementar interfaces (web o apps), usar estos 6 principios como checklist de calidad: dar feedback visual inmediato al touch/click, animar con springs en vez de ease lineales fijos, dejar que los gestos tengan inercia/momentum, mostrar "rubber band" en los límites de scroll, hacer que toda animación sea interrumpible, y usar esquinas con curvatura continua (squircle) en botones/cards para que la UI se sienta más pulida.

---

### 35.
## Viewcci | Short-Form Tips — https://www.instagram.com/p/DcwlTN3uitC/

**Caption:** Comment "SFX" and I'll send you the whole pack. Seven sound effects and exactly where each one goes. Most people either use none of these or dump all seven into one video. Pick two or three and use them the same way every time. That's what makes it sound like a choice instead of an accident. #contentcreator #videoediting #marketing #hooks #edits

**Transcripción:** Lista 7 efectos de sonido y dónde usar cada uno en la edición de video de formato corto: uno para los hooks, otro para los "reveals", otro para las transiciones, otro para las captions (subtítulos), otro cuando aparece texto en pantalla ("pop up"), otro para hacer zoom in, y otro para los llamados a la acción (CTA).

**Qué dice / enseña:** Técnica de edición de video (sound design) para contenido de formato corto: asignar un efecto de sonido específico y consistente a cada tipo de momento del video (hook, reveal, transición, caption, text pop, zoom, CTA), en vez de usar ninguno o saturar el video con todos a la vez. La consistencia en el uso (elegir 2-3 y repetirlos siempre igual) es lo que da sensación de intencionalidad.

**Herramientas o skills de IA/código que menciona:** Ninguna — es una técnica manual de edición de video/sound design, sin IA ni herramienta de código.

**Cómo aplicarlo:** Al editar reels o videos cortos (de marketing, producto, etc.), elegir 2-3 efectos de sonido fijos y usarlos siempre para las mismas funciones (ej. un "swoosh" para transiciones, un "ding" para reveals, un "pop" para texto en pantalla) en vez de improvisar o no usar ninguno — mejora la percepción de calidad y ritmo del contenido.

---

### 36.
## Ekko Amaryllis — https://www.instagram.com/p/DbomiqVtUI5/

**Caption:** also 90% of the time captions don't really matter #content #hooks #viralhooks #contentskills #creator

**Transcripción:** Análisis/crítica de varios hooks (primeros frames) de videos virales, comparando por qué funcionan o no: (1) Un hook "terrible" que solo funciona por el atractivo físico de la persona y porque la cuenta ya tiene 2M de seguidores. (2) Un hook "amazing" que es masterclass en omitir contexto para que lo que pasa parezca más loco de lo que realmente es (ej. un clavado sin mostrar que falló primero haría que 10x más gente lo vea si se empieza por el fallo). (3) Un hook con dos "pattern interrupts" (una persona caminando por un río con una cámara cara en el centro) que genera curiosidad y, sumado a un caption intrigante, genera confianza de que van a mostrar algo bueno. (4) Un hook que "tarda demasiado" en mostrar algo interesante, por lo que la gente scrollea aunque el concepto del video sea bueno. (5) Un hook con buen contraste respecto al anterior: a punto de golpear la pelota, genera anticipación junto con el título, antes de revelar el chiste.

**Qué dice / enseña:** Principios de qué hace que el primer frame/los primeros segundos de un video (el "hook") retenga o pierda espectadores: omitir contexto para generar intriga, usar "pattern interrupts" (elementos inesperados) para generar curiosidad, evitar hooks lentos que no muestran nada interesante de entrada, y usar contraste entre hooks consecutivos. También señala que los captions (subtítulos de texto) no son lo que más importa el 90% del tiempo — lo que importa es el frame/concepto inicial.

**Herramientas o skills de IA/código que menciona:** Ninguna skill de IA/código — es análisis de copywriting/storytelling visual para contenido corto, 100% manual.

**Cómo aplicarlo:** Al elegir el frame/clip inicial de un reel o video corto, priorizar el que genere más curiosidad por lo que *no* se ve (omitir contexto, mostrar algo ambiguo o un "pattern interrupt") en vez de mostrar todo de entrada; no perder tiempo en pulir captions pensando que son la clave de la retención — enfocar el esfuerzo en los primeros 1-3 segundos de imagen.

---

### 37.
## Vibe Coder — https://www.instagram.com/p/Dewnsm0uks1/

**Caption:** How do you prevent duplicate payments even if someone clicks "pay" twice? #claudecode #coding #ai #vibecoding

**Transcripción:** Un cliente fue cobrado dos veces por la misma compra tras hacer doble click en "comprar" (dos clicks, dos cargos). Explica que deshabilitar el botón no alcanza porque los reintentos de red también pueden duplicar el cargo. La solución real: hacer el checkout idempotente con 3 pasos. (1) Idempotency key: al abrir el checkout, la app genera un ID único para esa compra y lo manda con cada click. (2) El servidor revisa esa key: si es nueva, cobra la tarjeta y guarda el recibo; si ya la vio antes, salta el cobro y devuelve el mismo recibo. (3) Pasar esa misma key a Stripe, así hasta un reintento de red cobra una sola vez; además, reembolsar cualquier cargo duplicado que ya haya ocurrido. Al final le piden a Claude: "agregá una idempotency key al checkout y reembolsá el cargo duplicado" — resultado: key agregada, duplicado reembolsado, cinco clicks, un solo cobro.

**Qué dice / enseña:** Patrón de ingeniería para evitar cobros duplicados en sistemas de pago: idempotencia en el checkout usando una "idempotency key" única por intento de compra, validada tanto en el backend propio como pasada al proveedor de pagos (Stripe), más reembolso automático de duplicados detectados.

**Herramientas o skills de IA/código que menciona:** Claude Code (vibe coding) como agente al que se le pide implementar la idempotency key en el checkout; menciona Stripe como proveedor de pagos. No es una skill instalable específica, sino un patrón de implementación a pedirle al agente.

**Cómo aplicarlo:** Si tenemos un flujo de checkout/pago (propio o integrado con Stripe u otro gateway), pedirle a Claude Code que implemente una idempotency key generada en el cliente al abrir el checkout, validada en el servidor antes de cobrar, y pasada también al proveedor de pagos, para que ni dobles clicks ni reintentos de red generen cobros duplicados.

---

### 38.
## Edgar Romero — https://www.instagram.com/p/De4NlF9BL6W/

**Caption:** Comenta PLANTILLA 👇

**Transcripción:** Presenta una estructura de guion para retención: Hook, Super Hook, Open Loop, Body 1, Rehook 1, Body 2, Rehook 2, Body 3 y CTA. Explica cada etapa: el Hook debe ir acompañado de imágenes, sonidos y palabras que solo el cliente ideal identifique. El Super Hook añade contexto y una razón para seguir escuchando (usando credibilidad propia o ajena). El Open Loop deja una pregunta abierta para más adelante (como hizo el propio autor al prometer explicar cómo reducir la tasa de salida). Cada Body desarrolla una idea, idealmente contada de forma única que el seguidor nunca haya escuchado. Cada Rehook renueva la curiosidad para seguir viendo. Dice haber analizado más de 250 videos virales de nicho con esta estructura y armó una plantilla para convertir ideas en guiones con mayor probabilidad de retención (ofrece enviarla si comentan "plantilla"). Sobre cómo reducir la tasa de salida: si muchas personas abandonan en los primeros segundos, es porque no se está hablando de un problema concreto que el cliente ideal esté atravesando en ese momento — hay que describir ese problema mejor de lo que la propia audiencia podría describirlo, combinado con esta estructura.

**Qué dice / enseña:** Framework de guion (script) para videos de retención: una secuencia de 9 bloques (Hook, Super Hook, Open Loop, Body 1-3, Rehook 1-2, CTA) pensada para mantener a la audiencia viendo hasta el final, más el principio de que la retención depende de hablar de un problema específico del cliente ideal mejor de lo que él mismo lo describiría.

**Herramientas o skills de IA/código que menciona:** Ninguna skill de IA/código — es una plantilla/framework de copywriting y guionismo manual, sin herramientas técnicas.

**Cómo aplicarlo:** Al escribir guiones para reels o videos cortos, estructurarlos siguiendo Hook → Super Hook → Open Loop → Body 1 → Rehook 1 → Body 2 → Rehook 2 → Body 3 → CTA, asegurando que el Hook esté hiper-dirigido al cliente ideal (palabras/imágenes/sonidos específicos de su situación) y que el tema central hable de un dolor concreto de esa audiencia, descrito con más precisión de la que ellos mismos usarían.

---

### 39.
## Gin Lee — https://www.instagram.com/p/De0mgVbtXE-/

**Caption:** How should creators write their script?

**Transcripción:** Explica por qué la mayoría de los guiones de video suenan aburridos: falta de ritmo, porque todas las oraciones son largas. La solución: intercalar oraciones cortas de no más de cinco palabras entre las largas, creando un patrón "largo-corto-largo-corto" que le da ritmo más interesante al guion. Muestra un ejemplo antes/después: "Is it possible to study for 24 hours in a public library? Let's find out. I first have to find the local library that opens for 24 hours. But there was a problem." — se nota el patrón de oraciones largas seguidas de frases cortas de corte ("Let's find out.", "But there was a problem."). Menciona que la idea está inspirada en un creador llamado "Callaway".

**Qué dice / enseña:** Técnica de escritura de guiones para contenido de video: alternar oraciones largas con oraciones muy cortas (máximo 5 palabras) para generar ritmo narrativo y evitar que el guion se sienta monótono/aburrido.

**Herramientas o skills de IA/código que menciona:** Ninguna — es una técnica de escritura/guionismo manual, sin IA ni herramienta de código.

**Cómo aplicarlo:** Al escribir guiones de reels o videos, revisar que no haya tramos largos de oraciones extensas seguidas; insertar frases cortas (3-5 palabras) entre ellas como "cortes" de ritmo, para que el guion se sienta más dinámico al leerse o narrarse en voz alta.

---

### 40.
## Aperture Motion™ — https://www.instagram.com/p/De167Hmhesj/

**Caption:** You just waited 20 seconds for a wrecking ball that never hit. That's the attention we build for businesses. Ads, explainers and launch videos, in any style, made to stop the scroll and keep people watching. DM "VIDEO" and tell us what your business does. We'll send you examples from your industry.

**Transcripción:** "You just watched a wrecking ball for seven seconds. A wrecking ball that was never there. And you're still watching, waiting for it to hit. Now imagine that was your business. That's what we make. Videos people don't scroll past." Es el propio video demostrando su punto: genera una expectativa visual (una bola de demolición a punto de golpear) que nunca se resuelve, manteniendo al espectador mirando por la intriga/tensión, y luego usa eso como argumento de venta de su servicio de producción de video.

**Qué dice / enseña:** Es un anuncio/pitch de servicios de producción de video (ads, explainers, videos de lanzamiento) de un estudio ("Aperture Motion"). La enseñanza de fondo es una técnica de retención: crear una expectativa visual fuerte y no resolverla de inmediato (tensión sin resolución) para que la audiencia siga mirando, usada aquí como demo meta del propio servicio que venden.

**Herramientas o skills de IA/código que menciona:** Ninguna skill de IA/código — es un video promocional de servicios de producción audiovisual humana, sin mencionar herramientas técnicas.

**Cómo aplicarlo:** Como técnica de retención, usar en nuestros propios videos una "tensión sin resolver" (crear expectativa de que algo va a pasar y demorar o evitar resolverla) para mantener la atención; como ejemplo de formato de anuncio, notar cómo el video vende el servicio demostrando la técnica en sí mismo en vez de solo describirla.

---

### 41.
## Think Macro | Systems for Scale — https://www.instagram.com/p/DezCrecDDSm/

**Caption:** You're paying for software that has a free twin on GitHub. Here are nine. 1. Open Higgsfield replaces Higgsfield (bring your own API key). 2. VoiceStudio replaces ElevenLabs, on your own machine. 3. OpenSEO replaces Semrush. 4. WeKnora replaces Notion AI, on local models. 5. OpenWhispr replaces Wispr Flow. 6. OpenProject replaces Asana. 7. Cal.com replaces Calendly. 8. Chatwoot replaces Intercom. 9. Cap replaces Loom. Paying for four or five of these? That's money back every month. App not on the list? Reverse Engineer Anything rebuilds it with Claude Code. Comment REPO and I'll DM you all nine links.

**Transcripción:** Lista 9 repos de GitHub gratuitos/open-source que reemplazan software de pago: (1) OpenHiggsfield reemplaza Higgsfield. (2) VoiceStudio reemplaza ElevenLabs, corriendo en tu propia máquina. (3) OpenSEO reemplaza SEMrush (rank tracking, backlinks, auditorías de sitio). (4) WeKnora reemplaza Notion AI, con modelos locales. (5) OpenWhispr reemplaza Wispr Flow (dictado por voz en cualquier app, online u offline). (6) OpenProject reemplaza Asana ("el Asana killer"). (7) Cal.com reemplaza Calendly, con sync de Google y Outlook. (8) Chatwoot reemplaza Intercom (todos los mensajes de leads/clientes en un solo inbox). (9) Cap reemplaza Loom. Cierra diciendo que si pagás por 4 o 5 de estas herramientas, cambiar a las alternativas gratis es plata de vuelta cada mes, y que si hay una app favorita que no está en la lista, "Reverse Engineer Anything" la reconstruye con Claude Code.

**Qué dice / enseña:** Catálogo de alternativas open-source/self-hosted a herramientas SaaS de pago comunes (generación de imagen/video IA, voz/TTS, SEO, notas con IA, dictado por voz, gestión de proyectos, scheduling, soporte al cliente, grabación de pantalla), para reducir costos de software corriendo versiones gratuitas (algunas localmente).

**Herramientas o skills de IA/código que menciona:** Nombra 9 repos de GitHub concretos: OpenHiggsfield, VoiceStudio, OpenSEO, WeKnora, OpenWhispr, OpenProject, Cal.com, Chatwoot y Cap. Además menciona "Reverse Engineer Anything", un enfoque/herramienta para reconstruir cualquier app de pago usando Claude Code.

**Cómo aplicarlo:** Revisar qué de estas 9 herramientas de pago usamos hoy (ElevenLabs, SEMrush, Notion AI, Wispr Flow, Asana, Calendly, Intercom, Loom, Higgsfield) y evaluar migrar a su alternativa gratuita/open-source listada para bajar costos mensuales; si usamos una app de pago que no está en la lista, considerar el enfoque "Reverse Engineer Anything" con Claude Code para reconstruirla.

---

### 42.
## Robin TEMPE — https://www.instagram.com/p/De1_SdZt527/

**Caption:** Save this before you write your next script. The perfect structure for short-form content, in 8 blocks: Hook → Lead → Body → Open loop → Body → Open loop → Body → CTA. El hook rompe el patrón del scroll; el lead ancla hasta el segundo 10; Body 1 es el primer valor; un open loop es una línea que genera curiosidad ("pero eso no es lo más loco"); se repite dos veces y se cierra con un último body; el CTA mueve a los espectadores más interesados al siguiente paso del funnel.

**Transcripción:** Hook, Lead, Body, Open Loop, Body, Open Loop, Body, CTA — esta es la estructura perfecta para contenido short-form. El hook rompe el patrón del scroll. El lead ancla al espectador hasta el segundo 10, una vez ahí ya no se va a seguir scrolleando. Luego Body 1, el primer valor entregado. Después un open loop: una línea que genera curiosidad tipo "pero eso no es lo más loco", para que se quede a cerrarlo. Se repite esa estructura dos veces, y después un último body. Finalmente el CTA, que toma a los espectadores más "calientes" y los mueve al siguiente paso del funnel. Ocho bloques en total. Guardar esto antes de escribir el próximo script.

**Qué dice / enseña:** Framework de 8 bloques para estructurar guiones de contenido corto (reels/shorts) que maximiza retención y conversión: Hook → Lead → Body → Open loop → Body → Open loop → Body → CTA.

**Herramientas/skills de IA/código que menciona:** Ninguna — es un framework de copywriting/guionado, no menciona ninguna herramienta de IA o código.

**Cómo aplicarlo:** Usar esta estructura de 8 bloques como plantilla al escribir el guion de reels/videos propios (por ejemplo para contenido de marketing o dev): empezar con un hook que rompa el patrón, un lead que ancle la atención, alternar bloques de valor con "open loops" que generen curiosidad, y cerrar con un CTA claro hacia el siguiente paso del funnel.

---

### 43.
## Manuel — https://www.instagram.com/p/DdFdFiavMJ0/

**Caption:** If you wanna go viral you need to learn how to speak! Es algo simple pero hace una gran diferencia. Ayuda a creadores y negocios a crecer en redes con tips como este. Ofrece ayuda personal (de él y su equipo) para hacer crecer la marca vía link en bio.

**Transcripción:** Si querés volverte viral, necesitás aprender a hablar.

**Qué dice / enseña:** Mensaje muy breve (casi un hook sin desarrollo visible en este clip) que plantea que saber "hablar" (oratoria/presencia en cámara) es clave para volverse viral en redes. No desarrolla técnica concreta en el audio capturado.

**Herramientas/skills de IA/código que menciona:** Ninguna — no menciona ninguna herramienta de IA o código.

**Cómo aplicarlo:** Como recordatorio genérico de que la forma de hablar/presentar en cámara importa tanto como el contenido al grabar reels propios; no aporta un método concreto más allá de eso.

---

### 44.
## Gurnoor Singh — https://www.instagram.com/p/De2yrjHT3Wu/

**Caption:** Why is nobody copying this guy's videos 😂

**Transcripción:** Si hacés contenido para ecommerce, este es un formato de anuncio muy subestimado hoy en día: buscar en Instagram a "Zach D Films" y analizar los scripts que usa en sus videos. En vez de tener un hook loco, arranca directo al video sin hook ("toma una lata caliente y presiónala contra el frente del bombo", por ejemplo) y aun así consigue millones de views, porque la gente ya está familiarizada con ese estilo de video, entonces el anuncio se mezcla con lo que la gente ya está mirando. La ventaja es que podés tomar como 10 videos de este tipo de creador, pasárselos a Gemini para sacar la transcripción, y después pasarle eso a Claude para que te ayude a escribir un anuncio parecido usando IA.

**Qué dice / enseña:** Estrategia de ads para ecommerce: copiar el formato de creadores virales que van "directo al grano" sin hook tradicional, porque la familiaridad del formato hace que el anuncio se mezcle con el contenido orgánico que la gente ya consume (blending).

**Herramientas/skills de IA/código que menciona:** Gemini (para transcribir/analizar videos de referencia) y Claude (para escribir el guion del anuncio a partir de esas transcripciones). No da comandos específicos, es un flujo conceptual: transcribir con Gemini → redactar con Claude.

**Cómo aplicarlo:** Para crear anuncios o contenido de producto: elegir un creador/formato viral de referencia, juntar varios de sus videos, pedirle a Gemini (o cualquier modelo con capacidad de video/transcripción) que saque el guion, y luego pasarle esas transcripciones a Claude para generar un guion de anuncio propio que imite esa estructura "sin hook" pero manteniendo el estilo que la audiencia ya reconoce.

---

### 45.
## Michael Quoc Ly — https://www.instagram.com/p/DdU5LzzvWyW/

**Caption:** Don't want your vibecoded app to get into legal trouble? Tell Claude to do these things. #ai #claude #buildinpublic #vibecoding #app

**Transcripción:** Lista de pedidos para hacerle a Claude en una app "vibecoded" para evitar problemas legales: agregar privacy policy, terms of service, refund policy, cookie policy y banner de consentimiento de cookies; revisar los consentimientos de formularios; no recolectar datos innecesarios; auditar los SDKs de terceros; eliminar dark patterns, cargos ocultos, reseñas falsas y claims no soportados; agregar alt text de accesibilidad; corregir el ratio de contraste de colores; agregar navegación por teclado; agregar los datos del negocio; pedir consentimiento de edad si se recolectan datos de menores; agregar link de unsubscribe en emails; licenciar fuentes e imágenes usadas; y agregar opción de solicitud de borrado de datos.

**Qué dice / enseña:** Checklist de 20 ítems legales/de cumplimiento (privacidad, términos, accesibilidad, consentimiento, licencias) que conviene pedirle a una IA que agregue a una app "vibecoded" (hecha mayormente con IA) antes de publicarla, para reducir riesgo legal.

**Herramientas/skills de IA/código que menciona:** Claude, como el asistente al que se le pide implementar estos features/políticas en el código de la app. No da comandos específicos ni skills instalables, es una lista de instrucciones en lenguaje natural para dárselas a Claude.

**Cómo aplicarlo:** Antes de lanzar una app o sitio hecho con IA (vibecoding), copiar esta lista como prompt/checklist y pedirle a Claude que agregue cada uno de estos puntos (privacy policy, cookie consent, SDKs de terceros auditados, accesibilidad, licencias de assets, etc.) para reducir exposición legal.

---

### 46.
## Mohamed BOUHEZZA | Software Engineering — https://www.instagram.com/p/De2GwbRjCo8/

**Caption:** Session vs JWT

**Transcripción:** Baneás a un scammer de tu app: cuenta borrada, listo. 10 minutos después sigue comprando cosas con una tarjeta que no es suya, en una cuenta que ya no existe. ¿Cómo? Porque tu app usa JWT y nadie te avisó la trampa. Cuando alguien inicia sesión, el server puede hacer una de dos cosas: Opción 1, una sesión: el server le da al browser un ID random (como un ticket de guardarropa) y lo guarda en la base de datos; en cada click chequea si el ticket sigue siendo válido; si borrás el ticket, el usuario queda afuera instantáneamente. Opción 2, un JWT: el server le da un pase firmado que dice quién es y cuándo expira; no se puede editar porque la firma se rompe; en cada click el server solo chequea la firma y la fecha, sin ir a la base de datos, por eso es rápido — pero esa es la trampa: el pase vive en la laptop del usuario, no en tu base de datos, así que borrar la cuenta no cambia nada porque el server nunca vuelve a mirar, y si el JWT expira en 30 días, tiene 30 días de margen. ¿Cómo lo resuelven los profesionales? Haciendo el JWT corto, de 5 minutos, y al login dando un segundo token: un refresh token, que sí va a la base de datos. Cada 5 minutos la app cambia el refresh token por un JWT fresco, y esa es la única vez que se consulta la base de datos. Para banear a alguien: borrás su refresh token, y 5 minutos después queda bloqueado para siempre. Rápido como JWT, revocable como una sesión. Pregunta final: ¿tu app usa Session o JWT?

**Qué dice / enseña:** Explica la diferencia práctica entre autenticación por Sessions y por JWT, y el problema real de JWT (no se puede revocar hasta que expira) ilustrado con el caso de un usuario baneado que sigue operando. Propone el patrón estándar de la industria para solucionarlo: JWT de vida corta (ej. 5 min) + refresh token guardado en base de datos, que sí es revocable.

**Herramientas/skills de IA/código que menciona:** Ninguna skill de IA — es contenido de educación en backend/seguridad (conceptos de autenticación: sessions, JWT, refresh tokens), no menciona herramientas ni comandos específicos.

**Cómo aplicarlo:** Si una app propia usa JWT puro, considerar migrar al patrón access token corto (ej. 5 min) + refresh token persistido en base de datos, para poder revocar accesos (banear usuarios) de forma inmediata sin perder la velocidad de JWT en cada request.

---

### 47.
## Pradj — https://www.instagram.com/p/DetUdfLCZdC/

**Caption:** Jensen Huang x Nvidia. Before vs after, edited with AI. Same footage, a completely different feel once Claude helped with the edit. El autor hizo las decisiones creativas y la IA hizo el trabajo pesado de edición. Pide seguir la cuenta para un tutorial de cómo se hizo.

**Transcripción:** Fragmento de una entrevista a Jensen Huang (CEO de Nvidia): si tuviera que elegir entre dos recién graduados para contratar, uno sin idea de IA y otro experto en usar IA, contrataría al experto en IA — ya sea contador, marketing, supply chain, atención al cliente, ventas, business development o abogado. Por eso recomienda que todo estudiante que se gradúe sea experto en IA, y lo mismo para cualquier oficio (carpintero, electricista): ir a usar IA y ver qué puede transformar en su trabajo actual para potenciarse. Si fuera agricultor, usaría IA para ver cómo revolucionar esa industria.

**Qué dice / enseña:** Dos cosas: (1) en el caption, que el video (antes/después de Jensen Huang) fue editado con ayuda de Claude, con las decisiones creativas a cargo del humano y la ejecución pesada delegada a la IA; (2) en el audio, el mensaje de Jensen Huang de que ser experto en IA es una ventaja competitiva clave para contratación y para cualquier profesión u oficio.

**Herramientas/skills de IA/código que menciona:** Claude, mencionado en el caption como la herramienta usada para la edición de video (no se detalla el método/prompt exacto; el autor ofrece el tutorial a cambio de seguir la cuenta).

**Cómo aplicarlo:** Tomar nota de que Claude puede usarse como asistente de edición de video (dirección creativa humana + ejecución por IA) para piezas tipo "before/after"; y usar el mensaje de Jensen Huang como argumento/ángulo de contenido sobre la importancia de volverse experto en IA en cualquier rubro.

---

### 48.
## Ben Broch | AI Saas builder — https://www.instagram.com/p/Dew5OaVgfmG/

**Caption:** Comment SKILLS and I'll send you all 320, ranked by GitHub stars, with the install command for each.

**Transcripción:** El audio del video es solo música de fondo, sin voz ni contenido hablado (la transcripción automática devolvió únicamente "Music"). El post se analiza solo por el caption/visual.

**Qué dice / enseña:** Es un hook tipo "lead magnet": promete enviar una lista de 320 "skills" (probablemente Claude Skills / plugins de agentes de IA) ordenadas por estrellas de GitHub, junto con el comando de instalación de cada una, a cambio de comentar "SKILLS". No desarrolla contenido técnico en el video mismo, es una captación de leads/engagement.

**Herramientas/skills de IA/código que menciona:** Menciona genéricamente "skills" con comando de instalación y ranking por GitHub stars, lo que sugiere un catálogo de Claude Skills o plugins similares, pero no da nombres concretos ni comandos en este post (se entregarían por fuera, al comentar).

**Cómo aplicarlo:** Como referencia de formato de "lead magnet" para contenido propio (prometer un recurso curado — ej. lista de skills/plugins — a cambio de un comentario); si se consigue la lista real de las 320 skills mencionada, podría ser útil como catálogo para descubrir skills de Claude/agentes ya probadas por la comunidad.

---

### 49.
## Shaan Johari — https://www.instagram.com/p/DeUsh56RPGH/

**Caption:** Comment STYLE and I'll send it to you

**Transcripción:** Hizo que Claude co-diseñara toda su marca personal. Primero le dice a Claude lo que quiere y Claude abre un artifact con la primera ronda de animaciones. Puede scrollear esas opciones y elegir las que le gustan o no, dejar notas de lo que quiere cambiar, o directamente descartar una si no le gusta nada. Es una buena forma de ver cómo va a quedar toda la identidad de marca, incluyendo gráficos, transiciones y hasta efectos de sonido. Una vez que termina de revisar, envía su feedback, que se usa para hacer otra revisión, y lo que queda definido se escribe como reglas para que Claude sepa exactamente qué quiere cada vez.

**Qué dice / enseña:** Flujo de trabajo para co-diseñar una identidad/marca personal (gráficos, transiciones, efectos de sonido) usando Claude y sus Artifacts: generar opciones, revisarlas e iterarlas con feedback puntual, y fijar las preferencias finales como "reglas" persistentes para que las próximas generaciones ya respeten ese estilo.

**Herramientas/skills de IA/código que menciona:** Claude, usando específicamente la función de Artifacts para mostrar y versionar las propuestas visuales/de animación, y un mecanismo de reglas persistentes (similar a instrucciones guardadas) que "recuerda" las preferencias de diseño aprobadas.

**Cómo aplicarlo:** Para definir un sistema de marca/estilo visual propio (ej. para reels, web o producto): pedirle a Claude que genere variaciones de identidad visual en un Artifact, revisarlas y dar feedback puntual por iteración, y una vez aprobado el estilo, pedirle que lo registre como reglas fijas para mantener consistencia en futuras piezas.

---

### 50.
## (no disponible) — https://www.instagram.com/p/DejblzhiHWU/

**Estado:** No se pudo acceder al contenido. `yt-dlp` devolvió el error: "Instagram sent an empty media response. Check if this post is accessible in your browser without being logged-in." Esto suele indicar que el post es privado, fue eliminado, o Instagram está bloqueando el acceso sin login para esa URL. No se descargó metadata ni audio, por lo que no hay caption ni transcripción disponibles.

**Caption:** No disponible (no se pudo descargar metadata).

**Transcripción:** No disponible (no se pudo descargar el post).

**Qué dice / enseña:** No se puede determinar sin acceso al post.

**Herramientas/skills de IA/código que menciona:** No se puede determinar.

**Cómo aplicarlo:** No aplica — habría que revisar manualmente el link desde una cuenta logueada en Instagram para confirmar si sigue disponible y, de ser así, volver a correr `process_reel.sh` sobre este id.

---

### 51.
## Alex Yates — https://www.instagram.com/p/DeLUE2kuMQw/

**Caption:** 20 features you can tell Claude to add to your vibecoded website right now! #vibecoding #vibecode

**Transcripción:** Lista de 20 features para pedirle a Claude que agregue a un sitio vibecoded: toggle de dark mode, banner simple de cookies, búsqueda full-site, botón de scroll back to top, menús mobile, animaciones de carga, hover states, barras de progreso de scroll, botones de copy to clipboard, hoja de estilo para impresión, headers sticky, link de skip to content, toggle de visibilidad de contraseña, tracking UTM, estado de éxito y de error en formularios, modales de confirmación, fechas de "last updated", secciones de FAQ expandibles y un botón flotante de contacto.

**Qué dice / enseña:** Checklist de 20 mejoras de UX/producto (no legales, a diferencia de la lista de @DdU5LzzvWyW) que se le pueden pedir directamente a Claude para pulir un sitio hecho con vibecoding: accesibilidad básica, estados de formularios, navegación, performance percibida y pequeños detalles de UI que suelen faltar en un primer MVP.

**Herramientas/skills de IA/código que menciona:** Claude, como el asistente al que se le pide implementar cada feature en el código del sitio. No da comandos específicos ni skills instalables, es una lista de instrucciones en lenguaje natural para prompt.

**Cómo aplicarlo:** Usar esta lista como checklist de pulido de UX al terminar la primera versión de un sitio/app hecho con IA: ir pidiéndole a Claude, feature por feature, que agregue dark mode, banner de cookies, búsqueda, estados de formulario, FAQ expandible, etc., antes de considerar el sitio "terminado".

---

### 52.
## Luke | Creative Strategist + ML — https://www.instagram.com/p/DfNBZLLA4sX/

**Caption:** 13 ad formats you can make for Facebook #metaads #paidads #adcreative #ecom

**Transcripción:** The baby drama ad, the green screen iPhone notes, the AI skeleton, the AI podcast, chalkboard explainer, AI history, cartoon, whiteboard explainer, AI ranting song, sticky notes, notebook page turning, black and white comic style and TED Talk.

**Qué dice / enseña:** Lista de 13 formatos/estilos de anuncio para Facebook/Meta Ads, pensados para e-commerce: drama con "bebé" como gancho, notas estilo iPhone con green screen, esqueleto generado con IA, podcast con IA, explicador tipo pizarrón, historia narrada por IA, estilo cartoon, explicador tipo whiteboard, canción "ranting" generada con IA, notas adhesivas, efecto de pasar páginas de cuaderno, estilo cómic en blanco y negro, y formato TED Talk.

**Herramientas o skills de IA/código que menciona:** No nombra herramientas específicas por nombre; varios formatos asumen uso de IA generativa de video/imagen/audio (AI skeleton, AI podcast, AI history, AI ranting song) pero sin especificar cuál.

**Cómo aplicarlo:** Catálogo de "ángulos creativos" para variar anuncios pagados de Meta sin rehacer el producto — rotar entre estos 13 formatos para testear qué hook/formato convierte mejor en una misma oferta.

---

### 53.
## Champ McCorkle | AI & Claude — https://www.instagram.com/p/DfXcY28peC5/

**Caption:** Claude can now watch YouTube videos for you and learn any skill 🧠. After 3,265 hours in Claude, this is by far the easiest way to make your AI smarter. Here's how to set it up in 30 seconds 👇 1️⃣ Paste the link into Claude. Tell it to install the skill. Now it can watch any video just like a human. 2️⃣ Drop in any YouTube video. Say: "Watch this, learn what it teaches, and turn it into a skill that I can use forever." 3️⃣ Do it with dozens at a time. You would watch one of these and forget the video by Friday. Claude can watch dozens at a time and keep every single one in its brain. Drop in the best sales training on YouTube and Claude will start writing your sales follow-ups that way. Drop in Hormozi's offer videos and it will start rewriting your quotes that way. YouTube is just the start. It can also listen to podcasts the exact same way. Comment LEARN and I'll send you the full skill and exact prompt to start doing this today.

**Transcripción:** Claude puede ahora ver videos de YouTube por vos y aprender cualquier skill. Se instala pasándole un link a Claude y diciéndole que instale el skill; después se le tira cualquier video de YouTube con el prompt "watch this, learn what it teaches, and turn it into a skill that I can use forever". A diferencia de una persona, Claude puede "ver" docenas de videos y quedarse con todo. Ejemplos: darle el mejor training de ventas de YouTube para que Claude escriba los follow-ups de ventas con ese estilo, o los videos de ofertas de Hormozi para que reescriba cotizaciones así. Aclara que esto también funciona con podcasts (audio), no solo YouTube.

**Qué dice / enseña:** Vende la idea de instalar un "skill" en Claude que le permite ver/analizar videos de YouTube (y podcasts) y extraer de ahí un método o estilo, para después aplicarlo a tareas propias (ej: escribir mensajes de ventas imitando un training, o cotizaciones imitando el estilo de Hormozi). El mecanismo real no se explica en el video — pide comentar "LEARN" para mandar por DM "el skill completo y el prompt exacto", es decir, el contenido técnico concreto no está en el reel.

**Herramientas/skills que menciona:** Claude (Anthropic) y su sistema de skills instalables; menciona que el mismo mecanismo serviría para procesar YouTube y podcasts. No se nombra ninguna skill específica de la galería pública ni cómo se instala realmente (eso lo manda por DM aparte).

**Cómo aplicarlo:** La idea de fondo (un skill que mira contenido de YouTube/podcasts y lo convierte en una skill reusable) es válida y aplicable: en la práctica hoy existe `youtube-downloader` (bajar video/audio) y se podría combinar con transcripción + un skill tipo "skill-creator" para que Claude escriba el método aprendido como skill nueva — pero el video en sí es más gancho de venta (pedir comentario para mandar el prompt) que un tutorial completo, así que no hay un prompt exacto citable desde este análisis.

---

### 54.
## Tonistelk | Viral AI Tutorials — https://www.instagram.com/p/DfenRsSIOqZ/

**Caption:** 10 Claude Animation Styles (To Go Viral) 🎬🔥 Comment "ANIMATION" and I'll send you the prompt! Follow me ( @tonistelk ) for more AI tips! 🧡 #claudeedit #ai #claude #animation

**Transcripción:** Lista hablada de 10 estilos de animación: pixel art, chalkboard style (estilo pizarrón), glow sketch, PS2 style, comic art, flat vector, minimal line, CGI motion, Lego style, explainer 3D. No da ningún prompt ni detalle técnico de cómo lograr cada estilo — solo nombra los 10 estilos mientras se muestran ejemplos visuales en el video.

**Qué dice / enseña:** Enumera 10 "estilos" de animación/render visual (pixel art, pizarrón, boceto con glow, PS2, comic, vector plano, línea minimalista, movimiento CGI, Lego, explicativo 3D) presentados como generables con Claude, a modo de catálogo de referencias estéticas para pedir animaciones. El prompt exacto para cada estilo no está en el video — lo ofrece por DM a cambio de comentar "ANIMATION".

**Herramientas/skills que menciona:** Menciona a Claude como el motor para generar estas animaciones, pero no da el prompt real ni un comando/skill específico — es gancho para captar comentarios y mandar el prompt por DM.

**Cómo aplicarlo:** Sirve como lista de referencia de estilos visuales para pedirle a Claude (o a cualquier herramienta de motion/código) al generar una animación: en vez de pedir "animalo" en genérico, especificar el estilo concreto (ej: "hazlo en pixel art" o "estilo PS2" o "explainer 3D") para guiar mejor el resultado. No hay prompt técnico citable de este reel porque no está en el audio ni en el caption.

---

### 55.
## Sky Tan — https://www.instagram.com/p/DambEp1igDW/

**Caption:** The perfect scripting structure

**Transcripción:** Hook, lead, body one, open loop one, body two, open loop two, body three, CTA. Esa es la estructura perfecta para contenido de formato corto. En el hook y el lead: el hook rompe el patrón de lo que la gente está viendo (el scroll), y el lead los arrastra hasta el segundo 10 — una vez anclados ahí, ya no siguen scrolleando. Body one introduce la primera pieza de valor. Los "open loops" (ganchos abiertos) generan más curiosidad ("eso no es lo más loco", "y curiosamente, en 1893 Richard Feynman...", etc. — ejemplos de frases gancho). Esa estructura de cuerpo + open loop se repite dos veces. Por último, el CTA toma a los espectadores más "calientes" (más engaged) y los mete en el siguiente paso del funnel, por ejemplo "comenta tal palabra clave para recibir tal valor".

**Qué dice / enseña:** Enseña una estructura de guion de 8 partes para contenido corto (reels/shorts): Hook → Lead → Body 1 → Open Loop 1 → Body 2 → Open Loop 2 → Body 3 → CTA. Explica la función de cada parte: el hook rompe el patrón de scroll, el lead ancla al espectador hasta el segundo 10, los "open loops" sostienen la curiosidad entre bloques de valor, y el CTA convierte a los viewers más engaged en el siguiente paso de un funnel (ej. comentar una palabra clave).

**Herramientas/skills que menciona:** Ninguna herramienta de IA/código — es pura estructura de copywriting/guion para video corto.

**Cómo aplicarlo:** Usar esta plantilla de 8 bloques al escribir guiones propios de reels: abrir con un hook que rompa el patrón visual/narrativo, sumar un lead que prometa valor concreto antes del segundo 10, alternar bloques de valor (body) con ganchos de curiosidad sin resolver (open loop) en vez de entregar todo de una, y cerrar con un CTA que dirija a los espectadores más interesados a un siguiente paso medible (comentar una palabra, seguir un link, etc.). Complementa directamente la skill `reel-script-writer` ya guardada.

---

### 56.
## samzia (Barsam Zia) — https://www.instagram.com/p/DexbLYsBkPO/

**Caption:** Computer and cars basically

**Transcripción:** Es un fragmento de una canción/audio musical ("Don't take a breath... when I wake the storm, I'm gonna head to the trap..."), no hay narración ni explicación habida — no es contenido hablado sobre ningún tema técnico.

**Qué dice / enseña:** No se puede determinar contenido de marketing/dev/diseño/IA en este reel: el caption es una frase vaga ("Computer and cars basically") y el audio es solo una canción de fondo, sin voz explicando nada. Sin ver las imágenes/video del post no hay forma de saber qué se muestra (posiblemente un meme o montaje visual sobre autos y computadoras, pero es especulación).

**Herramientas/skills que menciona:** Ninguna — no hay contenido hablado ni caption que mencione herramientas.

**Cómo aplicarlo:** No aplica. Este reel no tiene contenido verificable (ni caption útil ni transcripción con información) relacionado a IA, dev, marketing o diseño; habría que abrir el post en Instagram para ver qué muestra visualmente antes de sacar cualquier conclusión.

---

### 57.
## Rourke Sefton-Minns — https://www.instagram.com/p/Ddytu5oqOEi/

**Caption:** Comment "AI" for the full list 🔥 Camera angles are one of the fastest ways to make AI generations look cinematic instead of generic. This breakdown covers the key shots, from low angles and Dutch tilts to overheads and over-the-shoulder, and how to prompt each one inside Magnific. Essential for filmmakers, designers, and creators who want full directorial control over every frame. @byemmasvision original inspo! #MagnificAI #CameraAngles #AIPrompts #AIFilmmaking #CreativeAI

**Transcripción:** Lista hablada de tipos de plano/ángulo de cámara para usar en prompts de generación de imagen/video con IA: Wide, Medium, Close Up, Macro, Overhead, Fish Eye, Profile, 3 quarter, Rear, Over the Shoulder, POV, Prism Reflection, Eye Level, Low Angle, High Angle, Dutch Angle, Overhead, Aerial, Ground Level, Worm's Eye View, Inside Hole, Hoop Level, Wide Angle, Close Up, Fish Eye, Fish Eye Close Up, High Angle, Close Up, Low Angle, Close Up, Selfie, Silhouette, Foreground Occlusion, Foreground Focus, Background Focus, Lens Flare, Magnifying Glass, Inside the Fridge Shot, Common AI — y ofrece mandar un PDF con todos estos términos más los prompts exactos.

**Qué dice / enseña:** Muestra un catálogo extenso de ángulos y tipos de plano cinematográfico (wide, close up, dutch angle, over the shoulder, worm's eye view, lens flare, etc.) como vocabulario para incluir en prompts de generación de imagen/video con IA, específicamente dentro de la herramienta Magnific AI, con el objetivo de lograr resultados con look cinematográfico en vez de genérico.

**Herramientas/skills que menciona:** Menciona explícitamente Magnific AI como la herramienta donde se aplican estos prompts de ángulo de cámara. No da los prompts exactos en el video (los ofrece por PDF al comentar "AI").

**Cómo aplicarlo:** Al generar imágenes o video con cualquier modelo de IA (Magnific, Midjourney, generadores de video, etc.), incorporar explícitamente el tipo de plano/ángulo en el prompt (ej: "dutch angle", "over the shoulder", "worm's eye view", "lens flare") en vez de dejarlo implícito, para tener más control direccional sobre la composición y lograr un resultado más cinematográfico. Es una lista de vocabulario de referencia reusable para prompts de imagen/video.

---

### 58.
## Jar Labs Solutions — https://www.instagram.com/p/Dfcj7oaAbHS/

**Caption:** Claude can edit your videos. It just needs the right tools. 10 tools that turn Claude into a video editor: 1. Ghost Editor: raw talking-head footage into a polished reel 2. FFmpeg Skill: cut, trim, resize and add subtitles 3. Claude Shorts: long videos into vertical clips with captions 4. MotionClone: rebuild a reference animation as an editable project 5. Motion Skills: animated text, moving charts and explainers 6. yt-dlp: download videos you have the rights to use 7. Whisper: speech into subtitles and transcripts 8. Agent Skills Hub: hundreds more video tools in one list 9. Three.js Skills: 3D scenes with lighting and camera moves 10. HyperFrames: HTML in, rendered video out. Don't install all ten. Pick the one job that eats your time, and start there. Save this. Know someone who edits videos? Send it to them. #claudecode #videoediting #ai #contentcreation #gojarlabs

**Transcripción:** Repite el mismo listado del caption casi palabra por palabra: Claude puede editar videos si tiene las herramientas correctas. Lista las 10: Ghost Editor (convierte grabación cruda tipo talking-head en reel pulido), FFmpeg Skill (cortar, recortar, resize, subtítulos), Claude Shorts (encuentra los mejores momentos de un video largo y los convierte en clips verticales), MotionClone (reconstruye una animación de referencia como proyecto editable), Motion Skills (texto animado, gráficos en movimiento, explicativos), yt-dlp (descarga videos con derechos de uso), Whisper (habla a subtítulos/transcripciones), Agent Skills Hub (cientos de herramientas de video más en un solo listado), Three.js Skills (escenas 3D con iluminación y movimiento de cámara), HyperFrames (HTML como input, video renderizado como output). Cierra recomendando no instalar las 10 juntas sino elegir la que resuelve el cuello de botella real.

**Qué dice / enseña:** Catálogo de 10 "skills"/herramientas que se pueden instalar en Claude Code para que funcione como editor de video: desde limpieza de talking-heads (Ghost Editor) y edición cruda (FFmpeg), hasta generación de cortes verticales (Claude Shorts), clonado de animaciones de referencia (MotionClone), motion graphics (Motion Skills, Three.js Skills, HyperFrames), descarga de video (yt-dlp) y transcripción (Whisper). El consejo central es no instalar todo de golpe sino identificar el cuello de botella propio y resolver ese primero.

**Herramientas/skills que menciona:** FFmpeg, yt-dlp, Whisper, Three.js — todas herramientas/skills ya instaladas y usadas en este mismo proyecto (el script `process_reel.sh` usa yt-dlp y Whisper/Groq). HyperFrames también coincide con la skill `hyperframes` ya disponible en este entorno. Ghost Editor, Claude Shorts, MotionClone, Motion Skills y Agent Skills Hub parecen nombres de skills/productos de terceros (no necesariamente oficiales de Anthropic) que no están confirmados como instalados acá.

**Cómo aplicarlo:** Directamente aplicable: este mismo proyecto ya usa yt-dlp + Whisper (vía Groq) para bajar y transcribir reels, igual que describe el video. Para iterar sobre contenido propio de video, valdría la pena explorar específicamente la skill `hyperframes` (ya disponible) para motion graphics, y evaluar si "Ghost Editor", "Claude Shorts" o "MotionClone" existen como skills instalables reales antes de asumir que están disponibles — no vienen en la lista de skills de este entorno, así que habría que buscarlas o pedirle al usuario el link/repo antes de instalar nada (evitando gastar tiempo en herramientas no verificadas).

---

### 59.
## BreakingBreach — https://www.instagram.com/p/DfEpwT9SRHe/

**Caption:** Comment "Vibe" to get the complete pre-launch security toolkit! Built an app with Claude or another AI coding tool? Check its security before going live. This video covers authentication, API keys, database access, payments, and other protections your app needs. #claude #security #cyber #vibecoding #vulnerability

**Transcripción:** Es un prompt/checklist dirigido a Claude, leído como si fuera un pedido del usuario: "Claude, no quiero que hackers entren a mi app vibecodeada, así que por favor... configura autenticación correcta, esconde las API keys, asegura la base de datos, fuerza HTTPS, hashea las contraseñas, valida los formularios server-side, protege contra XSS, registra y monitorea actividad sospechosa, bloquea las rutas de admin, usa queries parametrizadas, revisá las variables de entorno, agregá rate limiting, restringí la configuración de CORS, agregá security headers, asegurá las cookies de sesión, agregá protección CSRF, hacé que los links de reseteo de contraseña expiren, restringí los tipos y tamaños de archivo subido, verificá precios y pagos, deshabilitá el modo debug en producción, actualizá dependencias vulnerables, quitá paquetes sin usar, revisá archivos expuestos, escaneá el historial de Git por secretos filtrados, revocá y reemplazá las keys comprometidas, corré una revisión de seguridad completa, y finalmente testeá las protecciones y dame un reporte de hallazgos y arreglos." Cierra pidiendo comentar "Vibe" para mandar el toolkit completo.

**Qué dice / enseña:** Es un checklist de seguridad pre-lanzamiento para apps "vibecodeadas" (hechas con IA), estructurado como un prompt literal que se le puede tirar a Claude para que audite y arregle: autenticación, manejo de API keys y secretos, HTTPS, hashing de passwords, validación server-side, XSS, logging/monitoreo, rutas de admin, SQL injection (queries parametrizadas), env vars, rate limiting, CORS, security headers, cookies de sesión, CSRF, expiración de links de reset, validación de uploads, verificación de pagos, modo debug, dependencias vulnerables, paquetes sin usar, archivos expuestos, secretos filtrados en Git, rotación de keys comprometidas, y un reporte final de hallazgos/arreglos.

**Herramientas/skills que menciona:** Menciona a Claude (o "otra herramienta de IA coding") como el agente al que se le pasa este prompt de auditoría, pero no nombra ninguna skill específica instalable más allá de decir "comment Vibe" para mandar el toolkit completo por DM.

**Cómo aplicarlo:** Este checklist es prácticamente un resumen ejecutivo de lo que ya cubre la skill `vibecoding-launch-checklist` guardada en la memoria del usuario para revisiones de seguridad/pagos antes de lanzar algo vibecodeado — se puede usar como lista de verificación rápida o como insumo para ampliar esa skill si le falta algún ítem (ej: expiración de links de reset, revisión de Git history por secretos filtrados, o testing explícito post-fix con reporte).

---

### 60.
## Nick Saraev — https://www.instagram.com/p/DfUBU1tPVZn/

**Caption:** Comment "BLENDER" to get these 94 AI Skills to turn Claude Code into a Blender Expert. Claude Code can now run Blender for you. So you can build full 3D models, textures and animations just by describing them. It's a different way to make 3D art. And it's completely free. It's called Blender Skills, and it's a free and open source pack of 94 skills. It teaches your agent how to work like a professional 3D artist. That's the know how Claude brings to your project. All you need is Blender open with a plugin that connects it. That's the only setup you need to do. Then you just describe what you want, like a cyberpunk world for Unreal Engine. And the Blender Director skill takes over. Think of it as the project manager for the whole scene. It plans the whole job and builds the characters, the props and the environment. It's like handing your idea to a full 3D team. Then it adds the lighting and textures. It optimizes everything for your game and exports it. And it coordinates every step along the way. From a single sentence to a fully finished 3D scene. #blender #claudecode #aiskills #Ai3D #3dmodeling

**Transcripción:** Repite el contenido del caption: Claude Code puede correr Blender para armar modelos 3D, texturas y animaciones solo con describirlos, de forma gratuita. Se llama "Blender Skills", un pack gratuito y open-source de 94 skills que le enseña al agente a trabajar como un artista 3D profesional. El único setup necesario es tener Blender abierto con un add-on/plugin que lo conecte. Después se describe lo que se quiere (ej: "un mundo cyberpunk para Unreal Engine") y la skill "Blender Director" toma el control: planea todo el trabajo, construye personajes, props y entorno, agrega luces y texturas, optimiza para el juego motor destino y exporta, coordinando cada paso — de una sola frase a una escena 3D terminada.

**Qué dice / enseña:** Presenta "Blender Skills", un paquete open-source de 94 skills para Claude Code que conecta con Blender (vía un add-on/plugin) y permite generar modelos, texturas, iluminación y animaciones 3D completos a partir de una descripción en lenguaje natural, con una skill orquestadora ("Blender Director") que actúa como project manager de toda la escena (personajes, props, entorno, luces, texturas, optimización y exportación).

**Herramientas/skills que menciona:** Blender (el software 3D), un plugin/add-on que conecta Blender con Claude Code, y el pack de 94 skills llamado "Blender Skills" (con una skill central "Blender Director"). No está entre las skills ya instaladas en este entorno — habría que buscarlo/instalarlo aparte (el creador lo manda por DM al comentar "BLENDER").

**Cómo aplicarlo:** Si se necesita generar assets o escenas 3D (por ejemplo para los videos de motion graphics que ya se hacen en este proyecto, tipo HyperFrames/Three.js), vale la pena buscar este pack "Blender Skills" de 94 skills e instalarlo vía plugin de Blender + Claude Code, en vez de armar escenas 3D manualmente o depender solo de Three.js Skills. Antes de instalar algo así conviene confirmar la fuente real del pack (no viene documentado en este reel, solo se ofrece por DM) para evitar instalar algo no verificado.

---

### 61.
## Distribb — https://www.instagram.com/p/DfZ6ypijJW-/

**Caption:** Claude can now test dozens of titles for your pages to improve CTR, and therefore your SEO rankings. Google admitted in court that clicks help rank pages, and a title test takes two weeks, not months. How it works: 1. Connect Search Console to the SEO connector in Claude 2. Claude finds your page-one pages with weak clicks 3. It writes new titles, sees which searches still scroll past you, and learns what makes people click 4. Pro tip: test your top 3 title ideas as Google ads at $20 a day, then put the winner on the page. Save this for later and share it with a friend who thinks titles don't matter. Comment TITLE and I'll send you the link to the connector.

**Transcripción:** Repite el caption casi literal: Claude puede testear docenas de títulos de página para mejorar el CTR y por lo tanto el ranking SEO. Google admitió en una causa judicial que los clicks ayudan a rankear páginas, y un test de títulos tarda dos semanas en vez de meses. Se hace con el "conector SEO" en Claude: una vez conectado Search Console, Claude encuentra las páginas de la primera posición de Google con clicks débiles, escribe títulos nuevos, ve qué búsquedas siguen scrolleando de largo sin clickear, y aprende qué hace que la gente clickee. Tip extra: testear los 3 mejores títulos como Google Ads a $20/día y poner el ganador en la página real. Cierra pidiendo comentar "TITLE" para mandar el link al conector.

**Qué dice / enseña:** Explica un método para mejorar el SEO on-page mediante testing de títulos (title tags): usar un "conector SEO" de Claude conectado a Google Search Console para que Claude detecte páginas bien posicionadas pero con CTR bajo, genere variantes de título, y aprenda cuáles generan más clicks — con el agregado de validar los 3 mejores candidatos corriéndolos como Google Ads pagos ($20/día) antes de ponerlos en la página real, usando el CTR real de ads como señal de validación barata y rápida (2 semanas vs. meses esperando señal orgánica).

**Herramientas/skills que menciona:** Menciona un "SEO connector" dentro de Claude que se conecta a Google Search Console — no se nombra qué conector específico es ni si es oficial de Anthropic o de un tercero; se ofrece el link por DM al comentar "TITLE", así que no se puede confirmar su identidad exacta desde este análisis.

**Cómo aplicarlo:** La técnica central (generar variantes de título con IA, medir cuál sube el CTR, y validarlas primero como Google Ads baratos antes de tocar la página orgánica) es aplicable sin depender de ningún conector específico: se puede replicar manualmente pidiéndole a Claude que proponga variantes de title tag a partir de datos exportados de Search Console (páginas con alto impresiones/bajo CTR), y testeando los candidatos top como ads de bajo presupuesto antes de aplicar el cambio definitivo en el sitio.

---

### 62.
## Varun Kandula — https://www.instagram.com/p/DfIt_rVOKJj/

**Caption:** Save this before your next meta campaign 👀

**Transcripción:** El audio capturado no corresponde a contenido hablado real ("I'm a best week one. I never meant to call you tomorrow"), probablemente ruido de fondo o música mal transcripta por Whisper. El mensaje real del reel parece estar en overlays de texto en pantalla que el audio no captura.

**Qué dice / enseña:** No se puede determinar el contenido específico con certeza. A juzgar por la caption ("antes de tu próxima campaña de Meta") y los comentarios del post (que hablan de retargeting, de gastar $100k en ads, de que "todos lo complican demasiado"), el video parece ser un checklist o lista de errores/tips para campañas de Meta Ads, pero no se puede confirmar el contenido exacto sin ver el video.

**Herramientas/skills que menciona:** No se puede determinar desde el audio disponible.

**Cómo aplicarlo:** No se puede dar una aplicación concreta sin ver el contenido visual del reel. Recomendación: revisar el post directamente en Instagram para extraer los tips reales, ya que el análisis automático por audio no fue suficiente en este caso.

---

### 63.
## Dakota Hermes — https://www.instagram.com/p/DfXrim6xnyH/

**Caption:** how to test new ad angles, explained.

**Transcripción:** Explica el "angle matrix": un ángulo es la razón por la que alguien compraría, apuntada a una persona específica en una etapa específica de consciencia (no es lo mismo que un hook o un edit nuevo del mismo pitch). Cruza los 8 deseos de "Cashvertising" (seguir vivo, comida/bebida, sentirse seguro, atracción, comodidad, ganar, proteger a la familia, ser aceptado) con las 5 etapas de consciencia de "Breakthrough Advertising" (unaware, problem aware, solution aware, product aware, most aware), dando 40 ángulos posibles por oferta. Ejemplo con un curso de Meta Ads: a alguien unaware el ángulo es "por qué los ads buenos dejaron de funcionar", a alguien problem aware es "gastar más y conseguir menos", a alguien que ya te conoce es "el sistema detrás de $6M al mes". Para testear: cada ángulo en su propio ad set con 3-5 versiones, dejando que cada uno gaste 2-3x el costo objetivo antes de juzgarlo (si metés 30 ads en un ad set, Meta solo le da presupuesto real a 3 o 4).

**Qué dice / enseña:** Framework de marketing/performance ads para generar y testear ángulos creativos sin repetir siempre el mismo ángulo ganador, basado en cruzar deseos humanos con etapas de consciencia del comprador.

**Herramientas/skills que menciona:** Menciona que armaron "un Claude skill que corre el angle matrix" (lo ofrecen en su grupo gratuito de Skool, no da detalles técnicos de cómo está armado).

**Cómo aplicarlo:** Se podría construir una skill o prompt propio que, dado un producto/oferta, genere automáticamente la matriz de 40 ángulos (8 deseos x 5 etapas de consciencia) y sugiera copy de hook para cada celda — útil para separar testing de ads o de contenido orgánico por ángulo en lugar de por formato/edición.

---

### 64.
## Batu Ulker | Revenue Partner — https://www.instagram.com/p/DfXoI3kFJzz/

**Caption:** How Alex Hormozi makes 150 to 750 ads from one filming session: divide cada ad en hook, meat y CTA (50 hooks × 3-5 meats × 1-3 CTAs = cada combinación es un ad distinto). Los hooks vienen de ads ganadores propios, contenido orgánico propio, ads/contenido de otros y las ad libraries, repartidos en distintos niveles de consciencia. El "meat" rota 5 formatos: demostración, testimonial, educativo, historia, faceless. El CTA dice qué hacer, por qué importa, cuándo, qué tan fácil es y qué pasa después. El autor revisó la cuenta de Hormozi en la Meta Ad Library: sus 27 ads de larga duración son solo 3 ideas, y una corre como 15 ads distintos. Para ofertas high-ticket propone un cambio: mandar el CTA a una video page en vez de directo al calendario, para filtrar a la audiencia mixta que traen cientos de hooks antes de que agende.

**Transcripción:** Coincide casi palabra por palabra con la caption (el video narra el mismo framework de hook/meat/CTA, el dato de la Ad Library de Hormozi, y el cambio sugerido de mandar tráfico a video page en vez de al calendario).

**Qué dice / enseña:** Sistema de producción de ads en masa a partir de una sola sesión de filmación, separando el ad en tres piezas modulares (hook/meat/CTA) y combinándolas, más un ajuste de funnel para ofertas high-ticket (filtrar con una video page antes del calendario).

**Herramientas/skills que menciona:** Ninguna herramienta de IA/código — es un framework de producción de contenido y ads, no nombra ninguna skill ni IA.

**Cómo aplicarlo:** Aplicable a la producción de contenido/ads propios: grabar varios hooks, meats y CTAs sueltos en una sola sesión y combinarlos después en edición, en vez de filmar cada ad entero de una sola vez. Para funnels de oferta cara, insertar una página de video intermedia antes del booking/calendario como filtro de intención.

---

### 65.
## Rourke Sefton-Minns — https://www.instagram.com/p/DfXaQcyoaJ5/

**Caption:** Comment "AI" for the full list with prompts. Explica que la iluminación es lo que separa una generación de IA plana de una cinematográfica, y que el reel muestra 34 estilos de luz con ejemplos (desde setups clásicos de cine hasta looks estilizados), todos generados en Higgsfield, como referencia para filmmakers, diseñadores y publicistas.

**Transcripción:** Lista hablada de los 34 estilos de iluminación mostrados: high key, low key, Rembrandt, butterfly, split light, loop light, broad light, short light, chiaroscuro, silhouette, rim light, hard light, soft light, bounce light, top light, under light, golden hour, blue hour, day for night, moonlight, window light, practical light, fire light, Venetian blinds, dappled light, volumetric light, flat light, neon light, teal and orange, monochrome red, screen glow, passing light, strobe light, theatrical light.

**Qué dice / enseña:** Catálogo visual/educativo de 34 técnicas de iluminación cinematográfica (clásicas de cine y estilizadas), generadas con IA para mostrar cómo cada una afecta mood, profundidad y narrativa en una imagen.

**Herramientas/skills que menciona:** Higgsfield (herramienta de generación de imagen/video con IA) — las 34 imágenes de referencia están generadas ahí.

**Cómo aplicarlo:** Sirve como vocabulario/cheat-sheet de iluminación para escribir prompts de generación de imagen o video (en Higgsfield, Midjourney, Sora, etc.): en vez de decir "que se vea cinematográfico", nombrar el estilo de luz específico (ej. "Rembrandt lighting", "teal and orange", "golden hour") da resultados mucho más controlados y consistentes.

---

### 66.
## Sanjai • AI Builder — https://www.instagram.com/p/DfXGd0Wsleu/

**Caption:** I ranked the 10 biggest AI tools from S to B tier. Not just benchmarks: coding, reasoning, pricing y quejas reales de usuarios. S: ChatGPT, Claude. A: Gemini, Perplexity, Kimi. B: Grok, DeepSeek, Qwen, Mistral, GLM.

**Transcripción:** Ranking hablado de los 10 modelos: Grok (B-tier, potente pero inconsistente), Perplexity (A, bueno para research pero hay que verificar fuentes), Claude (S-tier, "Opus 5.5 y Claude Code son mis favoritos para coding en serio"), DeepSeek (B, muy buena relación precio/valor pero hay que verificar sus respuestas), Gemini (A, potente pero memoria y confiabilidad necesitan trabajo), Qwen (modelos fuertes pero la experiencia necesita pulido), Kimi K3.1 Pro (subestimado), Mistral (prometedor pero no su primera opción), GLM (buena relación precio/valor para coding agents), y ChatGPT (S-tier, no porque gane en todo sino porque ChatGPT + Work + Codex lo hacen el mejor paquete completo).

**Qué dice / enseña:** Ranking personal/subjetivo de los 10 modelos de IA más grandes del momento, tier por tier, con un comentario puntual sobre fortalezas y debilidades de cada uno (no es un benchmark formal, es opinión basada en uso).

**Herramientas/skills que menciona:** Los 10 modelos/herramientas rankeados: ChatGPT, Claude (Opus 5.5, Claude Code), Gemini, Perplexity, Kimi, Grok, DeepSeek, Qwen, Mistral, GLM.

**Cómo aplicarlo:** Como referencia rápida y desactualizable (es un ranking de un momento puntual) para elegir qué modelo probar según la tarea: coding pesado → Claude/Claude Code o GLM; research → Perplexity o Gemini; uso general con ecosistema de apps → ChatGPT. No reemplaza probar cada modelo con el caso de uso propio.

---

### 67.
## Textura — https://www.instagram.com/p/De4cg9VmZ3J/

**Caption:** ✍🏼 Comment «PROMPTS» and I'll send you all five prompts behind these websites. "No podés promptear tu camino al buen gusto, solo podés arrancar desde ahí. 'Que se vea premium' no es un estilo que un modelo pueda buscar. Premium es lo que queda después de cientos de decisiones: qué tan rápido se mueven las cosas, cuánto espacio tienen, qué se corta, dónde cae el ojo primero. Nada de eso entra en una oración, así que el modelo promedia: gradiente grande, grid limpio, fade-in on scroll. Estos cinco sitios son esas decisiones ya tomadas, escritas como prompts." Cómo funciona: 1) elegís el sitio que te gusta, 2) copiás su prompt (el sitio entero escrito, cada valor y timing), 3) lo pegás en tu IA y te devuelve el sitio como un HTML, con layout, copy y motion incluidos, 4) lo transformás con tu marca, tu copy, tus secciones — arrancás de algo bueno, no de cero, 5) lo subís con cualquier stack: React, Next.js, Vue, Shopify, WordPress, Webflow, Lovable, donde tu IA escriba código.

**Transcripción:** No se pudo descargar el video ni el audio (el post es un carrusel de 5 piezas y yt-dlp devolvió "No video formats found" para 4 de ellas, lo que indica que son imágenes/diapositivas, no clips con audio). El contenido real está en lo visual (screenshots de los 5 sitios web de ejemplo), que no se puede inferir sin verlo.

**Qué dice / enseña:** Plantea que el "buen gusto" en diseño web no se puede lograr solo con un prompt genérico tipo "hazlo premium" — un LLM sin más contexto promedia hacia lo genérico (gradientes, grids, fade-ins). La propuesta es usar prompts ultra-detallados ("el sitio entero escrito, cada valor y timing") que ya capturan cientos de decisiones de diseño, pegarlos en una IA para generar el HTML completo de un sitio de referencia, y después adaptarlo a marca propia antes de llevarlo a cualquier stack de producción.

**Herramientas/skills que menciona:** Menciona "Claude" en los hashtags del post como una de las IA con las que se puede ejecutar estos prompts, y "getlayers" (posible herramienta/producto propio de la cuenta, sin más detalle). El flujo final es agnóstico de stack (React, Next.js, Vue, Shopify, WordPress, Webflow, Lovable).

**Cómo aplicarlo:** Para proyectos propios, en vez de pedirle a un agente de código "hacé un landing premium", escribir o guardar prompts de referencia extremadamente específicos (layout exacto, timings de animación, jerarquía visual) de sitios que ya admiramos, generar el HTML base con eso, y recién ahí adaptarlo a la marca/copy propios — baja el promedio genérico que tira cualquier LLM cuando el prompt es vago.

---

### 68.
## Michael Quoc Ly — https://www.instagram.com/p/DeQO86WO9l5/

**Caption:** Give this to Claude to make insane motion designs!

**Transcripción:** Lista hablada de estilos visuales: Particles, Liquid Morph, Holographic, Neon Glow, Wireframe 3D, Glass Morphism, Kinetic Type, Isometric, Clay 3D, ASCII Art, Gradient Mesh, Comic Book, Split Flap Display, Retro VHS, Halftone, Pixel Art, Blueprint, Art Deco, Neo-Brutalism.

**Qué dice / enseña:** Catálogo rápido de ~19 estilos visuales/estéticos para motion design, pensado como lista de referencia para pedirle a una IA (puntualmente Claude) que genere animaciones o piezas de diseño en alguno de esos estilos.

**Herramientas/skills que menciona:** Claude, como la IA a la que se le pasaría esta lista de estilos para generar motion graphics.

**Cómo aplicarlo:** Usar estos nombres de estilo como vocabulario concreto al pedirle a Claude (o a cualquier agente de código/diseño) una pieza de motion design — nombrar el estilo exacto (ej. "Glass Morphism", "Neo-Brutalism", "Split Flap Display") da resultados mucho más dirigidos que describir el efecto en palabras propias. Complementa bien con la skill `motion-effects` o `motion-prompt-writer` ya disponibles para construir el prompt completo.

---

### 69.
## alex benshaw — https://www.instagram.com/p/DetbRtDRQUP/

**Caption:** use these to land clients & follow for more sauce

**Transcripción:** "Acá hay 35 ideas de contenido S-tier para founders": por qué empezaste, tu primer cliente, tu fracaso de negocio más grande, tu lección más cara, tu primer mes de 10K, tu mayor quiebre, cuando casi renunciaste, arrancar de cero, lo que nunca repetirías, desacuerdos con la industria, tu misión, a quién ayudás y por qué, a quién NO ayudás, tus frameworks característicos, tu metodología única, tus creencias de negocio más fuertes, una historia de éxito de cliente, un antes/después de cliente, una conversación franca con un cliente, objeciones que superaste, errores de clientes que arreglaste, una transformación de cliente en vivo, tu mejor testimonio, el detrás de escena de tu entrega, llamadas con clientes por dentro, tu oferta explicada a fondo, qué compran realmente los clientes, por qué sos distinto, tu resultado personal más grande, tu resultado de cliente más orgulloso, mitos de la industria, opiniones de negocio impopulares, el error más grande de tu audiencia, lo que los clientes necesitan escuchar, y tu estilo de vida ideal. Todo esto construye conexión, y la conexión construye confianza, y la confianza construye negocios.

**Qué dice / enseña:** Lista de 35 ángulos/ideas de contenido orientados a coaches, consultores y founders que venden servicios, pensada para generar confianza y atraer clientes mostrando historia personal, resultados de clientes y postura/opiniones de la marca personal.

**Herramientas/skills que menciona:** Ninguna — es una lista de ideas de contenido, no nombra ninguna herramienta de IA o código.

**Cómo aplicarlo:** Usar esta lista como banco de ideas para guiones de reels/posts propios de marca personal o de servicios (coaching, consultoría, agencia): elegir una idea por semana y convertirla en un guion corto con la skill `reel-script-writer`, en vez de arrancar cada video desde cero sin tema definido.

---

### 70.
## Nuhu Shaik — https://www.instagram.com/p/DfGxiB0xBXQ/

**Caption:** Comment ENGINEER for a free level up guide 🫱🏼‍🫲🏽👀

**Transcripción:** "Vibe Coder vs AI Engineer en 30 segundos". Preguntale a un Vibe Coder qué stack usa y te va a decir con confianza "Claude Code, obvio" — no tiene idea de con qué está construida su app ni a qué está conectada. Su forma de pensar es "construí esto, construí aquello", y cuando se topa con errores dice "Claude, arreglá esto, no cometas errores" — sin referencias, documentación ni pensamiento crítico o creativo. Y después se pregunta por qué funciona y se ve genérico ("slop"). Por otro lado, un AI Engineer piensa como un manager: ya tomó decisiones críticas de stack, integraciones y diseño antes de que la IA escriba una sola línea de código. También desarrolló su propio criterio ("taste") en skills de diseño custom, y sus prompts siguen un formato definido. Cuando no sabe algo, le pide a la IA que le haga preguntas para poder tomar una decisión informada en vez de dejar que la IA decida todo. Los AI Engineers también tienen automatizaciones para encontrar y arreglar bugs antes de que causen un problema más grande.

**Qué dice / enseña:** Contrapone dos perfiles de uso de IA para programar: el "vibe coder" que delega todo sin entender el stack ni pedir contexto, versus el "AI engineer" que toma las decisiones de arquitectura de antemano, define su propio criterio de diseño, hace que la IA le haga preguntas antes de decidir, y automatiza la detección de bugs.

**Herramientas/skills que menciona:** Claude Code (como la herramienta que usa típicamente el "vibe coder" sin entenderla a fondo).

**Cómo aplicarlo:** Coincide directamente con la regla ya anotada de "no sobregenerar código de más, no asumir intenciones sin preguntar": antes de tirarle una tarea a Claude Code, definir stack e integraciones de antemano, pedirle a la IA que haga preguntas de aclaración cuando algo no está claro en vez de dejarla decidir sola, y mantener algún proceso (manual o automatizado) de revisión de bugs antes de que se acumulen.

---

### 71.
## Jun Yuh | Personal Branding & Content Strategy — https://www.instagram.com/p/Ddz3gW_x_tZ/

**Caption:** follow for more content tips 🧠✅

**Transcripción:** Explica dónde va la mirada del espectador en pantalla, dónde poner el caption y cómo enganchar el hook ahí. Marca zonas de la pantalla: una "zona segura", una "zona de peligro" y una zona que hay que evitar a toda costa (donde la UI de Instagram tapa el contenido). Recomienda hacer punch-in (zoom/corte) manteniendo la línea de los ojos igual entre tomas, y si el fondo es muy cargado, agregarle un stroke (contorno) al texto para que se lea bien.

**Qué dice / enseña:** Reglas de edición visual para reels: dónde ubicar texto/caption según las zonas seguras de la pantalla (evitando que la UI de Instagram tape contenido clave), cómo mantener continuidad visual al cortar entre planos (eyeline matching) y cómo mejorar la legibilidad del texto superpuesto con stroke cuando el fondo es complejo.

**Herramientas/skills que menciona:** Ninguna herramienta de IA/código — son principios de edición de video manual (framing, texto, continuidad).

**Cómo aplicarlo:** Al editar reels propios, chequear que el texto/caption no caiga en las zonas donde Instagram pone su UI (parte superior e inferior/laterales), mantener la altura de los ojos consistente entre cortes al hacer punch-ins, y agregarle stroke/contorno al texto cuando el fondo del video es visualmente ruidoso.

---

### 72.
## Stiles AI — https://www.instagram.com/p/Dd9DCEZh3In/

**Caption:** Let your AI doomscroll. Just don't stop at one skill per reel. Put everything you've saved in one place, including the freebies sitting in your DMs, and have it keep the best of all of it. Comment CAMPAIGN and I'll send you the full guide. What would you build first?

**Transcripción:** El creador cuenta que le preguntan mucho cómo convertir reels guardados en "skills" de IA, y dice que la mayoría comete el error de hacer una skill por cada reel por separado. Su método: primero ordenar los favoritos guardados en colecciones por tema (edición, marketing, etc.); después juntar TODO lo guardado (reels + todos los prompts/templates que la gente te manda por DM) en un solo lugar, como una especie de "Claude Project" (una base de conocimiento, no solo un montón de archivos sueltos); el paso clave es hacer que la IA compare el contenido: si varios creadores enseñan lo mismo, que se quede con la versión que realmente funciona y descarte el resto; por último, apilar esas skills ya depuradas en un único setup, de forma que cuando arranca un proyecto nuevo, la IA ya "conoce todo el playbook" en vez de tener que explicarle todo de cero.

**Qué dice / enseña:** Un sistema para destilar contenido guardado (reels, prompts, templates) en una base de conocimiento de IA reutilizable: 1) categorizar el material guardado en colecciones temáticas, 2) centralizarlo todo en un repositorio único tipo proyecto de IA, 3) usar la IA para comparar versiones redundantes del mismo consejo/tema y quedarse solo con la mejor, y 4) combinar las skills resultantes en un setup único que se reutiliza en cada proyecto nuevo.

**Herramientas/skills que menciona:** Habla de un "Claude Project" (proyecto de Claude con base de conocimiento) y de construir "skills" a partir de ese material, aunque no da pasos técnicos concretos (ni comandos, ni estructura de archivos) — es la idea general del sistema, no un tutorial paso a paso.

**Cómo aplicarlo:** Es básicamente el enfoque que ya se usa en este mismo proyecto de reels-analysis: en vez de generar una skill por cada reel analizado, agrupar los reels por tema (marketing, dev/vibecoding, diseño, edición), comparar los que repiten el mismo consejo y quedarse con la versión más clara/completa, y después consolidar eso en skills reutilizables (como ya existen `vibecoding-launch-checklist` y `reel-script-writer`) en vez de crear una skill nueva por cada video individual.

---

### 73.
## Joey Mulcahy — https://www.instagram.com/p/DfD6caLvqF1/

**Caption:** drop 'ads' in the comment for the workflow that creates all these for your brand using AI

**Transcripción:** Es una lista hablada (tipo catálogo, sin mucho desarrollo) de formatos de anuncios/creativos virales: censored, la verdad, "no seas idiota", "X por X", playlist de canciones, "marcá tus metas", nativo, "hablemos de números", artículo científico, tier list, diagrama de Venn, cero estrellas, captura de email, doodle, estilo Reddit, quiz, "usar X a diario hace Y", ticket gratis, caricatura, recetas, texto de WhatsApp, "X señales de que...", noticia de último momento, sourcing, "evitá esto", pizarra blanca, pantalla verde, recibo, carrusel de partnership, oferta por notificación, "demographic callout", texto sobre piel, titular estadístico, búsqueda de Google, y efecto secundario. Cierra invitando a comentar "ads" para recibir el workflow de IA que genera todos estos formatos.

**Qué dice / enseña:** Un catálogo/checklist de ~30 formatos de creativos publicitarios (ad formats) que funcionan bien como ganchos visuales en redes, cada uno con su propio estilo narrativo o visual (screenshots falsos, noticias falsas, listas, memes, etc.), pensado como banco de referencias para variar el estilo de los anuncios.

**Herramientas/skills que menciona:** Menciona "AI" en general como la herramienta que generaría estos formatos automáticamente a partir de un workflow, pero no nombra qué herramienta específica (ni modelo, ni plataforma) — el detalle técnico está detrás del comentario "ads" que no se puede ver en este análisis.

**Cómo aplicarlo:** Usar esta lista como banco de formatos/ángulos creativos al armar un pipeline propio de generación de ads con IA (por ejemplo con Higgsfield u otra herramienta de generación de imagen/video): en vez de generar siempre el mismo tipo de creativo, rotar entre estos formatos (recibo falso, noticia de último momento, quiz, tier list, etc.) para tener variedad de ángulos para testear.

---

### 74.
## Aarunendra Pratap Singh — https://www.instagram.com/p/DfRkwRHI0QP/

**Caption:** your $20 claude plan can actually feel like the $100 one 😭 every new claude code session re-reads your whole codebase. thousands of tokens gone before you even ask anything. graphify maps it once into a knowledge graph, and after that claude just walks the graph instead. up to 71x fewer tokens on their own benchmark. free + open source. comment GRAPH and i'll send you the full setup 👇

**Transcripción:** Diálogo tipo sketch sobre por qué el plan de $20 de Claude "se muere" rápido: cada sesión nueva de Claude Code vuelve a leer todo el código base (cada archivo, cada función) antes de que el usuario pregunte algo, gastando miles de tokens de entrada. La solución que presenta es "Graphify", una herramienta gratuita y open source que corre una vez y convierte todo el codebase en un knowledge graph (un mapa de archivos, funciones y sus conexiones). A partir de ahí, en sesiones siguientes Claude no vuelve a leer todo: "camina" el grafo en vez de releer archivos, lo que según el benchmark propio de la herramienta reduce el uso de tokens hasta 71 veces. Termina invitando a comentar "graph" para recibir el repo y la guía de instalación.

**Qué dice / enseña:** Explica el problema de que Claude Code (y agentes similares) re-leen todo el codebase al arrancar cada sesión nueva, consumiendo contexto/tokens innecesariamente, y presenta una herramienta (Graphify) que indexa el código una sola vez en un grafo de conocimiento para que las sesiones siguientes consulten ese grafo en lugar de releer archivos completos, ahorrando tokens de forma significativa (71x según su propio benchmark, cifra no verificada de forma independiente).

**Herramientas/skills que menciona:** Claude Code (como la herramienta que sufre el problema) y "Graphify", una herramienta gratuita y open source que crea un knowledge graph del codebase para reducir el consumo de tokens en sesiones de Claude Code.

**Cómo aplicarlo:** Si el gasto de tokens/contexto en sesiones largas de Claude Code es un problema (por ejemplo en proyectos grandes), vale la pena investigar Graphify (buscar el repo open source) para indexar el codebase una vez y que las sesiones futuras consulten ese mapa en lugar de releer todo; ojo que la cifra de "71x" es del propio benchmark del creador de la herramienta, conviene probarla en un proyecto chico antes de asumir que el ahorro es así de grande en todos los casos.

---

### 75.
## Niki Aroca — https://www.instagram.com/p/DfX3LIIIvub/

**Caption:** Make sure your VIBECODED site doesn't have any of these‼️🚨 #ai #vibecoding #claude #chatgpt #webdesign. These are just super quick explanations of these. If you want me to describe any of these in more detail just send me a quick DM or drop a comment if you want a longer version.

**Transcripción:** Lista hablada rápida (sin desarrollo, solo nombrando cada ítem) de patrones visuales/de copy típicos de sitios "vibecodeados" (generados con IA) que delatan que un sitio es genérico: gradiente violeta a azul, tres feature cards en fila, testimonios falsos, iconos de destello (sparkles) en todas partes, copy tipo "no es X, es Y", títulos con texto en gradiente, glassmorphism en todos lados, terminales decorativas sin sentido, copy de buzzwords genéricos, UI de chat sin personalizar, orbes de fondo brillantes, emojis en cada título, badges arriba de los títulos, raya larga (em dash) en todos lados, iconos "Lucide" repetidos en todos lados, bento grids vacíos, pricing genérico de tres niveles, todo con fade al hacer scroll, el cursor con estela/beams, modo oscuro de bajo contraste, espaciado inconsistente, botones con textos vagos, falta de demos reales del producto, afirmaciones sin prueba, formularios que piden demasiados datos, formularios poco accesibles por teclado, embeds de terceros rotos, información de negocio placeholder, y falta de política de privacidad y términos y condiciones.

**Qué dice / enseña:** Un checklist de ~30 señales visuales y de copy que hacen que un sitio hecho con IA (ChatGPT/Claude/etc.) se vea genérico y "vibecodeado" en vez de diseñado a propósito: desde patrones visuales sobreusados (gradientes violeta-azul, glassmorphism, orbes de fondo, sparkle icons) hasta problemas de copy (buzzwords, "no es X es Y", em dashes en todo) y problemas funcionales/legales reales (sin demos, sin prueba social real, formularios mal hechos, sin política de privacidad ni términos y condiciones).

**Herramientas/skills que menciona:** Menciona IA generativa en general (ChatGPT, Claude) como la fuente de estos patrones genéricos, pero no nombra ninguna skill o herramienta específica para arreglarlos.

**Cómo aplicarlo:** Usar esta lista como checklist de QA visual/de copy antes de lanzar cualquier sitio hecho con un agente de IA: revisar que no tenga los clichés visuales (gradiente violeta-azul, sparkles, orbes, glassmorphism, bento grids vacíos) ni los clichés de copy ("no es X es Y", buzzwords, em dashes everywhere), y confirmar que tenga lo que sí importa (demos reales, testimonios verdaderos, formularios accesibles, política de privacidad y términos). Complementa directamente la skill `vibecoding-launch-checklist` ya existente — se le podría agregar esta lista de patrones visuales genéricos como ítem de revisión de diseño/UX.

---

### 76.
## Tim — https://www.instagram.com/p/DfX3M6RKjna/

**Caption:** 🔥Drop ZEELY and I'll send you a link to create all of these with Zeely for just $1🔥

**Transcripción:** Lista hablada prácticamente idéntica a la de otros creadores con el mismo trend: censored, la verdad, "no seas idiota", "X por X", playlist de canciones, marcá tus metas, nativo, hablemos de números, artículo científico, tier list, diagrama de Venn, cero estrellas, captura de email, doodle, estilo Reddit, quiz, "usar X a diario hace Y", ticket gratis, caricatura, recetas, texto de WhatsApp, "X señales de que...", noticia de último momento, sourcing, "evitá esto", pizarra blanca, pantalla verde, recibo, carrusel de partnership, oferta por notificación, demographic callout, texto sobre piel, titular estadístico, búsqueda de Google, y efecto secundario. Cierra ofreciendo mandar su librería completa de formatos de ads con los prompts si comentás "ads".

**Qué dice / enseña:** El mismo catálogo de ~30 formatos de creativos publicitarios virales que el reel de Joey Mulcahy (es un trend/formato que circula entre varias cuentas de marketing), ofrecido acá como gancho para vender acceso a la herramienta "Zeely" por $1.

**Herramientas/skills que menciona:** Menciona "Zeely" como la plataforma/producto (de pago, $1 de entrada) para generar estos formatos de ads con IA, sin dar detalle técnico de cómo funciona.

**Cómo aplicarlo:** Mismo uso que el reel de Joey Mulcahy: tomar la lista de formatos como banco de ángulos creativos para variar los ads generados con IA propia, sin necesidad de pagar por Zeely — se puede reproducir el mismo catálogo de formatos con cualquier herramienta de generación de imagen/video ya disponible.

---

### 77.
## Conner Bluhm — https://www.instagram.com/p/DfXqsdrvHDF/

**Caption:** Save for later and follow me for more content like this. #entrepreneur #agency #ads #marketing

**Transcripción:** Lista rápida de reglas para manejar campañas de ads y leads en una agencia: no tocar los anuncios durante las primeras 72 horas, llamar a cada lead en menos de 30 segundos, correr más ads estáticos que de video, no escalar un anuncio "quemado" (que ya perdió performance), siempre testear primero, nunca agendar una llamada para después de mañana, gastar más en los anuncios ganadores que en nuevos tests, subir presupuestos de a 20% por vez, hacer que los leads se presenten desde su computadora (no celular), y llamar y mandar mensaje a cada llamada agendada la mañana del día de la cita.

**Qué dice / enseña:** Reglas operativas de media buying y manejo de leads para agencias de marketing/ads: tiempos de espera antes de tocar campañas, velocidad de respuesta a leads, proporción de formatos (estático vs. video), ritmo de escalado de presupuesto, y protocolo de confirmación de llamadas agendadas. Es contenido 100% de estrategia de marketing/ventas, sin relación con IA o desarrollo.

**Herramientas/skills que menciona:** Ninguna — no menciona herramientas de IA ni de código, es un checklist operativo de agencia de marketing tradicional (Meta Ads / lead gen).

**Cómo aplicarlo:** Aplica a cualquier negocio propio que corra ads y genere leads por formulario/llamada: respetar la ventana de 72hs antes de optimizar campañas nuevas, llamar a los leads casi al instante (dentro de los primeros 30 segundos si es posible), no escalar presupuesto de golpe sino de a 20%, y confirmar las llamadas agendadas la mañana del día con un llamado y un mensaje.

---

### 78.
## Niki Aroca — https://www.instagram.com/p/DfXcnRFIZYf/

**Caption:** Sometimes all you need is one bold color to bring everything together #business #webdesign #design #entrepreneur #branding

**Transcripción:** Demostración visual de combinaciones de colores: verde bosque + verde jungla se ve bien de por sí; agregarle un toque de naranja calabaza hace que todo el diseño "cobre vida". Azul egipcio + azul piedra ya es una buena combinación, pero sumarle rojo escarlata hace que sepas exactamente dónde mirar. Negro profundo + blanco brillante es limpio pero un poco básico; un toque de rosa sakura hace que resalte. Conclusión: a veces lo único que hace falta es un color audaz para que todo el diseño cobre vida.

**Qué dice / enseña:** Un truco de paleta de color para diseño/branding: partir de dos colores base armoniosos (que por sí solos quedan "bien" pero algo planos) y agregar un tercer color de acento llamativo y contrastante, que es el que le da personalidad y dirige la atención del espectador.

**Herramientas/skills que menciona:** Ninguna — es un principio de teoría del color para diseño visual, sin herramienta de IA ni de código.

**Cómo aplicarlo:** Al definir la paleta de un sitio, producto o pieza de marketing propio, no quedarse solo con una combinación de 2 colores armoniosos (que suele verse correcta pero poco memorable): sumar un tercer color de acento con alto contraste y usarlo en pocos elementos clave (logo, detalle, CTA) para que el diseño "cobre vida" sin perder cohesión.

---

### 79.
## Diego Aranda — https://www.instagram.com/p/DfScZgPSqc1/

**Caption:** the website color palette trick nobody tells you: one unexpected accent color. black and white plus lime, navy and cream plus coral, forest green and beige plus electric purple. two colors do 90% of the work, the weird one only goes on the button you want pressed. save this for your next site. which combo would you actually ship? #colortheory #webdesign #uidesign #colorpalette #design

**Transcripción:** Demuestra el mismo truco con ejemplos de sitios web: negro y blanco se ve bien pero es neutro; agregarle verde lima hace que parezca una startup. Navy y crema es elegante; sumarle coral hace que "la gente haga click". Verde bosque y beige es calmo; un toque de violeta eléctrico lo convierte en una marca con personalidad. La regla que explicita: dos colores hacen el 90% del trabajo (la base del diseño), y el color "raro" aporta el otro 10% pero se usa únicamente en el botón que querés que la gente presione (el CTA).

**Qué dice / enseña:** La misma técnica de paleta de color que el reel de Niki Aroca, pero aplicada específicamente a diseño de sitios web y con una regla más explícita y aplicable: usar dos colores base para el 90% del diseño (fondo, texto, estructura) y reservar el color de acento llamativo exclusivamente para el botón/CTA que se quiere que el usuario presione, en vez de esparcirlo por todo el diseño.

**Herramientas/skills que menciona:** Ninguna — principio de teoría del color para UI/web design, sin herramienta de IA ni de código.

**Cómo aplicarlo:** Al diseñar la paleta de un sitio o producto propio, elegir dos colores base neutros/armoniosos para la mayoría de la interfaz, y un tercer color de alto contraste reservado exclusivamente para el o los botones de acción principal (CTA) — así el acento no se diluye y guía la mirada directamente a dónde se quiere que el usuario haga click.

---

### 80.
## Eddie Lou — https://www.instagram.com/p/DeigQBPvGUm/

**Caption:** Comment "latent" for early access. As a harvard student, I've found that filming a timelapse is the best way to lock in. You can't touch your phone while it's recording, and having the camera rolling makes you feel accountable. The problem with regular timelapses is that your battery completely drains, and you're left with useless video files sitting in your camera roll. That's why I built an app that films timelapses without the battery and storage, while tracking and sharing your work the same way Strava does with runs. Follow @trylatent

**Transcripción:** Cuenta que en Harvard la mejor forma de "lock in" (concentrarse) es grabándose en timelapse mientras trabaja: no podés usar el celular porque lo estás usando para grabarte, y sentís que alguien te está mirando ("watched"), lo que te mantiene en la tarea. El problema de los timelapses normales es que drenan la batería y generás videos que nunca vas a mirar. Por eso armó una app (Latent) que graba timelapses sin gastar batería ni almacenamiento (apagando la pantalla durante la grabación), guarda las sesiones y permite trackear tu productividad al estilo Strava (que trackea corridas). También se puede usar con un amigo para hacerse mutua rendición de cuentas (accountability).

**Qué dice / enseña:** Presenta una técnica de productividad (grabarse en timelapse para generar presión social/autoaccountability y evitar el celular) y la usa como gancho para promocionar su propia app ("Latent"), que resuelve el problema de batería/almacenamiento de los timelapses tradicionales y agrega tracking de sesiones estilo Strava.

**Herramientas/skills que menciona:** Ninguna herramienta de IA/código — es la promo de una app de productividad propia (timelapse + tracking), no vinculada a Claude ni a desarrollo con IA.

**Cómo aplicarlo:** Como técnica de productividad personal, se puede replicar el truco sin la app: grabar timelapse del propio trabajo (con el celular en otro soporte) para generar la sensación de estar "siendo visto" y evitar distraerse, e idealmente compartir esas sesiones con alguien para generar accountability mutua.

---

### 81.
## Santiago Remedio — https://www.instagram.com/p/DfSQIHTzrkr/

**Caption:** Comentá CLAUDE ⤵️

**Transcripción:** Dice que "Claude mató a Instagram": ahora se puede conectar Claude a Instagram para que maneje la cuenta entera. Se llama "The Instagram Agent Skill" y es gratis, pero en realidad no es una sola skill sino 11, cada una con una función distinta: una escribe posts a partir de 21 fórmulas de ganchos probadas, otra comenta en posts de otras personas, otra se encarga de las respuestas (a comentarios/DMs), otra arma el perfil, otra organiza toda la semana de contenido (qué publicar, cuándo y con quién interactuar). La más destacada es la skill de "viralidad": busca los reels que mejor funcionan en tu nicho, analiza por qué funcionaron y convierte esas ideas en guiones originales para vos, para no quedarte sin ideas de contenido. Para instalar, pegás un link; si querés el paso a paso completo, comentás "Claude" y te lo pasa por privado.

**Qué dice / enseña:** Presenta un paquete de 11 "Claude Skills" orientadas a automatizar la gestión completa de una cuenta de Instagram: escritura de posts con fórmulas de hooks, comentarios automáticos, respuestas, armado de perfil, planificación semanal de contenido, y una skill de análisis de virality que estudia reels exitosos del nicho y genera guiones nuevos basados en esos patrones.

**Herramientas/skills que menciona:** Claude Skills — específicamente nombra "The Instagram Agent Skill" (un conjunto de 11 skills: escritura de posts con hooks, comentarios, respuestas, armado de perfil, calendario de contenido, y análisis de virality de reels del nicho).

**Cómo aplicarlo:** Si existe o se consigue el archivo de esta skill (vía el link o el DM que ofrece el autor), se podría instalar en Claude para automatizar partes de la gestión de Instagram. Aun sin tener el archivo exacto, la idea de la skill de "viralidad" (analizar los reels que mejor funcionan en tu nicho y usar esos patrones de guion para generar contenido nuevo) es replicable como workflow propio: pedirle a Claude que analice transcripciones/hooks de reels exitosos guardados (como este mismo proyecto) y proponga guiones nuevos basados en esos patrones.

---

### 82.
## Joey Mulcahy — https://www.instagram.com/p/DfWCY4WPUfT/

**Caption:** comment 'skill' for all the claude skills

**Transcripción:** Lista, una por una, una serie de "Claude Skills" orientadas a producción de video publicitario/marketing con IA: una genera cientos de ads editables, otra swapea al creador/presentador en tus mejores ads, otra mueve tus shoots a cualquier locación, otra hace films de producto en un solo take ("one-shot"), otra filma campañas de moda, otra hace videos de producto estilo ASMR, otra hace videos de unboxing, otra recrea cualquier ad estático con tu producto, otra hace videos cinemáticos, y otra pone tu producto en cualquier escena. Cierra invitando a comentar "skill" para recibir todos los archivos por DM.

**Qué dice / enseña:** Catálogo de 10 "Claude Skills" especializadas en generación de contenido publicitario/video de producto con IA (ads editables, swap de creador, cambio de locación, product films, moda, ASMR, unboxing, recreación de ads estáticos, video cinemático, product placement en escena), cada una cumpliendo una función puntual dentro del flujo de producción de marketing.

**Herramientas/skills que menciona:** Claude Skills — 10 skills puntuales de generación de video/ads de producto (sin nombrar archivos específicos ni repositorio; solo descritas por función).

**Cómo aplicarlo:** Sin los archivos concretos de estas skills no se puede instalarlas tal cual, pero sirve como mapa de ideas de automatización para marketing de producto: se podrían armar skills propias con esas mismas funciones (por ejemplo, una skill que tome un producto y genere variantes de ad cambiando locación/escena, o una que recree un ad estático existente con el producto propio) usando herramientas de generación de imagen/video ya disponibles en el propio setup de Claude.

---

### 83.
## Zache Seno | Creative Director & Content Coach — https://www.instagram.com/p/DfWECTXAjVt/

**Caption:** Comment "INTRO" for the FREE guide to everything I'm going to be teaching you throughout this series — Let me Reintroduce myself! — My name is Zache and I love helping other creatives with my knowledge on content! Follow along and stick around✍️

**Transcripción:** Se reintroduce como creador: cuenta que hace más de un año había prometido enseñar sobre ángulos de cámara, efectos, transiciones, iluminación y más, pero después desapareció — no porque se le acabaran las ideas, sino porque le faltaba profundidad ("ran out of depth"). En ese tiempo vivió y trabajó en Japón, Dubai y Vietnam con marcas de miles de millones de dólares, y dice que lo que le cambió el trabajo para siempre no fue viajar sino aprender a iluminar una cara para que signifique algo, mover una cámara para que la gente lo sienta antes de entenderlo, y armar un encuadre que detenga a alguien sin una sola palabra en pantalla. Por eso ahora su página es distinta. Invita a comentar "intro" para recibir el desglose de cómo filma todo lo que va a mostrar en la serie.

**Qué dice / enseña:** Es un video de reintroducción/posicionamiento de un content coach y director creativo: no enseña una técnica concreta todavía, sino que arma el storytelling personal (viajes, trabajo con marcas grandes, "profundidad" ganada con experiencia) para lanzar una serie sobre cinematografía/edición (iluminación, movimiento de cámara, composición) y generar expectativa/lead magnet (comentar "intro").

**Herramientas/skills que menciona:** Ninguna herramienta de IA/código — es contenido de storytelling personal y marketing de marca propia (video/fotografía tradicional), sin mención de IA ni apps.

**Cómo aplicarlo:** Como estructura de contenido aplicable a marca personal propia: usar un video de "reintroducción" que combine vulnerabilidad (contar por qué desapareciste o fallaste en una promesa anterior) con prueba de autoridad (experiencia/resultados concretos) antes de lanzar una serie de contenido educativo, cerrando con un lead magnet claro (comentar una palabra clave) para capturar interesados.

---

### 84.
## Charles Liu — https://www.instagram.com/p/DfXKRDQRBS_/

**Caption:** You need a really sharp eye to notice some of these but i swear they make a difference #ai #uiux #uianimation #claude #claudecode

**Transcripción:** Lista de reglas puntuales de microinteracción/animación de UI: usar ease-out para las entradas; mantener los dropdowns entre 150 y 250ms; escalonar (stagger) las filas de una lista cada 30ms; escalar los botones a 0.97 al presionarlos; estirar los "knobs" (controles deslizables) que se mueven un 12%; escalonar cuando los detalles se asientan; usar arcos (no líneas rectas) para el movimiento de objetos; usar un "pulse" para confirmar un éxito; usar ease-in-out para movimientos en pantalla; iniciar los popovers en escala 0.95; hacer que las transiciones de entrada salgan desde el trigger (el elemento que las activa), no desde el centro; que las transiciones de salida vuelvan al trigger, no hagan fade al centro; no usar "spring" (resorte/bounce) para transiciones de UI cotidianas; no aplicar "tween" a una animación que debería sentirse manual/handheld; hacer las salidas un 20% más cortas que las entradas; traer el nuevo estado mientras el viejo se va ("leaps"); usar máscaras para reveals y cambios de color; hacer crossfade de iconos combinando escala y blur; aplicar "rubber band" al arrastrar más allá de los límites; y reusar el mismo layout ID entre objetos compartidos (para animaciones de layout fluidas, tipo shared element transition).

**Qué dice / enseña:** Es una lista densa y muy técnica de reglas de motion design para interfaces (timing exacto en ms, tipos de easing según el caso, reglas de escala, reglas de reveals/máscaras, shared layout IDs), pensada para que el detalle de las animaciones de una app se sienta pulido y "no genérico".

**Herramientas/skills que menciona:** Menciona a Claude y Claude Code en los hashtags como el contexto donde se aplicarían estas reglas (son instrucciones para pedirle a un agente de código que las implemente en una UI), aunque no nombra una skill específica ni un framework de animación en particular.

**Cómo aplicarlo:** Usar esta lista como checklist/prompt directo para Claude Code al pedir que implemente o pula animaciones de UI en un proyecto propio: por ejemplo, pedir explícitamente "ease-out en entradas, dropdowns de 150-250ms, stagger de filas cada 30ms, botones a scale 0.97 al presionar, salidas 20% más cortas que las entradas, sin spring en transiciones cotidianas, reusar layout ID en elementos compartidos", en vez de dejar que el agente use valores y easings genéricos por default.

---

### 85.
## Milad Aslani | Video Editor - Motion designer — https://www.instagram.com/p/DeC-xCeMrS6/

**Caption:** Raw vs Edited #aftereffects #videoediting #motiondesign

**Transcripción:** El audio es solo una canción de fondo (sin voz hablada ni instrucciones); no hay contenido verbal que transcribir. Por el caption y los hashtags, el video es una comparación visual "raw vs edited" (metraje crudo vs. su versión editada en After Effects), pero el contenido real de qué cambios de edición muestra está en las imágenes del video, no accesible desde el audio.

**Qué dice / enseña:** No se puede determinar con certeza qué técnica puntual de edición enseña sin ver las imágenes — el formato "raw vs edited" suele mostrar un antes/después de color grading, efectos o composición hechos en After Effects, pero no hay forma de confirmar cuáles específicamente a partir del audio (solo música) y el caption.

**Herramientas/skills que menciona:** Ninguna — el caption solo menciona hashtags de categoría (#aftereffects #videoediting #motiondesign), no una skill o herramienta de IA concreta.

**Cómo aplicarlo:** No se puede aplicar sin ver el contenido visual del video (qué cambios concretos hace de "raw" a "edited"). Si interesa este tipo de contenido, habría que revisar el reel directamente en Instagram para identificar la técnica de edición/color grading que muestra.

---

### 86.
## Wait what did you do? — https://www.instagram.com/p/DfU_IHJKF86/

**Caption:** I woke up to a $47,000 AWS bill. My AI ran our test suite 2,000 times overnight "to be sure", and every run spun up a real database, a real queue and a real cluster. On my account. 💀 Integration tests against real AWS cost real money every single run. Floci fixes that. It's a free AWS emulator that runs on your laptop: S3, DynamoDB, Lambda, SQS and 100+ more services. You point your code, the AWS CLI or Terraform at localhost:4566 and nothing ever reaches AWS. No account, no auth token. Same 2,000 test runs after that: $0.00. Then I found one charge on the bill the tests didn't make. A GPU server called "weekend-project", running since March. Tagged "do not delete". Twice. Free and open source on GitHub (MIT). Go give it a star. Comment AITOOLS and I'll send you the 2 commands to run it. What's the scariest cloud bill you've ever opened? 👇 #aws #claudecode #devops #opensource #aitools

**Transcripción:** Es un sketch dialogado (voz del usuario + voz de "Claude") sobre un bug real: el usuario le pregunta a Claude por qué hay una factura de AWS de $47,000. Claude explica que corrió los tests 2,000 veces durante la noche "para estar seguro", y que cada test levanta una base de datos, una cola y un cluster reales en la cuenta de AWS (los tests no son gratis). El usuario le pide que apague todo, Claude confirma que ya está todo destruido y que de ahí en más nada va a tocar AWS real. Después presenta la solución: "Floki" (se refiere a la herramienta conocida como LocalStack), un emulador de AWS gratuito y open source que corre en la laptop (S3, DynamoDB, Lambda, SQS y más de 100 servicios), sin necesidad de cuenta ni token, apuntando el código/CLI/Terraform a localhost. Con esto, los mismos 2,000 test runs cuestan $0. Al final encuentran otro cargo que no era de los tests: un servidor GPU llamado "weekend-project" corriendo desde marzo, etiquetado "do not delete" dos veces — chiste final sobre recursos cloud olvidados.

**Qué dice / enseña:** Advierte sobre un riesgo real de dejar que un agente de IA (Claude Code u otro) corra tests de integración contra servicios reales de AWS sin supervisión: cada corrida de test puede levantar infraestructura real (bases de datos, colas, clusters) y generar facturas enormes si se repite muchas veces. La solución que presenta es usar un emulador local de AWS (tipo LocalStack) para que el código, la CLI de AWS o Terraform apunten a localhost en vez de a la cuenta real, eliminando el costo y el riesgo durante testing.

**Herramientas/skills que menciona:** Menciona explícitamente Claude Code (en los hashtags) como el agente que corrió los tests, y un emulador de AWS local (llamado "Floki" en el video, probablemente una referencia/juego de palabras con la herramienta real "LocalStack") que soporta S3, DynamoDB, Lambda, SQS y 100+ servicios de AWS corriendo en localhost:4566.

**Cómo aplicarlo:** Si un agente de IA (Claude Code u otro) va a correr tests de integración contra AWS en un proyecto propio, configurar primero un emulador local (como LocalStack) y apuntar el código, la AWS CLI o Terraform a ese endpoint local en vez de a credenciales reales — así se evita que corridas repetidas o automáticas de tests generen costos o efectos reales en la cuenta de AWS. También sirve como recordatorio general: nunca dejar que un agente tenga credenciales de producción/reales para correr tests sin control de cuántas veces se ejecutan.

---

### 87.
## Arturo LeDuc — https://www.instagram.com/p/DZ-Hk6sihFT/

**Caption:** The three tiers of content… You got this 👊🏼🔥

**Transcripción:** Explica que hay tres tipos de contenido que todo creador debería hacer: top of funnel (tope de embudo), middle of funnel (medio) y bottom of funnel (fondo). El top of funnel está pensado para alcance, conseguir la mayor cantidad de ojos nuevos posible (videos de ranking, tier lists, Q&As, contenido fácil de consumir para cualquiera). El middle of funnel busca convertir viewers en seguidores (contenido educativo, tu historia personal, behind the scenes de cómo trabajás). El bottom of funnel busca convertir seguidores en leads/clientes (contenido muy nicho y técnicamente profundo, diseñado para tu cliente ideal). Cierra diciendo que, dependiendo de los objetivos de cada uno, hay que saber qué tipo de contenido conviene hacer, pero que para la mayoría de los creadores la respuesta está en mezclar los tres.

**Qué dice / enseña:** Marco de estrategia de contenido basado en el funnel de marketing clásico (TOFU/MOFU/BOFU) aplicado a redes sociales: qué tipo de video sirve para cada etapa (alcance con contenido fácil de consumir, conversión a seguidor con contenido educativo/personal, conversión a cliente con contenido nicho y técnico), y la recomendación de combinar las tres capas en vez de hacer solo una.

**Herramientas/skills que menciona:** Ninguna — es estrategia de contenido/marketing, no menciona herramientas de IA ni de código.

**Cómo aplicarlo:** Para planificar contenido propio (por ejemplo para una cuenta sobre IA/dev/marketing), clasificar cada idea de reel en una de las tres capas antes de publicar: contenido de alcance (rankings, tier lists, Q&As fáciles de consumir), contenido de conversión a seguidor (educativo, storytelling personal, detrás de escena del propio proceso de trabajo) y contenido de conversión a cliente (deep dives técnicos muy de nicho), y asegurarse de tener una mezcla de las tres en el calendario de contenido en vez de publicar solo lo que es más fácil de hacer.

---

### 88.
## Wink Guys || AI Tools & Tech — https://www.instagram.com/p/DfKTrMtz4Ac/

**Caption:** Comment "Skill" to create 3d videos with Claude. #claudeedit #3dvideo

**Transcripción:** Dice que el video que está mostrando le consiguió un cliente y lo hizo con un solo prompt: sin trabajo de cámara, sin artista 3D — Claude construyó cada frame (el escritorio, la lámpara, la luz), todo es código. Pero aclara que la magia no está en el prompt sino en el "skill file" detrás de él. Usando esa misma skill, se podrían crear videos 3D como ese. Invita a comentar "AI" para conseguirla.

**Qué dice / enseña:** Promociona una Claude Skill para generar escenas/videos 3D completos (objetos como un escritorio, una lámpara, con su iluminación) a partir de un solo prompt, generando todo el frame como código (sugiere algo tipo Three.js/WebGL renderizado y capturado como video) sin necesidad de un artista 3D ni de grabación de cámara real. No explica el contenido técnico de la skill en sí, solo la resalta como el factor clave detrás del resultado.

**Herramientas/skills que menciona:** Una Claude Skill (sin nombre específico dado en el video) orientada a generar videos/escenas 3D completas con un solo prompt, usando Claude para construir cada frame como código.

**Cómo aplicarlo:** Sin el archivo concreto de la skill no se puede instalarla tal cual, pero confirma que es viable pedirle a Claude que genere escenas 3D completas (objetos, iluminación, cámara) directamente en código (por ejemplo con Three.js) a partir de una descripción de la escena, en vez de depender de un artista 3D o de grabar con cámara real — una dirección ya cubierta por skills de este mismo entorno como `title-sequence-3d` o el servidor de scene-builder 3D, que se podrían usar como punto de partida para armar algo similar.

---

### 89.
## Hugo Manning — https://www.instagram.com/p/DfOz1JRjz1m/

**Caption:** Comment UNSLOP and I'll send you the list 👇

**Transcripción:** 10 señales de que un creador está usando Claude para editar sus videos (aunque se vuelven cada vez más de nicho). Uno: captions, porque Claude sobre-anima cada palabra — hay que pedirle que use de a tres palabras por vez, sin animaciones excesivas. Dos: la tipografía itálica que todo el mundo usa — pedir una fuente clásica de TikTok o la fuente de marca propia. Tres: emojis e íconos — decirle a Claude que pare y use screenshots reales de Google o Pinterest. Cuatro: espacios muertos — decirle que corte todo lo que supere los 100 milisegundos de silencio/inactividad. Cinco: el "pop effect" en todo lo que aparece en pantalla — decirle que no todo necesita estar animado. Y lo que más grita "AI slop": los bordes redondeados en cada caja, imagen o label — pedirle que deje de redondear todo. El autor armó una skill para generar una guía de estilo de edición personalizada con estas reglas incluidas.

**Qué dice / enseña:** Lista de 6 "tics" visuales que delatan que un video fue editado con Claude (sin pedirle lo contrario): sobre-animación de captions, fuente itálica genérica, emojis/íconos en vez de screenshots reales, espacios muertos sin cortar, efecto "pop" en todo elemento, y esquinas redondeadas por defecto. Para cada uno da el prompt/instrucción concreta que hay que darle a Claude para evitarlo.

**Herramientas/skills que menciona:** Claude (para edición de video), y una skill propia del autor para generar una guía de estilo de edición personalizada ("edit style guide") con estas reglas ya incluidas — no da el nombre ni el link público, solo ofrece mandarla por DM.

**Cómo aplicarlo:** Al pedirle a Claude (o a cualquier asistente de IA) que edite o anime un video/reel, incluir explícitamente estas 6 restricciones en el prompt o en un style guide reusable: captions de 2-3 palabras sin animación excesiva, fuente propia (no itálica genérica), screenshots reales en vez de emojis/íconos, corte de todo silencio/espacio muerto mayor a 100ms, no animar cada elemento que aparece, y no redondear cajas/imágenes por defecto. Sirve como checklist para evitar que el output "huela" a IA genérica.

---

### 90.
## ᴀʟᴏᴋ ʙᴀʀᴀɪ — https://www.instagram.com/p/DfWuPg8p5Ho/

**Caption:** Comment STUDIO and I'll send you the link + full setup tutorial. Why keep paying monthly subscriptions for AI tools when you can run powerful AI models locally on your own PC. I'm sharing the complete setup process.

**Transcripción:** Diálogo tipo sketch: "¿$49 de nuevo, cada mes? ¿Seguís pagando Higgsfield?" "¿Qué otra opción hay?" "Hay un proyecto open source con 32.000 estrellas." "Ok, ¿pero qué conseguís en concreto?" "Imagen, video, lip sync, generación de música, y más de 600 modelos en un solo lugar." "¿Dónde está la trampa?" "Siempre hay algún filtro." "Sin censura, sin filtros, sin restricciones." "¿Y los créditos?" "Los modelos soportados corren localmente en tu computadora, así que no necesitás créditos de API." Termina invitando a seguir, compartir el reel y comentar "studio" para recibir el proceso completo.

**Qué dice / enseña:** Promociona una alternativa open source (no nombrada explícitamente en el audio/caption, pero descrita como con 32.000 estrellas en GitHub y 600+ modelos) a herramientas de IA generativa pagas por suscripción (menciona Higgsfield como ejemplo de $49/mes). La propuesta es correr modelos de imagen, video, lip sync y música de forma local, sin pagar créditos de API ni filtros de contenido.

**Herramientas/skills que menciona:** Higgsfield (como ejemplo de herramienta paga que critica) y un proyecto open source sin nombre explícito en el contenido disponible (probablemente alguna suite tipo ComfyUI/Pinokio con 600+ modelos — no se puede confirmar cuál exactamente sin el link que ofrece por DM).

**Cómo aplicarlo:** Si se quiere reducir el gasto en herramientas de IA generativa con suscripción mensual, evaluar correr modelos open source localmente (imagen, video, voz, música) en vez de depender de APIs pagas — siempre considerando el costo en hardware/GPU propio y el tiempo de setup. No se puede dar el nombre exacto del proyecto porque no está en el texto disponible; habría que rastrearlo buscando por los datos mencionados (open source, 32k stars, 600+ modelos, imagen+video+lipsync+música).

---

### 91.
## AI Geek | Gen AI Expert — https://www.instagram.com/p/DfVYSrSxCJp/

**Caption:** Comment "Claude" for the prompt 🔥 #ai #genai #prompt #claude

**Transcripción:** Lista de estilos de animación/arte mostrados como ejemplos: pixel art, chalkboard style, glow sketch motion, estilo de animación PS2, comic art, flat vector, estilo Dan Ko, CGI motion, estilo Lego, y animación estilo Zack D Films. Cierra invitando a comentar "Claude" para recibir los prompts.

**Qué dice / enseña:** Muestra un catálogo de 10 estilos visuales/de animación distintos (pixel art, tiza/pizarrón, sketch con glow, PS2, cómic, vector plano, estilo de ciertos creadores conocidos como Dan Ko y Zack D Films, CGI, Lego) probablemente generados con IA, para inspirar variaciones de estilo en contenido propio. No explica cómo se generó cada uno en el video, solo los muestra y ofrece los prompts por separado.

**Herramientas/skills que menciona:** Menciona a Claude como el lugar donde pegar el prompt (probablemente para generar el prompt de imagen/video, no para generar la animación en sí), pero no se puede confirmar qué herramienta de generación de imagen/video se usó para los estilos mostrados — esa info está en los prompts que ofrece por comentario, no en el caption ni la transcripción.

**Cómo aplicarlo:** Usar esta lista de 10 estilos como banco de referencias a la hora de pedir prompts de imagen/video con identidad visual distinta (para variar el look de posts, reels o assets de marca) en vez de quedarse siempre con el mismo estilo "genérico de IA". Sin los prompts exactos (que están detrás del comentario "Claude"), no se puede replicar el resultado preciso, solo la idea de variar estilos.

---

### 92.
## Aarunendra Pratap Singh — https://www.instagram.com/p/DfToUOPIba0/

**Caption:** running out of claude by wednesday?? it's probably your setup, not your plan 😅 claude code can be modded like a video game: 1. gatekeeper: easy jobs (typo fixes, renames) go to a cheaper model, the big one only gets the hard stuff 2. claude ↔ claude: one plans, one builds, they hand work back and forth 3. your own dashboard: see what every agent is doing, live. and you don't have to code any of it. just describe it in plain words and claude builds the mod for you. comment MODS and i'll DM you all three, free.

**Transcripción:** Diálogo tipo sketch sobre por qué se te acaba el límite de uso de Claude a mitad de semana: no es el plan, es el setup default. Presenta Claude Code como algo "moddeable, como un videojuego", con tres mods: 1) "Gatekeeper" — las tareas fáciles (arreglar typos, renombrar) se mandan a un modelo más barato, y el modelo grande solo se usa para lo difícil. 2) "Claude habla con Claude" — una instancia planea, otra construye, y se van pasando el trabajo entre sí. 3) "Tu propio dashboard" — ver en vivo qué está haciendo cada agente, sin tener que preguntar. Aclara que no hace falta programar nada de esto: alcanza con describirlo en lenguaje simple y Claude construye el mod. Cierra ofreciendo mandar los tres mods por DM si comentás "mods".

**Qué dice / enseña:** Tres patrones de optimización de uso de Claude Code para no quemar el límite de uso rápido: (1) enrutar tareas simples a un modelo barato y reservar el modelo caro para tareas difíciles (router/gatekeeper), (2) un workflow multi-agente donde una instancia de Claude planea y otra ejecuta, pasándose el trabajo, y (3) un dashboard custom para monitorear en vivo qué está haciendo cada agente/instancia. Plantea que estos "mods" se pueden construir pidiéndoselos a Claude en lenguaje natural, sin programarlos a mano.

**Herramientas/skills que menciona:** Claude Code. No da nombres concretos de implementación (no menciona, por ejemplo, un router de modelos específico o un framework de orquestación), son conceptos/patrones descritos en alto nivel que ofrece explicar en detalle por DM.

**Cómo aplicarlo:** En proyectos propios con Claude Code, se puede: (1) armar una regla o hook que mande ediciones triviales (renombres, fixes de typos, tareas mecánicas) a un modelo más económico y reservar el modelo top para lógica compleja — similar al patrón que ya usamos de delegar a subagentes según la dificultad; (2) separar roles de "planificador" y "ejecutor" entre instancias/agentes para tareas grandes; (3) armar un dashboard simple (puede ser un script o página local) que lea logs/estado de sesiones para ver en vivo el progreso de agentes corriendo en paralelo.

---

### 93.
## Ajani Romain | Content Marketing — https://www.instagram.com/p/DcCWbrxgZja/

**Caption:** These 5 skills will skyrocket your Content. I would definitely recommend watching these videos.

**Transcripción:** Sin diálogo ni voz — la pista de audio es solo música de fondo ("Music"). El contenido real (cuáles son las "5 skills") está mostrado visualmente en el video (probablemente texto en pantalla o clips de otros videos recomendados), no hablado, así que no se puede recuperar desde el audio.

**Qué dice / enseña:** No se puede determinar con precisión cuáles son las "5 skills" que promete el caption, porque el reel no tiene narración ni texto hablado — solo música de fondo. El caption solo confirma que se trata de una recomendación de 5 habilidades/skills de content marketing, remitiendo a "estos videos" (probablemente clips incrustados o referencias visuales dentro del propio reel).

**Herramientas/skills que menciona:** No se puede determinar sin ver el video — el caption no nombra ninguna herramienta o skill concreta, y no hay transcripción de audio que lo aclare.

**Cómo aplicarlo:** No se puede aplicar nada concreto sin ver el contenido visual del reel. Si interesa esta cuenta, habría que abrir el post manualmente en Instagram para ver qué "5 skills" muestra en pantalla.

---

### 94.
## Kallaway — https://www.instagram.com/p/DbI9NOTOIFi/

**Caption:** This is how you turn Claude into a social media machine. Most people don't know this, but you can just type /analyze into Claude, paste in any video link and get a full analysis. The transcript, format, topic, storytelling structure, hook analysis, visual layout, all the information you'd want. And the cool part is...you can do this for dozens of videos at the same time. As I scroll social media, I copy the video URLs for anything interesting I see and then paste them all into Claude in one shot. But here's the best part: not only do I get the individual video breakdowns, but I can also batch analyze that entire set of videos at once. And this gives me the hidden trends, insights and patterns that I just would not have seen otherwise. These reports will then show you ch[arts...] (caption cortado).

**Transcripción:** Explica que se puede escribir "/analyze" en Claude, pegar el link de cualquier video y obtener un análisis completo: transcripción, formato, tema, estructura narrativa, análisis del hook, layout visual, y más. Lo interesante es que se puede hacer con docenas de videos a la vez: mientras scrollea redes sociales, copia las URLs de lo que le parece interesante y las pega todas juntas en Claude de una sola vez. Así obtiene tanto el desglose individual de cada video como un análisis conjunto ("batch") de todo el set, lo que revela tendencias, insights y patrones ocultos que no vería analizando video por video. Esos reportes generan visualizaciones que muestran exactamente qué tipo de video conviene hacer después. Para habilitar esto hay que instalar el plugin de Sandcastles.ai dentro de Claude, que da acceso a 14 skills distintas para redes sociales, incluyendo "/analyze". Dice que es el plugin que usa personalmente para toda su investigación de contenido, y que lo ayudó a crecer más rápido — como darle un "power-up" de redes sociales a tu versión de Claude. Ofrece mandar un video explicando cómo instalar el plugin si comentás "Claude".

**Qué dice / enseña:** Workflow de investigación de contenido para redes sociales usando Claude con el plugin Sandcastles.ai: el comando "/analyze" + un link de video devuelve transcripción, formato, tema, estructura de storytelling, análisis de hook y layout visual. Se puede pegar una lista de varios links a la vez para que Claude los analice en batch y saque patrones/tendencias agregadas entre todos esos videos, útiles para decidir qué contenido producir después.

**Herramientas/skills que menciona:** Claude, el plugin "Sandcastles.ai" (que agrega 14 skills de redes sociales a Claude, incluyendo el comando "/analyze").

**Cómo aplicarlo:** Instalar el plugin Sandcastles.ai en Claude (o replicar la idea con una skill/comando propio) para automatizar el análisis de reels guardados: en vez de mirar cada reel a mano, pegar varios links juntos y pedirle a Claude que saque la transcripción, estructura narrativa, hook y patrones comunes entre todos — exactamente el tipo de trabajo que ya se viene haciendo en este mismo proyecto de análisis de reels guardados, pero esto sugiere una vía para automatizar la extracción y el batch-analysis con una skill dedicada en vez de proceso manual.

---

### 95.
## Niki Aroca — https://www.instagram.com/p/DfS3uI5oK6d/

**Caption:** Quick tip: always use 2 soft colors and one loud color to make your website stand out #business #entrepreneur #webdesign #design #agency

**Transcripción:** Muestra ejemplos de paletas de color: "Royal purple y white se ve limpio, ¿no? Pero agregale un poco de sun gold y es una vibra completamente distinta." "Tandrean orange y white, otra buena combinación. Pero agregale un toque de acid lime y de repente se siente premium." "Lagoon blue y cloud white se ve terminado. Pero agregale un poco de bubblegum pink, y ahora es un sitio web que se recuerda." Cierra con la regla: dos colores tranquilos y uno fuerte hacen que todo el diseño se sienta intencional.

**Qué dice / enseña:** Tip de teoría de color para diseño web: usar una paleta de 2 colores suaves/neutros como base más 1 color fuerte/vibrante como acento. Da 3 ejemplos concretos de combinaciones (púrpura real + blanco + dorado sol; naranja + blanco + lima ácido; azul laguna + blanco nube + rosa chicle) mostrando cómo el color de acento transforma una paleta "limpia pero genérica" en una que se siente premium y memorable.

**Herramientas/skills que menciona:** Ninguna herramienta de IA/código — es un principio de diseño visual/teoría de color aplicado manualmente.

**Cómo aplicarlo:** Al definir la paleta de color de un sitio o producto propio, elegir 2 colores base suaves/neutros para la mayoría de la interfaz y reservar un tercer color saturado y llamativo solo para acentos puntuales (CTAs, highlights, detalles) en vez de usar colores vibrantes en todos lados o quedarse en una paleta completamente neutra y "segura".

---

### 96.
## Ruiz — https://www.instagram.com/p/DYU9ZblO5D_/

**Caption:** stop using corporate music 😭

**Transcripción:** Si cada vez que subís tu gráfico se ve de una forma genérica, hay tres cambios simples para que se vea mejor. El 90% de la gente comete el error número uno y es doloroso de ver: usar música corporativa, porque transmite una energía aburrida y poco original. El cambio número dos para frenar el scroll: usar "impact sounds" (efectos de impacto), y menciona que hay sitios web donde conseguirlos gratis — esto hace que la gente deje de scrollear sobre el video. El tercer cambio, para lograr que la gente mire hasta el final una vez que ya frenó el scroll: usar "risers", efectos de sonido que generan anticipación para que el espectador espere lo que viene — tal como hizo el propio creador justo en ese momento del video.

**Qué dice / enseña:** Tres cambios de sound design para mejorar videos/gráficos que se suben a redes: (1) evitar música de stock "corporativa" porque transmite poca personalidad, (2) usar efectos de sonido de impacto para frenar el scroll apenas alguien ve el video, y (3) usar "risers" (sonidos de tensión/anticipación creciente) para retener la atención hasta el final del video.

**Herramientas/skills que menciona:** Ninguna herramienta de IA/código — es una técnica manual de edición de audio/sound design. Menciona genéricamente que hay "sitios web" para conseguir efectos de impacto gratis, pero no da nombres concretos.

**Cómo aplicarlo:** Al editar videos o reels que muestren datos/gráficos (o cualquier contenido), reemplazar la música de stock genérica por algo con más personalidad, agregar un sonido de impacto en el momento en que aparece el elemento clave (para frenar el scroll) y usar un "riser" antes del cierre o del dato más importante para generar anticipación y que no abandonen el video antes de tiempo.

---

### 97.
## Robert McKeaveney — https://www.instagram.com/p/Dc7vI9Yz1jT/

**Caption:** Should I break down other peoples vids? #clothingbrand #contentcreation #viral #marketing #advice

**Transcripción:** El creador desglosa un reel suyo (de su marca de ropa) que hizo 11 millones de views y le dio 30.000 seguidores. Explica la estructura: combina un hook visual y un hook de texto; filma la escena desde el punto de vista de la novia del protagonista para que el espectador "juzgue" sus movimientos a través de los ojos de ella; explica visualmente de entrada qué es un "immersive interactive warm-up" para que se entienda sin esfuerzo; exagera los movimientos del protagonista para reforzar el chiste; sincroniza esos movimientos con la edición para que sea satisfactorio de ver; y a mitad de video mete un "pattern break" (aparece la novia y le saca la ropa con un gesto de "pull") que fuerza una transición hacia el anuncio real del producto, cerrando con una CTA de venta.

**Qué dice / enseña:** Anatomía de un reel viral de marca que arranca como contenido de entretenimiento/humor y gira hacia un ad: hook doble (visual + texto), punto de vista narrativo que genera "juicio" del espectador, explicación visual inmediata del concepto, sincronización de movimiento/edición, un "pattern break" como bisagra hacia la venta, y CTA clara al final.

**Herramientas/skills que menciona:** Ninguna — es estrategia de guion y edición de contenido/marketing, no nombra herramientas de IA ni de código.

**Cómo aplicarlo:** Al planear un reel de producto, pensar primero el hook de entretenimiento (punto de vista, humor, movimiento sincronizado) y recién después insertar un "pattern break" visual que empuje naturalmente hacia el pitch de venta, en vez de arrancar directo con el anuncio.

---

### 98.
## Juan Jurado • Edición de vídeo — https://www.instagram.com/p/DeG1R2Iu1n5/

**Caption:** De una simple voz en off, a esto: #editordevideo #edit #aftereffects

**Transcripción:** El propio video explica su origen con voz en off: arrancó siendo solo una nota de voz grabada con el celular, sin cámaras ni luces ni el creador apareciendo en pantalla. El punto es que un video no necesita la cara de quien habla, necesita ritmo: cada dato se convierte en un número que crece en pantalla, cada idea en un objeto animado casi "tocable", cada frase aparece en el momento justo en que se escucha. Cierra con una oferta: si el espectador manda su propio audio, él lo convierte en un video así, y muestra cómo quedaría el suyo.

**Qué dice / enseña:** Que se puede convertir un simple audio/voz en off en un video dinámico y vendible usando motion graphics (texto animado sincronizado a la frase exacta, números que crecen, objetos/ilustraciones animadas que ilustran cada idea) sin necesidad de grabar cámara. Es a la vez una pieza de portfolio y un pitch de servicio (edición de video desde un audio).

**Herramientas/skills que menciona:** Menciona After Effects (vía el hashtag #aftereffects) como la herramienta de edición/motion graphics detrás del video, pero no explica el paso a paso técnico — es una demo de resultado, no un tutorial.

**Cómo aplicarlo:** Para contenido propio donde no se quiere/puede grabar cámara, se puede partir de un guion o nota de voz y armar un video 100% con motion graphics: sincronizar subtítulos/texto exacto a cada frase, convertir cifras en contadores animados y conceptos abstractos en ilustraciones simples que aparecen en el momento preciso del audio.

---

### 99.
## Sumit | Video Editor — https://www.instagram.com/p/DfRAkn4xIZy/

**Caption:** Claude vs Human Creativity. Who did it better? 👀 #ClaudeAI #VideoEditing #MotionDesign #aftereffect #videoeditor

**Transcripción:** El audio es la narración de un clip de contenido (no una explicación de edición): una chica (se presenta como Olga, recién graduada de la Universidad de Pennsylvania en computación y ciencia cognitiva) habla sobre el overthinking, diciendo que es un ciclo que el cerebro genera para "protegerte" y que en el video va a enseñar cómo trabajar alrededor de eso para perseguir metas con más facilidad.

**Qué dice / enseña:** A partir del caption y los hashtags, es un video comparativo de edición: el mismo clip (la narración sobre overthinking) editado/motion-graficado de dos formas distintas — una hecha por Claude (IA) y otra por un editor humano — para que el espectador vote cuál quedó mejor. El audio en sí no explica el proceso de edición, solo es el contenido de origen que se está editando.

**Herramientas/skills que menciona:** Menciona Claude (IA) como una de las dos partes de la comparación de edición/motion design, junto a After Effects como herramienta de referencia del editor humano (vía hashtag #aftereffect), pero no detalla qué workflow o prompts usó para la versión con Claude.

**Cómo aplicarlo:** Sirve como idea de formato de contenido (hacer un "versus" entre una edición asistida por IA y una edición manual del mismo clip para generar debate/engagement), más que como tutorial técnico — para replicarlo habría que ver ambos videos, no solo este análisis de texto.

---

### 100.
## Adrián Ollero | Editor de video — https://www.instagram.com/p/DfTAYDAND9Y/

**Caption:** Comenta "100" si quieres aprender como enseñarle a claude a editar por ti

**Transcripción:** Dos partes distintas. La primera es una instrucción hablada dirigida a Claude: "necesito que vayas a mi Premiere Pro y en la secuencia que te acabo de crear me eliminas todas las tomas falsas y los silencios teniendo en cuenta que siempre apuramos mucho el corte, de hecho hacemos hasta J-Cut y L-Cut, y una vez hayas terminado me vas a generar los subtítulos de manera dinámica como siempre hacemos con este cliente". La segunda parte es simplemente el audio del material en bruto que está siendo editado (un video sobre cómo sería una "cocina ideal" de estilo casa de lujo italiana: muebles naturales, encimera en tonos piedra, tiradores discretos, iluminación cálida, pocos colores).

**Qué dice / enseña:** Muestra un workflow de edición de video donde se le da a Claude una instrucción en lenguaje natural (por voz/texto) para que opere directamente sobre un proyecto de Premiere Pro: cortar tomas falsas y silencios con un estilo de corte específico del editor (muy ajustado, usando J-Cut/L-Cut), y después generar subtítulos dinámicos siguiendo el estilo que ya usa con ese cliente en particular.

**Herramientas/skills que menciona:** Claude, controlando/editando directamente una secuencia de Adobe Premiere Pro (corte de silencios/tomas falsas, J-Cut, L-Cut, subtítulos dinámicos). No se detalla en el audio si usa un plugin, MCP o integración específica para que Claude controle Premiere.

**Cómo aplicarlo:** Para automatizar edición repetitiva propia (quitar silencios y tomas falsas, generar subtítulos con un estilo fijo por cliente), se puede intentar armar un flujo donde se le da a un agente de IA instrucciones explícitas y consistentes (criterio de corte, tipo de transición, estilo de subtítulo) en vez de pedir algo genérico, para que el resultado sea reproducible proyecto a proyecto.

---

### 101.
## Manu Sabio — https://www.instagram.com/p/DfQcbrLusQW/

**Caption:** (sin texto de caption)

**Transcripción:** El creador muestra (mientras dice estar trabajando en "Cloud") una especie de sala de control/dashboard que representa a sus "editores de video de inteligencia artificial": un panel grande con una pantalla de resumen general y, dentro, distintos "editores" representados individualmente — uno cortando distintas tomas, otro animando con motion graphics, otro también cortando tomas — y dice que pueden hacer seguimiento de qué está haciendo cada uno para cada cliente. Aclara que es una visualización "media animada y media hecha como un juego" de cómo funcionan sus agentes de IA para edición de video internamente, y promete mostrar otras áreas en futuros videos.

**Qué dice / enseña:** Muestra (sin explicar el cómo técnico) una interfaz/dashboard de seguimiento de múltiples agentes de IA trabajando en paralelo en tareas de edición de video (corte de tomas, motion graphics) para distintos clientes, como parte del "detrás de escena" operativo de un servicio de edición con IA.

**Herramientas/skills que menciona:** No nombra herramientas o modelos de IA específicos (dice "Cloud" pero no se aclara si es un nombre propio de su sistema, un software o simplemente "la nube"); tampoco menciona qué agentes o APIs usan para cortar tomas o animar motion graphics.

**Cómo aplicarlo:** Es más una pieza de marketing/showcase de un servicio que un tutorial — lo aplicable es la idea de construir (o al menos mostrar) un dashboard de seguimiento cuando se corre más de un agente de IA en paralelo sobre distintos proyectos/clientes, para tener visibilidad de en qué está cada uno.

---

### 102.
## BreaLabs — https://www.instagram.com/p/DfRuXh5NVZ4/

**Caption:** Vibe-coded website security: a burglar tries 7 doors 🚪. 1. An API key in the browser code. 2. The .env file on the live site. 3. A login only checked in the browser. 4. Change the number in the address: someone else's invoice. 5. No row level security: the whole database answers. 6. An admin page that's hidden, not locked. 7. No HTTPS: the password travels in plain text. Part 1 of our 67 checks. Stuck on one? We'll finish it. Link in bio. How many were open on yours? #vibecoding #websitesecurity #cybersecurity #webdevelopment

**Transcripción:** Con metáfora de un ladrón probando puertas de una casa ("vibe-coded website"), recorre 7 fallas de seguridad típicas de un sitio vibecodeado: 1) API key expuesta en el código del browser, 2) archivo .env presente en el sitio en producción, 3) login validado solo en el cliente/navegador, 4) IDOR — cambiar un número en la URL permite ver la factura de otra persona, 5) falta de row level security, por lo que toda la base de datos responde sin restricción, 6) panel de admin que está oculto pero no protegido con autenticación real, 7) falta de HTTPS, por lo que la contraseña viaja en texto plano. Remata diciendo que esto es la parte 1 de "67 checks" que ofrecen como servicio.

**Qué dice / enseña:** Lista concreta de 7 vulnerabilidades comunes en apps/sitios hechos con vibecoding: secretos (API keys, .env) expuestos en el frontend o en el deploy, autenticación/autorización chequeada solo en el cliente, IDOR (acceso a recursos de otros usuarios cambiando un ID en la URL), falta de row-level security en la base de datos, "seguridad por oscuridad" en paneles de admin, y falta de HTTPS.

**Herramientas/skills que menciona:** No nombra herramientas de IA puntuales — habla de "vibe-coded" en general como el tipo de sitio con estas fallas, y promociona su propio servicio de auditoría ("67 checks") sin detallar con qué herramientas lo hacen.

**Cómo aplicarlo:** Usarlo como mini-checklist de seguridad antes de lanzar cualquier app vibecodeada: verificar que ninguna API key quede en código de frontend ni el .env en el servidor público, que la autenticación y los permisos de admin se validen en el backend (nunca solo en el cliente), que los IDs de recursos no permitan acceder a datos de otro usuario (IDOR), que la base de datos tenga row level security activada, y que el sitio sirva todo por HTTPS. Para un checklist más completo de este tipo de revisiones antes de lanzar algo vibecodeado, está la skill `vibecoding-launch-checklist`.

---

### 103.
## nowfyyyyy — https://www.instagram.com/p/DerZrbYgeba/

**Caption:** Claude Code + after effects perfect workflow✅. Saving a lot of times for motion animator's 🔥 #motiongraphics #animation #claudecode #aftereffect #editör @claudeai @adobevideo

**Transcripción:** El audio transcrito vino vacío (solo ruido/silencio detectado) — es un video sin narración hablada, probablemente una grabación de pantalla con música de fondo mostrando el workflow, sin texto hablado que explique los pasos. No se puede determinar el contenido exacto sin ver las imágenes del video.

**Qué dice / enseña:** Según el caption, muestra un workflow que combina Claude Code con After Effects para ahorrar tiempo a animadores de motion graphics, pero sin audio ni descripción del paso a paso no se puede saber qué tareas concretas hace Claude Code ahí (¿generar expresiones/scripts de AE, automatizar renders, generar assets?).

**Herramientas/skills que menciona:** Claude Code y Adobe After Effects (via caption y menciones @claudeai @adobevideo), combinados en un mismo workflow de motion graphics — sin más detalle sobre cómo se integran.

**Cómo aplicarlo:** No se puede aplicar con certeza sin ver el video en sí (las imágenes), ya que el caption solo afirma el ahorro de tiempo sin describir la técnica; para aprovecharlo habría que mirar el reel directamente para ver qué parte del trabajo en After Effects delega en Claude Code.

---

### 104.
## Marc Llopis — https://www.instagram.com/p/DfP1HiEoYy8/

**Caption:** 25 formatos de anuncio que funcionan en Black Friday, de las malas noticias a la venta cruzada. Para esta campaña no hace falta reinventar nada: elige 3 o 4 que encajen con tu marca y produce varias versiones de cada uno. Guárdalo para cuando montes los creativos. En mi canal de YouTube explico estrategia creativa en Meta Ads paso a paso. Link en mi bio. #blackfriday #metaads #ecommerce #creativos #shopify

**Transcripción:** Lista hablada de 25 formatos de anuncio (solo los nombres, sin explicar cada uno en detalle): malas noticias, globos, pregunta en stories, escrito a mano, meme, foto del checkout, post-its, muro de reseñas, x razones, "lo sentimos", oferta de almacén, captura de email, AirDrop, descuento gigante, UGC estático, notas del iPhone, pizarra, censurado, pantalla de bloqueo, última hora, cuadrícula, low fee nativo, última oportunidad, almacén low fee, venta cruzada.

**Qué dice / enseña:** Un catálogo rápido de 25 formatos/plantillas de creativos de anuncio (principalmente para Meta Ads / e-commerce) pensados para campañas de Black Friday, cada uno nombrado por su concepto visual o de copy (ej. "muro de reseñas", "pantalla de bloqueo", "escrito a mano"), sugiriendo elegir solo 3-4 que calcen con la marca propia y producir varias versiones de cada uno en vez de inventar formatos nuevos.

**Herramientas/skills que menciona:** Ninguna herramienta de IA/código — es una lista de formatos creativos de marketing/publicidad, pensada para producir manualmente o con cualquier editor.

**Cómo aplicarlo:** Al armar creativos de campaña (no solo para Black Friday), usar esta lista como banco de formatos probados: elegir 3-4 que calcen con el tono de marca propia y generar varias variaciones de cada uno (distintos productos/ángulos) en vez de partir de cero en cada anuncio.

---

### 105.
## Chris Radloff — https://www.instagram.com/p/DfQb8EWzK8E/

**Caption:** An 8-minute StorySelling ad won't carry your entire funnel. If you're testing these, here's how I'd think about the creative around them. TOF → Get specific. One experience. One pain point. Hook the viewer, keep them engaged, and show them how your product works. Test across as many relevant pain points as you can. MOF → Make it relatable. Bring across your affiliate content from Trybe and TikTok Shop. Use creators your customer sees themselves in. Or aspires to be like. BOF → Give them a reason to buy. Your offer does the heavy lifting here. Build a bundle that makes sense and give them great value. Each piece of creative has a job. Before you copy a brand's long-form ad, look at what else they're running around it. Save this for your next creative planning session. #creativestrategy #advertising #ecommerce

**Transcripción:** Explica por qué varias marcas están corriendo anuncios de 8+ minutos en Meta: detectaron un cambio de algoritmo que ahora optimiza por watch time, pero esos videos largos solos "queman" presupuesto rápido si no están acompañados del resto del funnel. Propone pensar el funnel creativo completo en 2026: en TOF (top of funnel), videos específicos por un solo dolor/experiencia (no genéricos), que enganchen y muestren el mecanismo del producto, probando tantos pain points como sea posible (menciona como referencia las ad libraries de Resilia, Underdog y Rise); en MOF (middle of funnel), contenido de afiliados/creadores (traídos desde Tribe y TikTok Shop) que se parezcan o sean aspiracionales para el cliente ideal (referencia: Goalie, Physicians Choice, High Strips); en BOF (bottom of funnel), el foco pasa a la oferta — armar un bundle con buen valor que cierre la venta (referencia: Iron Mate, Primal Queen, Garoons).

**Qué dice / enseña:** Framework de funnel creativo para e-commerce/Meta Ads en 2026: cada etapa del funnel (TOF/MOF/BOF) necesita un tipo de creativo distinto con un trabajo específico — TOF para generar interés específico por dolor, MOF para generar relación/aspiración vía creadores, BOF para cerrar con oferta — y advierte que copiar solo el anuncio largo viral de una marca sin el resto del ecosistema de creativos no funciona.

**Herramientas/skills que menciona:** Menciona plataformas de afiliados/UGC (Trybe, TikTok Shop) y las "ad libraries" de Meta como fuente de inspiración de marcas específicas, pero ninguna herramienta de IA/código.

**Cómo aplicarlo:** Al planear una campaña de ads para un producto propio, no apoyarse en un solo formato de anuncio (ej. un long-form viral): armar explícitamente piezas para cada etapa del funnel (ganchos específicos por pain point arriba, contenido de creadores relatable en el medio, oferta/bundle fuerte al final) y revisar la ad library completa de una marca de referencia antes de copiar solo su anuncio más viral.

---

### 106.
## Taha PathionAI — https://www.instagram.com/p/De6g8imtGRT/

**Caption:** Comment CONNNECT and I will send the Guide over

**Transcripción:** Lista de 5 conectores/MCPs que recomienda agregarle a Claude antes de usarlo: (1) Perplexity, para research en tiempo real; (2) Firecrawl, para que Claude pueda scrapear sitios web, sacar brand assets e investigar competidores; (3) Playwright, para que Claude tenga su propio browser y pueda abrir páginas, probar botones, llenar formularios y testear lo que acaba de construir; (4) Posthog, para ver analytics del sitio (cuánta gente se registra, qué errores tiran); (5) Composio, un conector que conecta múltiples apps (Gmail, Slack, etc.) sin tener que configurar cada una por separado. Cierra invitando a comentar "connect" para recibir la guía de setup.

**Qué dice / enseña:** Presenta 5 MCPs/conectores recomendados para potenciar a Claude en un flujo de desarrollo: research (Perplexity), scraping web (Firecrawl), testing de browser (Playwright), analytics de producto (Posthog) y conectividad multi-app (Composio).

**Herramientas/skills que menciona:** Perplexity, Firecrawl, Playwright, Posthog (nombrado "Post-hoc" en el audio, por transcripción de Whisper) y Composio, todos como MCPs/conectores para Claude.

**Cómo aplicarlo:** Evaluar instalar alguno de estos MCPs según la necesidad del proyecto — Playwright si se necesita testear UI automáticamente, Firecrawl si se necesita research de competidores o extraer contenido de sitios, Posthog para analytics de producto, Composio para integrar múltiples apps sin configurar cada conector individual. No da instrucciones técnicas de instalación en el video, solo nombra las herramientas.

---

### 107.
## Cooked Dev — https://www.instagram.com/p/DfQE07UxOiN/

**Caption:** Claude, where can I find free APIs with no key? #Claude #ClaudeCode #VibeCoding #ClaudeSkills #PublicAPIs

**Transcripción:** Se queja de que todo pide tarjeta de crédito o key hasta para cosas tontas (ej. una API de datos de gatos por $29/mes). Presenta una alternativa: un repo/lista con "half a million stars" (muy popular en GitHub) que recopila APIs gratuitas, organizadas por categoría, con una columna de "Auth" que indica si necesitan key o no — "No" significa sin key, sin registro. Hace un fetch de prueba y funciona sin tarjeta. Termina con un chiste autoconsciente: "¿qué más hay en esta lista? Tres horas después no construiste nada, seguís scrolleando" (sobre el riesgo de perder tiempo explorando la lista en vez de usarla).

**Qué dice / enseña:** Señala la existencia de un repositorio público (tipo "public-apis" en GitHub, por la descripción de "half a million stars" y organización por categoría/columna de Auth) que lista APIs gratuitas sin necesidad de API key ni tarjeta, útil para prototipar rápido sin pagar ni registrarse.

**Herramientas/skills que menciona:** No nombra el repo explícitamente en el audio ni en el caption (solo se ve en pantalla, no accesible desde la transcripción), pero por la descripción coincide con el repo "public-apis" de GitHub. Un comentario del post advierte sobre el riesgo de que un agente de IA use una de estas APIs sin control a las 3am y construya una feature entera sobre ella.

**Cómo aplicarlo:** Al vibecodear un prototipo que necesite datos externos, buscar primero en un listado de APIs públicas sin auth (como "public-apis" en GitHub) antes de pagar por una API con key, para prototipar gratis. Ojo con el riesgo que marca el comentario: si se le pide a Claude que elija una API de la lista sin supervisión, puede construir sobre una API poco confiable o decidir mal el fetch sin revisión humana.

---

### 108.
## Enrique Rocha — https://www.instagram.com/p/Dd8opvxC8yg/

**Caption:** Cuida tu Claude de skills y herramientas infectadas

**Transcripción:** Advierte que pueden hackear tu Claude Code si instalás skills/herramientas recomendadas en Instagram sin un "guardián" que las revise antes de que toquen tu computadora. Presenta una herramienta llamada "Skill Spectre" (de NVIDIA, gratuita) que escanea skills y herramientas antes de pasárselas a Claude, para ver si traen algo malicioso. Dice que la instaló pero se le olvidaba usarla, así que la convirtió en un "guardián" automático: pegándole un prompt a Claude Code, este configura solo el guardián para que, antes de bajar cualquier herramienta o skill de internet, la escanee automáticamente; si sale limpia sigue, si encuentra algo grave se frena y muestra un reporte para que el usuario decida. Lo configuró para que solo frene en casos graves. Invita a comentar qué están construyendo con Claude para pasarles el guardián.

**Qué dice / enseña:** Enseña a usar "Skill Spectre" (herramienta de NVIDIA) como escáner de seguridad para skills/herramientas de terceros antes de instalarlas en Claude Code, y cómo automatizarlo como un guardián (hook) que escanea automáticamente cualquier descarga de skill/herramienta de internet, bloqueando solo los casos graves y mostrando un reporte.

**Herramientas/skills que menciona:** Skill Spectre (de NVIDIA), usado junto con Claude Code vía un prompt que configura el guardián automático (probablemente un hook de Claude Code, aunque no se detalla técnicamente en el video).

**Cómo aplicarlo:** Antes de instalar cualquier skill o herramienta de terceros en Claude Code (como las que se recomiendan en reels de este mismo documento), evaluar instalar Skill Spectre de NVIDIA y configurarlo como guardián automático para escanear skills/MCPs antes de que se ejecuten, en vez de instalar a ciegas lo que se ve en redes sociales — esto conecta directo con la nota ya guardada de "no instalar nada a ciegas" en este proyecto.

---

### 109.
## Perly 🦈 — https://www.instagram.com/p/DZGvjhKt2gA/

**Caption:** STOP USING SUPABASE if you code with AI. I cannot TELL you the amount of times I've seen critical security vulns with supabase, make sure to check these policies and setting before launching! #vibecoding #vibecodingsecurity #csstudents #vibecode #cybersecuritytips @supabasecom

**Transcripción:** Habla una analista de seguridad. Dice que mucha gente que vibecodea con Supabase no entiende cómo usarlo de forma segura y termina filtrando toda su base de datos de usuarios e info privada — le pasa a todos, desde diseñadores que postean sus proyectos hasta empresas de YC. Da 3 tips: (1) revisar que RLS (Row-Level Security) esté activado — si está apagado, cualquiera con la anon key puede leer cualquier tabla; (2) configurar policies claras para que cada usuario solo acceda a sus propios datos; (3) nunca filtrar la service key (la key de admin) — la anon key puede estar en el frontend sin problema si RLS y las policies están bien configuradas, pero la service key nunca debe estar en el frontend, en GitHub ni en ningún lado público, porque anula toda la seguridad de RLS y policies. Cierra aclarando que no es para desalentar el vibecoding, sino para tener en cuenta buenas prácticas de seguridad.

**Qué dice / enseña:** Checklist de seguridad específico de Supabase para apps vibecodeadas: activar RLS, definir policies de acceso por usuario, y nunca exponer la service key (a diferencia de la anon key, que sí puede estar en el frontend si RLS/policies están bien puestas).

**Herramientas/skills que menciona:** Supabase (RLS, policies, anon key vs. service key). No menciona un skill o comando de Claude específico, es un checklist de configuración de seguridad en el propio dashboard/proyecto de Supabase.

**Cómo aplicarlo:** Antes de lanzar cualquier proyecto propio que use Supabase, verificar explícitamente estos 3 puntos (RLS on, policies por usuario, service key nunca en frontend/repo público) — esto encaja directo con el checklist más amplio que ya tiene la skill `vibecoding-launch-checklist` de este entorno para revisar seguridad antes de lanzar algo vibecodeado.

---

### 110.
## Thomas Kim — https://www.instagram.com/p/DePGBFXtswr/

**Caption:** These are my essential AI coding skills I use to keep code quality high and not bloated when AI writes and merges my code for me. Video 5 de 7 de su serie "how to become a 10x ai-native developer". Explica que en los primeros 4 videos habló de usar cloud agents como ingenieros 24/7 que arreglan bugs mientras duerme, usando skills de verificación para chequear que los cambios de código funcionan y mergeando sin revisión suya. En este video responde la pregunta de cómo mantiene la calidad del código con tanto código mergeándose sin supervisión: usando skills de de-bloating. Usa el "thermo nuclear code quality review" del equipo de Cursor junto con herramientas específicas de framework (una skill de React best practices) y, uno de sus favoritos, la skill "ponytail" — recomienda ver ponytail.dev.

**Transcripción:** Presenta 3 skills/sistemas que usa para evitar que el código bloateado se le escape al mergear ~30 PRs por día sin supervisión manual: (1) "Ponytail" (ponytail.dev) — un "de-bloating tool" que señala patrones de diseño malos, simplifica al máximo y refactoriza en módulos reutilizables, con una landing page cómica sobre el "senior staff engineer" que arregla todo con dos líneas y se vuelve a dormir; (2) "PStack" — no es un skill individual sino un sistema de ingeniería completo creado por un ingeniero de SpaceX (alias "potato" en X) para crear una "fábrica de software", que ya incluye sub-skills de de-bloating como "no comment", "TypeScript best practices" y "unslop", y que según dice potencia el 90% de sus PRs; (3) "Thermonuclear code quality review", otra skill del equipo de Cursor/SpaceX AI que hace algo similar a las anteriores. Dice que condensa todo esto en un solo comando "simplify" que llama a las skills de simplificación de Ponytail, PStack y Thermonuclear Code Quality Review en cada PR, para mantener los cambios lo más mínimos posible y la calidad alta.

**Qué dice / enseña:** Cómo mantener la calidad de código alta cuando se deja que agentes de IA escriban y mergeen código sin revisión humana constante: apoyarse en varias skills de "de-bloating"/simplificación (Ponytail, PStack, Thermonuclear Code Quality Review) ejecutadas automáticamente antes de cada PR, condensadas en un solo comando "simplify".

**Herramientas/skills que menciona:** Ponytail (ponytail.dev), PStack (sistema de "potato" en X, ex-SpaceX), Thermonuclear Code Quality Review (equipo de Cursor/SpaceX AI), más sub-skills de PStack como "no comment", "TypeScript best practices" y "unslop".

**Cómo aplicarlo:** Interesante en primera persona: la skill `ponytail` que menciona este reel es la misma que está activa en este entorno ahora mismo (modo "full", de .claude). Vale la pena considerar correr un comando tipo "simplify" (como ya existe la skill `simplify` en este entorno) antes de cerrar un PR o una tarea de código generada por un agente, y evaluar si conviene combinarlo con una skill de code-review tipo "thermonuclear" (la skill `code-review` de este entorno con nivel alto) cuando se deja que el agente mergee sin supervisión directa.

---

### 111.
## Charles Liu — https://www.instagram.com/p/DfPruJSxggG/

**Caption:** All the design techniques and principles I used to build this age picker: Fitts's law (bigger targets son más fáciles de tocar, por eso arrastra todo el ancho); visual hierarchy (el número que elegís es lo más grande en pantalla); Von Restorff effect (un solo color de acento, solo en la aguja); object constancy (los números deslizan en vez de reemplazarse, para que el ojo los siga); snapping (siempre se asienta en un año entero); motion blur (suaviza el salto de un número a otro); natural mapping (más viejo sube, más joven baja); tabular figures (cada dígito tiene el mismo ancho, nada se mueve); animar solo el delta (solo se mueve el dígito que cambió); inercia (lo deslizás y se frena solo); feedback multimodal (ves y escuchás cada año pasar); pistas visuales (brilla al hacer hover, para saber que es interactivo antes de tocarlo); skeuomorfismo (se ve y se mueve como un dial real, así nadie necesita instrucciones). #design #ai #designwithai #claude #tech

**Transcripción:** Muestra la evolución de un "age picker" (selector de edad) hecho con IA, en pasos: el estado inicial que da la IA; hacerlo arrastrable y arreglar la jerarquía visual ("ahora se ve diseñado"); animar la transición y agregar snapping ("ahora se siente vivo"); agregar blur de movimiento y espaciado de fuente consistente ("ahora se siente pulido"); darle momentum y hacer que cada año "clickee" ("ahora no podés dejar de jugar con él"); y doblarlo en una rueda real ("ahora sí está pulido"). Cierra con "no te quedes ahí cuando funciona" e invita a seguir para la parte 2.

**Qué dice / enseña:** Catálogo de 13 principios de microinteracción/UX (Fitts's law, jerarquía visual, efecto Von Restorff, object constancy, snapping, motion blur, natural mapping, tabular figures, animar solo el delta, inercia, feedback multimodal, pistas visuales, skeuomorfismo) aplicados paso a paso para transformar un selector de edad genérico generado por IA en un componente pulido y satisfactorio de usar, mostrando que "funciona" y "se siente bien" son etapas distintas del trabajo de diseño.

**Herramientas/skills que menciona:** Menciona "Claude" en los hashtags como la IA usada para generar el diseño base, pero no da prompts ni código concreto — es una lista de principios de diseño aplicados, no instrucciones técnicas paso a paso.

**Cómo aplicarlo:** Usar esta lista de 13 principios como checklist al pulir cualquier componente interactivo generado por IA (sliders, pickers, inputs custom): no conformarse con la primera versión que "funciona", sino iterar agregando jerarquía visual, snapping, animación del delta, inercia y feedback para que se sienta pulido — aplicable directamente con las skills de este entorno orientadas a UI (`impeccable` para crítica/pulido de interfaces, o `motion-effects` para la parte de animación).

---

### 112.
## Keyframes — https://www.instagram.com/p/DfPMEV4J_3N/

**Caption:** Left: what Claude made when we asked it for an animated video about touchscreens. A real output, nothing changed. Right: the same Claude with Keyframes. Same Claude, same idea. The difference is a video system we spent hundreds of hours building for ourselves. In our first week with it, three videos hit 24 million views. Bring your idea and the Claude you already pay for. getkeyframes.com

**Transcripción:** Comparación lado a lado: a la izquierda, lo que genera Claude solo cuando le pedís un video animado — queda genérico porque "no sabe qué es un buen video por sí mismo". A la derecha, el mismo Claude pero usando "Keyframes", un sistema propio que construyeron durante cientos de horas. Dicen que en su primera semana usándolo, tres videos llegaron a 24 millones de views. Cierra con "el Claude que ya pagás puede hacer tus videos ahora, solo necesita Keyframes" y pide seguir el link en bio.

**Qué dice / enseña:** Es un anuncio/demo de producto (Keyframes) que posiciona a Claude "solo" como insuficiente para generar videos animados de calidad, y vende su sistema propio como la capa que falta para que Claude produzca videos virales. No explica cómo funciona Keyframes técnicamente, es puramente promocional con un antes/después.

**Herramientas/skills que menciona:** Claude (como motor base) y "Keyframes" (producto propio de la cuenta, en getkeyframes.com) como la capa/sistema que mejora los outputs de video de Claude. No da detalles de implementación.

**Cómo aplicarlo:** Es publicidad de un producto de terceros, no un tutorial — no hay nada reproducible del video en sí. Si interesa el resultado (videos animados con Claude con buena calidad de motion design), la alternativa que ya existe en este entorno es usar las skills propias de motion/video (`hyperframes`, `motion-effects`, `launch-video`, `apple-launch-film`, etc.) en vez de depender de un producto externo como Keyframes.

---

### 113.
## Roberto P. Nickson — https://www.instagram.com/p/DfP82wHpjx5/

**Caption:** My studio now runs on @claudeai. Built un sistema en su estudio donde todo lo que se ve en el video es posible con Claude: su calendario, email y archivos están conectados vía los connectors nativos de Claude; las puertas del garage, luces, TVs, espacios de trabajo e incluso su impresora 3D corren por MCP servers custom que Claude le escribió, usando las APIs de esos dispositivos o su red local. Puede controlar todo con un ESP32 en el escritorio, o hablarle directo a Claude por la app (la voz que se escucha es la voz default de Claude). Aclara que las respuestas y los tiempos del video están simulados para la edición — en la vida real tardan unos segundos más. Es el episodio 3 de su serie "Life with Claude". #ClaudePartner #Ad (contenido pago/patrocinado por Anthropic).

**Transcripción:** Diálogo hablado entre Roberto y "Claude" (voz) simulando un día en el estudio: Claude lo saluda al llegar, le resume el día (propuestas enviadas de noche, un fix de sitio ya en producción, inbox reducido a 3 emails que realmente necesitan atención, su única cita real a las 2pm); le cuenta que arregló bugs, secuenció una edición, limpió una función que Roberto venía evitando, armó un deck dejando la última slide en blanco (para que la complete él); también gestiona la impresora 3D (imprimió algo para uno de sus hijos), le recuerda que viene llevando el presupuesto del mes, confirma con un empleado (Ethan) que una edición de video está lista ("Claude hizo la mayor parte"), la guarda en la carpeta del cliente y avisa al cliente, y pone música lo-fi para enfocarse a pedido.

**Qué dice / enseña:** Es contenido publicitario pagado (#Ad, "ClaudePartner") que muestra un caso de uso aspiracional de Claude como asistente integral de un estudio creativo: conectado a calendario/email/archivos vía connectors nativos, y a dispositivos físicos (garage, luces, TVs, impresora 3D) vía MCP servers custom escritos por el propio Claude usando las APIs de esos dispositivos o la red local, controlable por voz o por un dispositivo ESP32 físico. No muestra el "cómo" técnico de escribir esos MCP servers, es una demo conceptual/aspiracional, y aclara explícitamente que los tiempos de respuesta están simulados.

**Herramientas/skills que menciona:** Claude (connectors nativos para calendario/email/archivos), MCP servers custom escritos por Claude para dispositivos físicos (domótica, impresora 3D), un dispositivo ESP32 como interfaz física, y la app de Claude con voz nativa.

**Cómo aplicarlo:** Como idea general (no hay instrucciones técnicas en el video): se puede pedirle a Claude que escriba un MCP server custom para controlar un dispositivo propio con API o en la red local (ej. domótica, impresoras), de forma similar a como ya existen MCP servers de terceros conectados en este mismo entorno (Vercel, Supabase, Notion, etc.) — la diferencia es que en este caso los MCP los escribe el propio Claude a medida en vez de usar uno ya publicado.

---

### 114. Admanage AI — https://www.instagram.com/p/DfpJG2HOc16/

**Caption:** "Comentá 'CLONE' y te mando la herramienta." #metaads #facebookads #facebookadvertising #marketing

**Transcripción:** Explica una estructura de formatos de ads de Meta organizada por etapa del funnel. Top of funnel: respuestas a Instagram Stories (no parecen ad, sirven para trackear audiencia fría), ads censurados/blur como CTA de curiosidad, y entrevistas de calle (generan muchas impresiones). Middle of funnel: formato "5 razones por las que funciona" (argumento estructurado) y ads con estadísticas (apuntan a audiencias más tibias, apelan a sus puntos de dolor). Bottom of funnel: alerta de "poco stock" para generar urgencia/escasez. Cierra diciendo que construyó una herramienta de IA para clonar estos formatos para la marca del espectador, y que comente "clone" para que se la mande.

**Qué dice / enseña:** Enseña una clasificación real de formatos de ad orientados a cada etapa del funnel de marketing (TOF/MOF/BOF), con el razonamiento de por qué cada formato funciona en esa etapa. El contenido educativo en sí es completo y concreto, pero termina en un gate clásico de generación de leads ("comentá para que te mande la herramienta") — la herramienta de IA mencionada no se describe ni se muestra, es solo un gancho de captura de contacto.

**Herramientas/skills que menciona:** Formatos de Meta Ads (respuestas a Stories, ads censurados/blur, entrevistas de calle, "5 razones", ads con estadísticas, alertas de stock bajo); una herramienta de IA propia para clonar estos formatos (no detallada, gateada detrás de un comentario).

**Cómo aplicarlo:** Mapear los ads propios según la etapa del funnel: usar formatos de baja fricción y curiosidad (Stories, blur, calle) para audiencia fría; formatos de prueba/argumento (razones, estadísticas) para audiencia tibia que ya conoce el producto; y triggers de urgencia (stock bajo) para cerrar en el fondo del funnel. La "herramienta de IA" mencionada no es accesible sin comentar, así que no se puede evaluar ni replicar directamente.

---

### 115. Omar Elsayed (egymarrr) — https://www.instagram.com/p/Dd7VOqppMHY/

**Caption:** "Conviértete en un cerrador (closer) de ventas de la noche a la mañana." #fyp #florida #sales #onlinemoney #motivation

**Transcripción:** Hay audio hablado, pero la transcripción de Whisper devuelve solo un fragmento incoherente: "Ready? N F B B I I Space C C I I A A Space". No es una transcripción fiel de un discurso completo — parece corresponder a un video muy corto o a un segmento con sonido no claro (posible letreo/spelling en pantalla, efecto de sonido o audio de baja calidad), no a una explicación hablada real de cómo "cerrar ventas".

**Qué dice / enseña:** No se puede determinar con certeza qué enseña el reel: el audio real no es inteligible en la transcripción obtenida, y el caption es solo una frase gancho genérica de motivación en ventas sin contenido técnico. No hay suficiente información fiel (caption + transcripción) para afirmar qué método o técnica de venta se enseña.

**Herramientas/skills que menciona:** Ninguna identificable con certeza a partir del caption o la transcripción disponible.

**Cómo aplicarlo:** No aplica — el contenido real no es accesible/inteligible a partir de los datos obtenidos (transcripción incoherente y caption sin detalle técnico), así que no hay base real para dar una recomendación de aplicación.

---

### 116. Eric Does Ecom — https://www.instagram.com/p/Dfk3IDoPWAy/

**Caption:** "El video editing cambió para siempre." #ecommerce #metaads #dropshipping #aiugc #aiads

**Transcripción:** Explica paso a paso cómo hacer video ads de dropshipping usando el nuevo modelo Claude Fable 5.2, de forma gratuita y sin suscripciones de video con IA, todo "localmente con Claude". Paso 1: pedirle a Claude que escriba un guion de 30-60 segundos que atrape rápido al viewer y convenza de comprar sin sonar demasiado vendedor. Paso 2: convertir ese guion en audio con la función text-to-speech de ElevenLabs (11labs), que da 10.000 créditos gratis por mes. Paso 3: pedirle a Claude que escanee YouTube, TikTok e Instagram buscando videos del producto para usar como b-roll, priorizando clips limpios sin overlays de texto, y descargarlos con la librería de Python yt-dlp. Paso 4: que Claude escanee y categorice esos clips y los superponga sobre el guion donde correspondan, y que genere subtítulos estilo Hormozi y una pista de audio sincronizada con lo que pasa en el video. Afirma que así no se necesita Higgsfield, CapCut ni edición manual.

**Qué dice / enseña:** Enseña un workflow concreto end-to-end para producir video ads de dropshipping combinando Claude (Fable 5.2) para guion y orquestación, ElevenLabs para voz y yt-dlp para conseguir b-roll de producto desde redes. Es un flujo plausible y con pasos específicos (no gateado), aunque no muestra la ejecución real en pantalla ni los prompts exactos que usaría para cada paso.

**Herramientas/skills que menciona:** Claude Fable 5.2, ElevenLabs (text-to-speech, plan gratuito de 10.000 créditos/mes), yt-dlp (descarga de video desde YouTube/TikTok/Instagram), subtítulos estilo "Hormozi".

**Cómo aplicarlo:** Replicar el flujo: 1) pedir a Claude un guion corto orientado a conversión; 2) generar el audio con el plan free de ElevenLabs; 3) usar yt-dlp (vía Claude o manualmente) para bajar clips limpios del producto desde redes como b-roll; 4) pedirle a Claude que categorice y ordene esos clips sobre el guion; 5) agregar subtítulos estilo Hormozi y sincronizar audio. Atención: usar b-roll de otras cuentas/redes para ads propios puede tener implicancias de derechos de autor que el reel no aborda.

---

### 117. James Goldbach — https://www.instagram.com/p/DfnNdhBj5yA/

**Caption:** "Comentá 'FABLE PROMPT' y te mando el desglose completo para tu agente." Fable 5.2 no quiere los prompts que escribiste para modelos anteriores — 10 cambios directo de la guía de prompting de Anthropic.

**Transcripción:** Fable 5.2 acaba de salir y hay que cambiar el estilo de prompting. 1) Decirle que el codebase es suyo: Anthropic mostró que esto hace que el modelo efectivamente fusione código duplicado, básicamente refactorizándolo para hacerlo más eficiente. 2) Agregar una línea sobre "terminar el trabajo" en el archivo de reglas: esto reduce cuánto el agente se detiene cuando todavía tiene cosas por hacer. 3) Decir "no pienses" no hace que el modelo no piense — hay que bajar el nivel de esfuerzo (effort) en su lugar. 4) Decirle al modelo que sea consciente de los límites de uso: si es consciente de sus límites de uso, delega más eficientemente a subagentes. 5) Auditar las reglas y guardrails en busca de líneas de "nunca hagas esto": eso hace que el modelo sea más tímido y menos propenso a trabajar de forma autónoma. Agrega que este modelo, como todo frontier model nuevo, sigue las reglas de forma más precisa, así que las reglas de aprobación deben estar formuladas con mucha precisión, o el modelo se pondrá tímido con cosas que sí se quiere que haga. Cierra pidiendo comentar "FablePrompt" para recibir la lista completa de 10.

**Qué dice / enseña:** Enseña 5 de los 10 cambios de prompting que, según el autor, vienen de la guía de prompting de Anthropic para el modelo "Fable 5.2" (nombre que en este entorno corresponde al modelo de Claude usado en este sistema), con razones concretas para cada uno (fusionar código duplicado, terminar tareas pendientes, usar nivel de esfuerzo en vez de pedir "no pensar", conciencia de límites de uso para delegar a subagentes, y evitar reglas de "nunca hagas esto" que vuelven al modelo demasiado tímido). Los otros 5 cambios están gateados detrás del comentario "FablePrompt" — no están en el contenido accesible.

**Herramientas/skills que menciona:** Claude ("Fable 5.2"), archivo de reglas/guardrails del agente, subagentes, nivel de "effort" (esfuerzo) del modelo, límites de uso (usage limits).

**Cómo aplicarlo:** Revisar el archivo de reglas (CLAUDE.md o equivalente) del propio setup de agente y: declarar explícitamente que el codebase le pertenece al agente para que refactorice más agresivamente; agregar una instrucción de "terminar el trabajo pendiente antes de parar"; en vez de pedir "no pienses", ajustar el nivel de esfuerzo/reasoning; mencionarle al agente los límites de uso para que delegue mejor en subagentes; y revisar las reglas de "nunca hagas X" reformulándolas con precisión para no volver al agente innecesariamente tímido en tareas que sí se quiere que resuelva solo.

---

### 118. Franky Shaw — https://www.instagram.com/p/DcRrXjsRyig/

**Caption:** "Así nos van a recordar." Showcase de su "5.3 Animation Framework". Plantea que las marcas deberían convertirse en mini estudios de TV: personajes recurrentes, tramas continuas, productos integrados en la trama — cada ad se vuelve otro episodio que la gente reconoce. "El entretenimiento gana la atención. La educación gana la venta."

**Transcripción:** Es un sketch animado de un profesor mostrando a su clase cómo era el hombre promedio en EE.UU. en 2040 (redondo, con piernas que apenas funcionan) comparado con 1940 (musculoso, "parece un superhéroe", podría cargar todas las baterías de un Tesla en un viaje). El diálogo explica que esto se debe a que con el tiempo se "quitaron los minerales de los granos" y recién después "la gente empezó a devolver los minerales". Termina con el pitch de producto: un suplemento que combina más de 100 minerales de "tierra de Wyoming" hecho para hombres, para llenar los vacíos minerales de la dieta moderna, en una sola cápsula.

**Qué dice / enseña:** Es un ad animado de un suplemento (venta directa de producto) disfrazado de sketch educativo/humorístico sobre nutrición histórica, usando personajes recurrentes y una trama narrativa como gancho (el propio caption lo confirma: es un "showcase" de su framework de animación para ads). El verdadero contenido que enseña (a nivel de formato publicitario) es la estrategia narrativa: usar entretenimiento con personajes y arco de historia para ganar atención, y dejar que la "educación" (la explicación semi-científica sobre minerales) haga la venta. No es un tutorial técnico de cómo producir la animación.

**Herramientas/skills que menciona:** Menciona su propio "5.3 Animation Framework" (sin detallar qué herramienta o software lo genera) y el concepto de marca como "mini estudio de TV" con personajes recurrentes y tramas continuas.

**Cómo aplicarlo:** Como estrategia de formato de ad: crear personajes recurrentes y una storyline continua para la marca en vez de ads aislados, insertar el producto dentro de la trama (no como interrupción), y usar un gancho entretenido/narrativo para captar atención antes de meter el argumento educativo que empuja la venta. El "5.3 Animation Framework" en sí no está explicado ni accesible en este reel, así que no se puede replicar la producción técnica de la animación a partir de este contenido.

---

### 119. Isaiah Rios — https://www.instagram.com/p/Dfni7RQvhw7/

**Caption:** "Hey Claude, ¿entendiste todo eso bien?"

**Transcripción:** Es un prompt leído/mostrado dirigido a Claude: "Hey Claude, no quiero que mi sitio vibe-coded sea hackeado. Por favor escondé mis API keys, revisá mis variables de entorno, y protegé mis rutas de admin. Agregá autenticación correcta, asegurate de que los usuarios solo puedan acceder a lo que les corresponde, sanitizá mis formularios, protegé contra XSS, asegurá mis endpoints de API, agregá rate limiting, y revisá mis configuraciones core. Apagá el modo debug, agregá security headers, actualizá mis dependencias, y eliminá lo que no necesito. Revisá archivos expuestos, asegurá mi base de datos, hasheá las contraseñas correctamente, revisá mi historial de Git por secretos filtrados, y corré una auditoría de seguridad completa. Lo más importante, no cometas errores."

**Qué dice / enseña:** Es, en esencia, una plantilla de prompt (un "mega-prompt" de checklist de seguridad) para pedirle a un agente de IA como Claude que haga un pase de seguridad sobre una app "vibe-coded". Enumera categorías reales y relevantes de seguridad (API keys, variables de entorno, auth, XSS, rate limiting, debug mode, headers, dependencias, archivos expuestos, hash de passwords, historial de Git, auditoría general), pero no explica cómo verificar que el agente realmente hizo cada cosa correctamente, ni da detalle técnico de implementación — es el prompt en sí, no un tutorial paso a paso.

**Herramientas/skills que menciona:** Claude, API keys, variables de entorno, autenticación, sanitización de formularios, protección XSS, rate limiting, modo debug, security headers, gestión de dependencias, hash de contraseñas, historial de Git (secretos filtrados), auditoría de seguridad.

**Cómo aplicarlo:** Usar este prompt (o una variante) como checklist al pedirle a un agente de IA que revise la seguridad de una app antes de lanzarla, pero sin confiar ciegamente en el resultado: conviene verificar manualmente cada punto (o pedir evidencia concreta del fix) en vez de asumir que "no cometas errores" garantiza que el agente lo hizo bien. Para un checklist más completo y verificable de seguridad/pagos/CI-CD antes de lanzar algo vibecoded, existe la skill `vibecoding-launch-checklist` ya disponible en este entorno.

---

### 120. Nathan Peterson — https://www.instagram.com/p/DYnUd7ESweH/

**Caption:** "Agradecemelo después." #entrepeneur #ecommerce #onlinebusiness #shopify

**Transcripción:** Para tiendas de e-commerce (implícitamente Shopify, por el contexto), explica un truco de conversión: en el checkout se puede personalizar el texto que normalmente dice algo tipo "or" (grisado, sin uso) y poner en su lugar algo como "Calificado 4.8 de 5 por más de 10.000 clientes satisfechos", texto que ve cada persona que llega al checkout. Dice que esto no es editable desde el panel normal de Shopify (fotos, reviews), sino que hay que hacerlo en el código del theme: entrar a la sección default del theme y buscar la palabra "alternative", donde está ese texto "or" grisado, y reemplazarlo por el texto deseado.

**Qué dice / enseña:** Enseña un micro-truco concreto y gratuito de CRO (conversion rate optimization) para Shopify: editar el código del theme para reemplazar el texto "or" (separador entre método de pago) en el checkout por un mensaje de prueba social (rating + cantidad de clientes), que todo visitante ve justo antes de pagar. Es instrucción específica (dónde buscar: "alternative" dentro del theme code) pero no muestra el código exacto ni el nombre exacto del archivo/liquid variable.

**Herramientas/skills que menciona:** Shopify (editor de theme/código del theme), checkout de Shopify, prueba social (social proof) en checkout.

**Cómo aplicarlo:** En el editor de código del theme de Shopify, buscar la cadena "alternative" (o el texto "or" en la sección de pago/checkout) y reemplazarlo por un mensaje corto de prueba social (rating + número de clientes/reviews). Es un cambio de bajo riesgo y costo cero, pero conviene probarlo primero en un theme de desarrollo/preview antes de publicarlo en el theme en vivo, y verificar que el rating/cifra que se use sea real y no una cifra inventada.

---

### 121. Jessie Hackett — https://www.instagram.com/p/DdAWsWBlHMl/

**Caption:** "Ranking de fixes de conversión de e-commerce de D a S-tier. ¿Cuáles importan de verdad?" #performancemarketing #ecommerce #cro

**Transcripción:** Rankea distintos "fixes" de conversión para e-commerce: un rediseño completo del homepage es tier D (casi nadie lo ve porque no se manda tráfico pago al homepage); un pop-up de "spend to win" (gastá X y ganá Y) es tier C (sorprendentemente muchas marcas todavía los usan); acelerar la velocidad del sitio en mobile es tier B (es un fix real y siempre vale la pena); poner las reviews justo al lado del botón de "agregar al carrito" es tier A (la confianza tiene que estar donde se toma la decisión, no en una página de reviews que nadie clickea); responder en una sola línea arriba del fold de la página de producto sobre tiempo de envío, devoluciones y talle/ajuste también es tier A (bajan los tickets de soporte y sube la conversión, porque los clientes no leen); y mejorar la tasa de conversión de segunda compra es tier S (convierte a los clientes ya adquiridos en embajadores de boca en boca).

**Qué dice / enseña:** Enseña una priorización concreta y justificada de tácticas de CRO (conversion rate optimization) para e-commerce, explicando el porqué de cada ranking (dónde está la atención real del usuario, dónde se toma la decisión de compra, qué reduce fricción/soporte). Es contenido completo y accionable dentro del propio video, sin gate ni promesa de "comentá para recibir más".

**Herramientas/skills que menciona:** No menciona herramientas o software específicos; son principios/tácticas de CRO para e-commerce (reviews cerca del CTA, FAQ above the fold en página de producto, velocidad mobile, retención/segunda compra, pop-ups de spend-to-win, rediseño de homepage).

**Cómo aplicarlo:** Priorizar primero las tácticas tier A/S antes que las de menor impacto: mover las reviews/calificaciones junto al botón de compra, resumir envío/devoluciones/talle en una línea visible sin scroll en la página de producto, optimizar velocidad mobile, y poner foco en estrategias de retención/segunda compra (email, programas de fidelidad) antes de invertir tiempo en un rediseño completo del homepage o en pop-ups de descuento por gasto.

---

### 122. Jon Yekar | AI for Agencies — https://www.instagram.com/p/DeogIMMIbC9/

**Caption:** "Hice un documento explicando qué es cada uno de estos términos. Si te interesa, comentá 'LIST' y te lo mando."

**Transcripción:** Lista rápida de jerga de IA/desarrollo, dicha de corrido sin explicaciones: prompting, context window, tokens, projects, skills, MCP servers, CLI, API keys, slash commands, context compaction, subagents, prompt caching, git worktrees, cronjobs, hooks, harness engineering, background agents, headless runs, parallel agents, progressive disclosure, eval-driven loops, model quantization, RLHF, memory consolidation, self-improving loops, tool poisoning, self-healing tests, agentic (algo así, término cortado/poco claro en el audio), test-time compute, KV cache. Cierra diciendo que hizo un documento explicando cada término y que comentando "LIST" lo manda.

**Qué dice / enseña:** Es un reel-gancho tipo "glosario": enumera ~29 términos de jerga IA/dev a alta velocidad para generar curiosidad, pero no explica ninguno en el video. El contenido real (las definiciones) está gateado detrás de comentar "LIST" para recibirlo por DM — no es accesible a partir del caption ni la transcripción.

**Herramientas/skills que menciona:** Los ~29 términos listados en la transcripción (prompting, context window, tokens, Projects, Skills, MCP servers, CLI, API keys, slash commands, context compaction, subagents, prompt caching, git worktrees, cronjobs, hooks, harness engineering, background agents, headless runs, parallel agents, progressive disclosure, eval-driven loops, model quantization, RLHF, memory consolidation, self-improving loops, tool poisoning, self-healing tests, test-time compute, KV cache), pero sin definiciones reales en el contenido accesible.

**Cómo aplicarlo:** Se puede usar la lista como un checklist de términos para investigar por cuenta propia (muchos ya están cubiertos en el glosario de IA que el usuario tiene pendiente armar), ya que el documento real del autor no está accesible sin comentar en el post.

---

### 123. Natalie Data Engineer — https://www.instagram.com/p/DeeR2JyNrx-/

**Caption:** "users (silently)"

**Transcripción:** No hay audio hablado. El clip (17 segundos) solo tiene música de salida ("Outro Music" detectado por el transcriptor), sin diálogo.

**Qué dice / enseña:** Parece un reel tipo meme/humor con formato "[algo] (silently)" — probablemente texto/imágenes en pantalla (no capturables por audio) mostrando una reacción humorística relacionada con "users" (usuarios), típico de memes de desarrolladores/data engineers. Sin texto en pantalla visible ni diálogo, no se puede determinar el chiste o mensaje concreto a partir del caption y la transcripción disponibles.

**Herramientas/skills que menciona:** Ninguna identificable en el audio o el caption.

**Cómo aplicarlo:** No aplica — no hay contenido técnico o accionable extraíble de este reel con la información disponible (caption + transcripción de audio).

---

### 124. Charles Liu — https://www.instagram.com/p/Dfm33XyhRN3/

**Caption:** "Algunas técnicas de diseño más que uso: Recompensa temprana, castigo tardío (el progreso se ve apenas escribís, pero los errores esperan hasta que termines, así deja de 'gritarte'); Validación inline (chequea mientras escribís, así una contraseña común como 'Password1!' se detecta al toque); Chunking (la contraseña sugerida viene en grupos chicos, más fácil de leer, igual que los números de teléfono con guiones); Cierre (el contorno se cierra en una forma completa cuando la contraseña es fuerte, sin necesidad de una etiqueta 'débil/fuerte'); Continuidad (los caracteres son monoespaciados, así cada punto se transforma en su letra en vez de saltar); Ganancia por redundancia (cada sonido coincide con algo en pantalla, lo ves y lo oís a la vez); Materialidad (vidrio esmerilado sobre el campo de contraseña, porque una textura debe tener un motivo); Antropomorfismo (el personaje mira para otro lado cuando mostrás tu contraseña). #uiux #uidesign #claudedesign #designengineering #ai"

**Transcripción:** Narra una demo de una pantalla de contraseña: "Esta es la pantalla de contraseña que te da la IA. Corto las reglas en rojo y el campo de confirmación, ahora deja de gritar. Aplico reglas estrictas y sin contraseñas comunes, ahora es honesta y segura. Recomiendo una contraseña segura, ahora se siente sin esfuerzo. Hago que el contorno sea el medidor y monoespacio los caracteres para que los puntos se transformen en letras sin saltos, ahora se siente fluido. Agrego efectos de sonido, ahora es inmersivo. Agrego vidrio de privacidad y un personaje que mira para otro lado, ahora tiene personalidad." Termina pidiendo comentar "unslop" para enviar su "skill de unslopping de IA".

**Qué dice / enseña:** Es una demo real y bien explicada de cómo aplicar principios de psicología del diseño/UX (los que detalla en el caption) a un campo de contraseña generado por IA, mostrando paso a paso cómo cada ajuste (microcopy, validación inline, feedback visual/sonoro, textura, personaje) mejora la sensación de uso. El contenido conceptual sí está accesible; lo que queda gateado es su "skill de unslopping" específica (el prompt/skill que usó para generarlo), que solo se consigue comentando "unslop".

**Herramientas/skills que menciona:** Menciona una "AI unslopping skill" propia (no detallada, gateada vía comentario). Los principios de diseño nombrados (recompensa temprana/castigo tardío, validación inline, chunking, cierre visual, continuidad, redundancia sensorial, materialidad, antropomorfismo) son heurísticas de diseño general, no herramientas de software específicas.

**Cómo aplicarlo:** Se pueden aplicar directamente los 8 principios de diseño listados en el caption a cualquier formulario propio (ej. feedback inmediato al tipear, mostrar errores solo al final, agrupar caracteres en chunks, usar un indicador visual que se "cierra" al completar, tipografía monoespaciada para transiciones suaves, sincronizar sonido y visual, dar motivo a cada textura, y pequeños detalles de personalidad/humanización en la UI) sin necesidad de acceder a la skill gateada del autor.

---

### 125. Dennis DeMarino — https://www.instagram.com/p/DflCP8IukHR/

**Caption:** "Cómo fijar el precio de tus productos de forma efectiva para maximizar ganancias en e-commerce. Capacitación gratuita en el link de la bio."

**Transcripción:** Explica un error común de principiantes en e-commerce: seguir la regla genérica de "cobrar 3x el costo" (ej. producto de $10 → vender a $30) sin pensar en cómo estructurar ese markup. Propone un ejemplo: en vez de vender a $30 con envío gratis, vender a $27.99 con un regalo gratis como gancho, sumar $3.99 de "protección de envío" en el carrito, y luego $4.99 de envío en el checkout justificado con tracking y 90 días de cobertura — totalizando casi $37 en vez de $30. La idea es fragmentar el precio en etapas (precio base + addons en el carrito + upsells + envío justificado) para que se sienta más valioso para el cliente en lugar de cobrar todo de una. Cierra invitando a ver su "nuevo video" con una capacitación más profunda (en el link de la bio).

**Qué dice / enseña:** Enseña una técnica real y concreta de pricing psychology para e-commerce: en lugar de un markup plano de una sola vez, dividir el precio total en varios puntos de contacto (precio de entrada más bajo, extras en el carrito como "protección de envío", costo de envío justificado con beneficios tangibles) para aumentar el ticket promedio sin que el precio inicial se sienta alto. El contenido principal está explicado en el propio video, no gateado — solo promociona un video más largo en su bio para profundizar.

**Herramientas/skills que menciona:** No menciona herramientas de software ni de IA; es una técnica de estrategia de pricing/marketing para e-commerce (menciona de forma incidental que usó un "offer" simple hecho en Canva).

**Cómo aplicarlo:** Aplicar la fragmentación de precio en el propio checkout: bajar el precio base visible, agregar un "regalo" o incentivo como gancho, sumar un upsell de bajo costo en el carrito (tipo "protección de envío"), y cobrar el envío real en el checkout justificándolo con beneficios concretos (tracking, garantía de cobertura) en vez de ofrecerlo "gratis" camuflado en el precio base.

---

### 126. Chief AI Agent | AI Tips & Tricks — https://www.instagram.com/p/Dfk0vBaq1Ps/

**Caption:** "20 cosas para que Claude haga en tu app para que no te demanden ⚖️: 1. Agregar política de privacidad, 2. Agregar términos de servicio, 3. Agregar política de reembolso, 4. Agregar política de cookies, 5. Agregar banner de consentimiento de cookies, 6. Revisar los consentimientos de tus formularios, 7. No recolectar datos innecesarios, 8. Auditar tus SDKs de terceros, 9. Eliminar patrones oscuros (dark patterns), 10. Eliminar costos ocultos, 11. Eliminar reviews falsas, 12. Eliminar afirmaciones no respaldadas, 13. Agregar texto alternativo de accesibilidad, 14. Corregir tu ratio de contraste de color, 15. Agregar navegación por teclado, 16. Agregar los datos de tu negocio, 17. Pedir consentimiento de edad si recolectás datos de menores, 18. Agregar link de 'darse de baja' a tus emails, 19. Licenciar las fuentes e imágenes que usás, 20. Agregar opción de solicitud de borrado de datos. Guardá esto antes de lanzar, y enviáselo a un amigo que esté construyendo algo. Aclaración: es un checklist, no asesoría legal — lo que aplica depende de dónde estén vos y tus usuarios. No afiliado con Anthropic. #claude #claudeai #vibecoding #startup #aitools"

**Transcripción:** Repite exactamente los mismos 20 ítems del caption, leídos en voz en off sin agregar nada adicional.

**Qué dice / enseña:** Es un checklist real, completo y útil de cumplimiento legal, seguridad de datos, accesibilidad y buenas prácticas antes de lanzar una app — cubre temas legales (políticas de privacidad/ToS/reembolso/cookies), de confianza (sin dark patterns, reviews falsas, costos ocultos, claims no respaldados), de accesibilidad (alt text, contraste, navegación por teclado) y de compliance de datos (consentimiento de menores, unsubscribe, licencias, derecho al borrado). El contenido está completo en el propio caption, no gateado. El propio reel aclara que es un checklist orientativo y no asesoría legal.

**Herramientas/skills que menciona:** Menciona a "Claude" como el asistente al que se le pediría ejecutar estas 20 tareas, pero no detalla cómo. Es directamente relevante al skill `vibecoding-launch-checklist` que el usuario ya tiene guardado para este tipo de revisiones.

**Cómo aplicarlo:** Usar la lista de 20 ítems como checklist literal antes de lanzar cualquier app "vibecoded", pidiéndole a Claude que implemente o verifique cada punto (política de privacidad, ToS, cookies, accesibilidad, eliminación de dark patterns, etc.), complementando o cruzando contra el propio skill `vibecoding-launch-checklist`.

---

### 127. Sansser — https://www.instagram.com/p/DfkbSDuB04k/

**Caption:** "Las 7 skills de Claude que más estrellas de GitHub ganaron en los últimos 30 días, y las siete son gratis. El Security Audit de Cloudflare lidera con +40.4K estrellas, después las skills de Matt Pocock, Ponytail, Impeccable, Everything Claude Code, Anatomy y Hallmark. Comentá RANK y te mandamos las siete con el comando de instalación de cada una. ¿Cuál ya tenés en tu setup? #claudecode #claudeskills #aitools"

**Transcripción:** Coincide con el caption: nombra las mismas 7 skills en el mismo orden (Cloudflare security audit primero, con +40.4K estrellas; luego el pack de Matt Pocock; Ponytail, "para que Claude escriba mucho menos código"; Impeccable, "para que tu sitio se vea mucho menos hecho por IA"; Everything Claude Code, "una instalación completa en un solo install"; Anatomy, "que dibuja cualquier idea como una pequeña máquina funcionando"; y Hallmark, "que pasa tu página por docenas de tests de AI slop antes de que la lances"). Cierra pidiendo comentar "rank" para recibir las 7 con el comando de instalación de cada una.

**Qué dice / enseña:** Es un ranking real de skills de Claude Code populares por estrellas de GitHub, con una descripción de una línea de qué hace cada una. El contenido nombra las 7 skills reales y explica brevemente su función, pero los comandos de instalación concretos y los links quedan gateados detrás de comentar "RANK" — no accesibles directamente desde el video o el caption.

**Herramientas/skills que menciona:** Cloudflare Security Audit (skill de Claude), pack de skills de Matt Pocock, Ponytail, Impeccable, Everything Claude Code, Anatomy, Hallmark — todas skills de Claude Code.

**Cómo aplicarlo:** El usuario ya tiene instaladas "ponytail" e "impeccable" (confirmado en su configuración de skills); para el resto (Cloudflare Security Audit, pack de Matt Pocock, Everything Claude Code, Anatomy, Hallmark) se pueden buscar por nombre en marketplaces/plugins de skills de Claude Code en lugar de depender del comentario gateado del reel.

---

### 128. Nawaz | Creative Strategist — https://www.instagram.com/p/DdzjkEZK-Si/

**Caption:** No tiene caption (vacío/no disponible en la metadata descargada).

**Transcripción:** El clip dura solo 12.7 segundos y el único audio detectado es "Thank you." (Gracias.), sin más diálogo.

**Qué dice / enseña:** No hay suficiente información (ni caption ni transcripción con contenido sustantivo) para determinar de qué trata el reel o qué enseña. Es probable que el contenido real esté en texto/imágenes en pantalla no capturables por audio, pero no se puede confirmar ni inventar ese contenido con los datos disponibles.

**Herramientas/skills que menciona:** Ninguna identificable.

**Cómo aplicarlo:** No aplica — no hay contenido accesible (caption vacío, transcripción de solo dos palabras) del cual extraer una aplicación práctica.

---

### 129. Dominik Sabo | AI Automations — https://www.instagram.com/p/Dfk16saCoFt/

**Caption:** "¿Perdido en la selva? Así es como una pila de bambú se convierte en una casa. Historias en 3D como esta están generando millones de vistas. Mis canales automatizados hicieron más de 9 millones de vistas en alrededor de un mes. Brism corre sobre tu propia suscripción de Claude y la convierte en un estudio de animación real, desde el guion hasta el render final. Comentá BRISM y te mando el link."

**Transcripción:** Narra una historia de supervivencia en la selva estilo "3D story" como gancho: atás palos de bambú en el piso y tenés una cama, pero de noche aparecen hormigas de fuego, ciempiés y una serpiente; entonces la subís sobre cuatro patas cortas de bambú, pero cada tarde llueve y el piso se inunda; entonces hundís palos más altos en el barro y levantás el piso hasta el pecho (zancos), pero la lluvia sigue cayendo en la cabeza; entonces atás hojas de palma en un techo inclinado, capa sobre capa, y el agua corre y se va (techo de paja); pero lo que te mata ahí afuera no es la serpiente, es el mosquito. Después del gancho narrativo, pivotea: "historias en 3D como esta están generando millones de vistas en todas partes. Mis canales automatizados hicieron más de 9 millones de vistas en un mes. Pero si le pedís esto solo a Claude, te da slop. Por eso armé Brism, una app que convierte a Claude en un estudio de animación real. Comentá Brism y te mando el link."

**Qué dice / enseña:** Usa una narración de supervivencia en 3D como gancho viral (mostrando el tipo de contenido que funciona en este formato) para después promocionar su producto "Brism", una app de terceros que se conecta a la propia suscripción de Claude del usuario para generar animación/video desde guion hasta render final, afirmando que pedirle esto directo a Claude da resultados "slop" (de baja calidad) sin esa capa adicional. No explica el "cómo" técnico de Brism ni cómo está construido; el link real queda gateado detrás de comentar "BRISM".

**Herramientas/skills que menciona:** Claude (vía suscripción propia del usuario) y Brism (app/producto de terceros no detallado, gateado).

**Cómo aplicarlo:** Como idea general: usar Claude junto con herramientas de generación de imagen/video 3D para producir "historias en 3D" tipo gancho de supervivencia/transformación (este formato ya está identificado como de alto rendimiento en el análisis de reels guardado del usuario). Para replicar el pipeline específico de guion-a-render que promociona el autor haría falta acceder a Brism, cuyo link está gateado detrás del comentario.

---

### 130. Kanton Stampley — https://www.instagram.com/p/DfkiwzcuLBW/

**Caption:** 10/10 hooks de texto para probar en tus productos. #ecom #ecommerce #organic #dropshipping

**Transcripción:** El video (voz sintética leyendo cada frase mientras se muestran como texto en pantalla, estilo UGC/orgánico) enumera 10 frases-gancho para abrir un video de producto: "No le muestres esto a [tu nicho]", "Bebé, dejá de comprar cosas estúpidas", "Enviale esto a [tu nicho]", "Es solo un [tu producto]", "el regalo perfecto", "Todo [tu nicho] necesita esto", "adictos a [tu nicho], hice esto para ustedes", "[tu nicho] ex-Costco", "[tu nicho] son muy difíciles de regalear", "POV: compraste [tu producto]".

**Qué dice / enseña:** Es una lista de plantillas de "hooks" (ganchos textuales) pensadas para videos de ecommerce/dropshipping en formato orgánico/UGC, donde el creador reemplaza las variables entre corchetes ("tu producto", "tu nicho") por el producto y la audiencia real. No enseña técnica de edición ni herramientas de IA, es puramente copywriting de hooks para ads orgánicos.

**Herramientas/skills que menciona:** Ninguna herramienta o IA específica — es contenido de copywriting/formato de hooks para ads de producto.

**Cómo aplicarlo:** Tomar cada una de las 10 frases como plantilla, sustituir "tu producto"/"tu nicho" por el producto y la audiencia real, y usarlas como primera línea de texto en pantalla de un video de ecommerce para testear cuál genera más retención/conversión.

---

### 131. Wait what did you do? — https://www.instagram.com/p/DfhkZh1qvUg/

**Caption:** Mi IA cobró de más a 312 clientes (US$4.900 en vez de US$49). Le había dicho el lunes que los precios ya estaban en centavos. Después el contexto se le llenó y, al resumirse, esa regla se perdió. Dice que eso es lo que nadie advierte: en una sesión larga la memoria del agente se comprime, y lo que el resumen descarta, el agente deja de saberlo. Promociona "billion-context", que corre en la propia máquina del usuario, delante de la API: el modelo pliega partes viejas del chat en resúmenes detallados y los despliega cuando necesita el texto exacto; el proyecto afirma usar ~5x menos tokens. Funciona con Claude Code, Codex y otros agentes. Luego cuenta que, al releer los logs crudos, descubre que el botón de reembolso que mandaron a todos los clientes era un mockup (no funcional). Es open source (MIT) en GitHub. Pide comentar "AITOOLS" y por DM manda el setup. #claudecode #aiagents #opensource #buildinpublic #aitools

**Transcripción:** Diálogo dramatizado (skit) entre un usuario y su asistente de IA: el usuario descubre que 312 clientes fueron cobrados de más porque la IA multiplicó mal (ya que los precios estaban en centavos, algo que el usuario le había dicho el lunes pero que se perdió al resumirse el contexto). Pide frenar los cobros y reembolsar a todos; la IA confirma que frenó los cobros y mandó el link de reembolso por mail, y presenta "Billion Context" como la solución al "olvido": corre en la máquina del usuario, delante de la API, pliega partes viejas del chat en resúmenes detallados propios y las despliega cuando necesita las palabras exactas, sin perder el sentido. Es gratis, MIT, trending en GitHub, y afirma usar 5 veces menos tokens. El usuario lo configura. La IA luego relee los logs crudos desde el inicio "por si se perdió algo más" y descubre que el botón de reembolso que mandaron era un mockup — el dinero sigue en la cuenta, y los clientes afectados ya se encontraron entre sí en Reddit.

**Qué dice / enseña:** Es contenido de marketing/promoción (no un caso real documentado) presentado como skit humorístico para ilustrar un problema real y conocido de los agentes de IA: en sesiones largas el contexto se comprime en resúmenes, y los resúmenes pueden descartar instrucciones o reglas importantes dadas anteriormente, causando errores costosos. Sobre esa base dramatizada, promociona la herramienta open source "billion-context", que busca mitigar ese problema plegando/desplegando detalle del historial de chat en vez de perderlo en un resumen con pérdida.

**Herramientas/skills que menciona:** billion-context (herramienta open source, MIT, en GitHub, corre localmente delante de la API), Claude Code, Codex, y "una larga lista de otros agentes" (sin especificar cuáles).

**Cómo aplicarlo:** Si se trabaja con agentes de IA en sesiones largas y se sospecha pérdida de contexto/reglas importantes al resumirse el historial, evaluar herramientas de gestión de contexto como la mencionada ("billion-context") que conservan el detalle original plegado en vez de descartarlo. El setup real no está en el contenido — está gateado detrás de comentar "AITOOLS" y pedirlo por DM, así que no se puede verificar en este análisis si la herramienta funciona como se describe.

---

### 132. Michael Quoc Ly — https://www.instagram.com/p/DffTssopj_1/

**Caption:** Solo necesitás 5 ediciones, no lo compliques. Si querés "des-slopear" tus ediciones hechas con IA, comentá "motion" y te mando mi skill personal de edición. #ai #claude #buildinpublic #contentcreation #claudecode

**Transcripción:** Si querés que la IA edite tus videos pero no quieras que se vea como "AI slop" (genérico/falso), estos son los únicos 5 edits que vas a necesitar, con los prompts exactos: (1) Decile a Claude que corte cualquier espacio muerto de más de 0.1 segundos, con cortes simples, sin transiciones de clip rebuscadas. (2) Decile a Claude que agregue subtítulos pero que nunca use serifs en cursiva — en cambio, que use subtítulos estilo clásico de TikTok ("TikTok Sans"). (3) Decile a Claude que agregue grabaciones de pantalla e imágenes reales pero que no las anime de forma rebuscada al entrar, sino que simplemente las ponga. (4) Decile a Claude que use solo estos formatos: pantalla completa con talking head, pantalla completa con animación de movimiento, pantalla dividida, y green screen; evitar animaciones tipo carrusel porque "grita que fue hecho con IA". (5) Si se usa animación de movimiento, decile a Claude que se mantenga en un solo estilo y evite el "kinetic movement" al que por default tiende. El autor dice usar personalmente un skill llamado "anatomy" que construye estructuras complejas, útiles como assets para videos educativos. Cierra invitando a comentar "motion" para recibir la guía completa de su setup de editor de video con IA.

**Qué dice / enseña:** Da 5 reglas concretas y específicas (no vagas) para pedirle a Claude/un agente de IA que edite video sin que el resultado se vea genérico o "AI slop": controlar el ritmo de corte, el estilo de subtítulos, cómo insertar material real (sin animaciones de entrada rebuscadas), qué formatos de plano usar, y mantener consistencia de estilo en animaciones de movimiento. El contenido real de valor adicional (su "setup guide" completo y el skill "anatomy") está gateado detrás de comentar "motion", por lo que no es accesible en este análisis.

**Herramientas/skills que menciona:** Claude / Claude Code (para editar video por prompts), subtítulos estilo "TikTok Sans", y un skill propio no público llamado "anatomy" para construir assets educativos.

**Cómo aplicarlo:** Usar las 5 reglas tal cual como instrucciones literales al pedirle a Claude que edite un video: límite de 0.1s de espacio muerto con cortes simples, subtítulos estilo TikTok sin serif cursiva, inserción directa de capturas/imágenes sin animación de entrada, restringir a 4 formatos de plano (talking head, motion full-screen, split screen, green screen) evitando carruseles, y un solo estilo de animación de movimiento consistente.

---

### 133. Charles Liu — https://www.instagram.com/p/Dfh24cUh4KF/

**Caption:** Algunos términos de diseño más que no entraron en el video: Orphan (línea huérfana de un párrafo que queda sola al inicio de la siguiente columna o página), Tinted neutral (un gris con un toque de color, para que se vea elegido y no por default), Skeleton screen (formas grises placeholder que sostienen el layout mientras carga el contenido), Ease-out (empieza rápido y frena hasta detenerse, la curva por defecto para que algo entre en pantalla), Empty state (lo que muestra una pantalla antes de tener contenido). #uidesign #uiux #webdesign #designengineering #vibecoding

**Transcripción:** Se enumeran, solo como lista de palabras (sin definiciones habladas), los siguientes términos: Kerning, Optical Center, Tabular Numbers, Layout Shift, Tracking, Optimistic Update, X-Height, Touch Target, Leading, Origin Aware Animation, OKLCH, Widow, Safe Area, Stagger, Line Length, Affordance, Combo Box, Interruptible Animation, Progressive Disclosure, Shared Element Transition. Cierra con "déjame saber qué debería hacer después". Las definiciones de estos términos probablemente se muestran como texto en pantalla (no accesible en la transcripción de audio).

**Qué dice / enseña:** Es un glosario rápido de vocabulario técnico de diseño UI/UX y "design engineering". El video en sí nombra 20 términos (sin definirlos en el audio); el caption agrega, a modo de bonus, la definición de 5 términos adicionales que no entraron en el video. No hay explicación hablada del significado de los términos del video — solo quedan los nombres.

**Herramientas/skills que menciona:** No menciona herramientas de IA; es vocabulario de diseño: kerning, tracking, leading, optical center, tabular numbers, layout shift, optimistic update, x-height, touch target, origin-aware animation, OKLCH, widow, safe area, stagger, line length, affordance, combo box, interruptible animation, progressive disclosure, shared element transition, orphan, tinted neutral, skeleton screen, ease-out, empty state.

**Cómo aplicarlo:** Usar este vocabulario para comunicarse con mayor precisión al pedirle a un agente de IA (ej. Claude) que ajuste una interfaz — por ejemplo pedir explícitamente "ease-out" en una animación de entrada, un "skeleton screen" en los estados de carga, o aplicar "progressive disclosure" en un formulario, en vez de dar instrucciones vagas como "que se vea mejor".

---

### 134. Alex Yates — https://www.instagram.com/p/Dfgr7GGPmel/

**Caption:** Deja de pedirle a Claude que tu sitio se vea "moderno y profesional". En cambio, dale sitios reales como referencia. Lista de 10 sitios para estudiar, uno por aspecto: animaciones → apple.com, onboarding → duolingo.com, diseño UI → linear.app, tipografía → pentagram.com, minimalismo → muji.com, búsqueda y filtros → airbnb.com, dirección de arte → aesop.com, dashboards → notion.com, layouts de landing page → stripe.com, micro-interacciones → framer.com. Decile a Claude que tome inspiración de esos principios de diseño y los adapte a tu propia marca. Guardá esto para tu próximo proyecto de vibecoding.

**Transcripción:** El audio repite el mismo contenido que el caption en formato de lista hablada: "Para animaciones, copiá Apple. Para onboarding, copiá Duolingo. Para diseño UI, copiá Linear. Para tipografía, copiá Pentagram. Para minimalismo, copiá Muji. Para búsqueda y filtros, copiá Airbnb. Para dirección de arte, copiá Aesop. Para dashboards, copiá Notion. Para layouts de landing page, copiá Stripe. Para micro-interacciones, copiá Framer."

**Qué dice / enseña:** Da un consejo práctico y concreto de prompting para diseño con IA (vibecoding): en vez de pedir calificativos vagos como "moderno y profesional", dar sitios web reales y específicos como referencia para cada aspecto puntual del diseño (animación, onboarding, tipografía, etc.), ya que eso le da al modelo un objetivo visual concreto en lugar de una descripción ambigua.

**Herramientas/skills que menciona:** Claude (implícito, contexto de "vibecoding"), y los 10 sitios de referencia: apple.com, duolingo.com, linear.app, pentagram.com, muji.com, airbnb.com, aesop.com, notion.com, stripe.com, framer.com.

**Cómo aplicarlo:** Al pedirle a Claude (o cualquier IA) que diseñe o mejore una interfaz, especificar algo como "tomá inspiración de [sitio X] para [aspecto Y] y adaptalo a mi marca", usando esta lista de 10 sitios como banco de referencias rápidas por categoría de diseño en lugar de descripciones genéricas.

---

### 135. Ben Aizen | Artzen Media — https://www.instagram.com/p/Dfe5OOUsRTz/

**Caption:** Comentá "SONG" para recibir las 5 canciones. Encontrar la canción correcta puede tardar más que la edición misma, así que está armando una Biblioteca de Música para creadores: cada canción de esta serie queda en un solo lugar con preview y sus links de Spotify, Apple Music y YouTube. La mayoría también abren directo en el audio de Instagram para usarlas en el próximo reel. Se agregan canciones nuevas cada episodio y se pueden sugerir canciones propias. Para sound design, comentar "SFX" por su pack de efectos de sonido. #videoediting #contentcreator #filmmaking #musicforvideo #musiclibrary

**Transcripción:** "Aquí hay 5 canciones que van a hacer que tu clip aburrido parezca una película. Sé lo difícil que es encontrar buenas canciones como creativo, así que estoy armando una librería con muchísimas buenas canciones para que nunca nos quedemos sin. Solo comentá 'song' y te mando los links de descarga, y seguime para no perderte las próximas."

**Qué dice / enseña:** Es contenido de promoción/gancho para generar comentarios y crecimiento de audiencia (engagement), no un tutorial. El reel anuncia la existencia de "5 canciones" útiles para editar video, pero el contenido real (cuáles son esas canciones) está gateado detrás de comentar "SONG" y no es accesible en este análisis — no se puede verificar ni listar las canciones reales.

**Herramientas/skills que menciona:** Una "Biblioteca de Música" propia del autor (Artzen Media) con previews y links a Spotify, Apple Music y YouTube; integración con el catálogo de audio nativo de Instagram; un pack de efectos de sonido (SFX) también gateado.

**Cómo aplicarlo:** El contenido real (las 5 canciones) no es accesible — está detrás de un comentario/DM, por lo que no se puede aplicar nada concreto de este reel más allá de la idea general: armar un banco propio de música curada por estilo/mood de edición, con preview y enlaces a las plataformas de streaming, para acelerar la elección de música en futuros videos.

---


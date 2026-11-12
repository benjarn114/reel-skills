# Reel Skills

Dos [Claude Code skills](https://docs.claude.com/en/docs/claude-code/skills) destiladas del análisis de 113 reels de Instagram guardados sobre IA/Claude, vibecoding, marketing y edición de video corto. En vez de guardar cada reel como una nota suelta, se comparó el contenido repetido entre creadores, se descartó lo redundante, y se consolidó lo validado en dos skills reusables.

## Skills

- **[`reel-script-writer`](skills/reel-script-writer/SKILL.md)** — hooks, estructuras de guion, sound design, formatos de ad, frameworks de funnel de contenido y catálogos de formatos de anuncio para reels/shorts/TikToks.
- **[`vibecoding-launch-checklist`](skills/vibecoding-launch-checklist/SKILL.md)** — checklist de seguridad, pagos, CI/CD, legal y pulido de UX antes de lanzar una app hecha mayormente con un agente de IA ("vibecoded").

## Cómo instalarlas

Copiá la carpeta de la skill que quieras a `~/.claude/skills/` (o a `.claude/skills/` dentro de un proyecto):

```bash
git clone https://github.com/<tu-usuario>/reel-skills.git
cp -r reel-skills/skills/reel-script-writer ~/.claude/skills/
cp -r reel-skills/skills/vibecoding-launch-checklist ~/.claude/skills/
```

Claude Code las detecta automáticamente y las usa cuando el pedido encaja con lo que describe cada skill (escribir un guion de reel, revisar seguridad antes de lanzar algo, etc.).

## El análisis completo

- [`DOCUMENTO.md`](DOCUMENTO.md) — las 113 fichas de análisis (cuenta, caption, transcripción, qué enseña, cómo aplicarlo) que son la fuente de cada ítem de las skills. Cada ítem de las skills cita el número de post de donde salió.
- [`cosas-para-tener-en-cuenta.md`](cosas-para-tener-en-cuenta.md) — todo lo que no se convirtió en skill (vocabulario de prompts para imagen/video con IA, teoría de color, microinteracciones de UI, herramientas mencionadas pero gateadas detrás de "comentá para que te lo mande por DM").

No se incluye el audio/video descargado de los reels originales (son ~64MB y no hay motivo para redistribuirlos) — solo texto de caption y transcripción, usados para el análisis.

## Todo mi setup de Claude Code

- [`my-claude-setup/`](my-claude-setup/) — todas las skills instaladas a nivel usuario (menos las que ya vienen por default con Claude Code), la lista de plugins instalados con su marketplace de origen, y el `CLAUDE.md` global. Pensado para reinstalar todo en otra PC — ver [`my-claude-setup/PLUGINS.md`](my-claude-setup/PLUGINS.md) para los pasos. No incluye API keys, settings.json ni nada de otras carpetas/proyectos personales.

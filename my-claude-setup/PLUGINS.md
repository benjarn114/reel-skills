# Plugins instalados (vía marketplace)

Estos plugins NO se copian como archivos (son cachés de ~350MB clonadas de GitHub) — se reinstalan apuntando a su marketplace de origen. En una Claude Code nueva:

```bash
/plugin marketplace add obra/superpowers-marketplace
/plugin install superpowers@superpowers-marketplace

/plugin marketplace add thedotmack/claude-mem
/plugin install claude-mem@thedotmack

/plugin marketplace add bayramannakov/claude-reflect
/plugin install reflect-mod@claude-reflect-marketplace

/plugin marketplace add johnnyvizz/claude-kit
/plugin install savvy-progress@claude-kit
/plugin install savvy-flow@claude-kit

/plugin marketplace add DietrichGebert/ponytail
/plugin install ponytail@ponytail
```

| Plugin | Marketplace (repo GitHub) | Versión al momento de exportar |
|---|---|---|
| superpowers | obra/superpowers-marketplace | 7.0.1 |
| claude-mem | thedotmack/claude-mem | 15.0.1 |
| reflect-mod | bayramannakov/claude-reflect | 3.3.0 |
| savvy-progress / savvy-flow | johnnyvizz/claude-kit | (ver marketplace) |
| ponytail | DietrichGebert/ponytail | (ver marketplace) |

## No portable por marketplace

- **blast-radius** corre desde un marketplace de tipo `directory` apuntando a una carpeta local (`claude-code-playground/claude-code/mods`), no un repo de GitHub — no se puede reinstalar con `/plugin marketplace add`. Si lo usás en la otra PC, copiá esa carpeta de mods a mano y agregala como marketplace local ahí.

## Skills (carpeta `skills/` de este repo)

Son las skills a nivel usuario (`~/.claude/skills/`), copiadas tal cual — no son plugins, son solo archivos (`SKILL.md` + scripts/referencias). Para instalarlas en la otra PC:

```bash
cp -r my-claude-setup/skills/* ~/.claude/skills/
```

No se incluyó la carpeta `synced/` (son las skills que Anthropic ya empaqueta con Claude Code por default — docx, pdf, pptx, xlsx, google-workspace, skill-creator, etc. — se sincronizan solas, no hace falta copiarlas).

## CLAUDE.md

`my-claude-setup/CLAUDE.md` es una copia de las instrucciones globales (`~/.claude/CLAUDE.md`). Pegalas en el mismo lugar en la otra PC si querés las mismas reglas/notas activas.

No se incluyó `settings.json` (tiene referencias a rutas y proyectos de otras carpetas personales que no corresponde compartir acá) — revisá `enabledPlugins` arriba y configurá manualmente lo que corresponda.

# Business Brain — ChimeraNext

Vault Obsidian (tool-agnóstico: Markdown en Git) que es la **fuente de verdad** del negocio.
Construido a partir del volcado Notion "Plantilla de Inicio" → DB "Departamentos Vertical #1".

## Metodología: CODE
Capture → Organize → Distill → Express. Notas atómicas (`Zettelkasten`), navegación por
**MOCs** (`_MOC.md` por unidad), capa de acción **PARA** en frontmatter (nunca en carpetas).

## Estructura
| Carpeta | Unidad |
|---|---|
| `0-gerencia/` | Gobernanza, estrategia, cumplimiento legal |
| `1-operaciones/` | Operaciones, cadena de suministro, talento |
| `2-ingenieria-producto/` | Tecnología e informática |
| `3-experiencia-cliente/` | Comercial, marketing, cliente |
| `identidad-marca/` | Las 6 identidades de marca |
| `4-finanzas/` | Finanzas y contabilidad |
| `_capitulos/` | Síntesis por capítulos (MOCs cross-unit) |
| `_templates/` | Plantillas de notas |
| `_procedimientos/` | SOPs versionados |
| `_retros-minutas/` | Retrospectivas y minutas |
| `_sources/` | Fuentes brutas e inmutables |
| `00-inbox/` | Zona de captura |

## Operación
- El agente lee `CLAUDE.md` y `index.md` PRIMERO.
- Frontmatter obligatorio (id, title, aliases, type, unidad, para, status, date, tags, sources).
- Regla de rigor: solo fuentes internas; sin fuente → `type: supuesto`.
- Barrido semanal de `00-inbox/` y `_sources/`; commit descriptivo por cambio.

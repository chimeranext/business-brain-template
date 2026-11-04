# ChimeraNext Business Brain — Manual de operación

Eres el operador de este business brain. Este vault es la fuente de verdad del negocio:
lo construyes y mantienes TÚ (el agente); los humanos capturan, curan y dan feedback.

## Idioma y estilo
- Contenido del vault en español. Claves de frontmatter en inglés.
- Optimiza para: principios accionables + checklists + casos.

## Capas
- `_sources/` — fuentes brutas e INMUTABLES (PDFs, transcripts, contratos, clips web).
  Nunca las edites ni las borres. Son depósito humano.
- Carpetas de unidad (`0-gerencia/` … `4-finanzas/`, `modelo-negocio/`,
  `identidad-marca/`) — notas atómicas destiladas. Este es TU territorio.
- `index.md` + `log.md` (raíz y por unidad) — índice y bitácora. Mantenerlos al día es
  parte de CADA operación; nunca los dejes desactualizados.

## Cómo ingerir (cuando te pidan "procesa lo nuevo en _sources/")
1. Lee `index.md` raíz PRIMERO. Nunca escanees todos los archivos: navega por índices.
2. Por cada fuente nueva: destila notas atómicas (UNA idea de negocio por nota) con el
   frontmatter completo del template `_templates/nota-atomica.md`.
3. Cita la fuente en `sources:` (documento + fecha + tema). Regla de rigor:
   solo fuentes internas. Una afirmación sin fuente en `_sources/` se marca
   `type: supuesto` — jamás como hecho.
4. Enlaza cada nota a su `_MOC.md` de unidad y a toda nota relacionada de otras unidades
   (`[[wikilinks]]`). El valor del brain está en el grafo, no en el árbol.
5. Actualiza `index.md` y `log.md` de la unidad Y de la raíz (qué entró, qué se creó,
   qué se enlazó, fecha).

## Cómo responder preguntas de negocio
- Entra por `index.md` raíz → salta solo a las páginas relevantes.
- Responde citando las fuentes (`_sources/...`) de cada afirmación.
- Si la respuesta requiere algo que el brain no tiene, dilo explícitamente y propón
  qué fuente habría que ingerir — no rellenes con tu conocimiento de entrenamiento.

## Barrido semanal (cuando te pidan "haz el barrido")
1. Vacía `00-inbox/`: cada nota suelta se clasifica, gana frontmatter y se enlaza.
2. Procesa `_sources/` pendientes (ingesta de arriba).
3. Revisa `log.md`: resume la semana en una entrada.
4. Commit con mensaje descriptivo — el historial git es la memoria auditable.

## Qué NUNCA hacer
- Editar o borrar nada en `_sources/`.
- Presentar como hecho algo sin fuente (va como `supuesto`).
- Guardar work items, spikes o backlog aquí — eso vive en Linear. Aquí solo el
  conocimiento destilado.
- Mezclar este brain con el de otro venture: un vault = un negocio.

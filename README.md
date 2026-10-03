# IEEE Access Review

Skill en español para revisar manuscritos propios o autorizados antes de enviarlos a IEEE Access. Combina lineamientos oficiales, ejemplos publicados y evaluación metodológica proporcional a las afirmaciones del artículo.

**Proyecto independiente, sin afiliación ni respaldo de IEEE.** Sus informes son asesoría previa al envío, no dictámenes editoriales ni garantías de aceptación.

## Qué revisa

- Contribución y correspondencia entre afirmaciones, evidencia y conclusiones.
- Diseño experimental, estadísticas, métricas y reproducibilidad.
- Figuras, tablas, referencias y declaraciones sobre participantes y asistencia de IA.
- Diferencias entre requisitos oficiales, prácticas observadas y mejoras opcionales.

Incluye orientación específica para sistemas RAG y servicios conversacionales. No exige métricas adicionales sin una afirmación que las justifique.

## Instalación local

Clona este repositorio en una carpeta nueva dentro de tu directorio personal de skills:

```sh
git clone https://github.com/RenzoLenes/ieee-access-review.git ~/.codex/skills/ieee-access-review
```

Si esa carpeta ya existe, conserva tu versión antes de reemplazarla. La skill necesita acceso al manuscrito y a sus evidencias; para actualizar políticas requiere navegación web. No necesita claves API propias ni incluye scripts que envíen documentos.

## Uso

```text
Usa $ieee-access-review para revisar este manuscrito antes de enviarlo a IEEE Access.
Indica el fragmento afectado, la evidencia, el motivo, la prioridad y cómo resolver cada hallazgo.
Distingue cambios de redacción, comprobaciones con datos existentes y experimentos nuevos.
```

Para calibrar la revisión, proporciona artículos comparables y solicita que las observaciones incluyan su página de referencia. Por defecto, la revisión produce un informe y conserva el manuscrito.

## Contenido

- [SKILL.md](SKILL.md): instrucciones principales.
- [Fuentes oficiales](references/official-sources.md): políticas consultadas y enlaces para revalidarlas.
- [Evaluación de RAG](references/rag-evaluation.md): métricas vinculadas a afirmaciones.
- [Ejemplos publicados](references/published-exemplars.md): fichas críticas de cuatro artículos, con DOI, páginas y límites de comparación.
- [Metadatos de interfaz](agents/openai.yaml).

## Alcance de los materiales

Este repositorio contiene instrucciones y notas de análisis, no manuscritos privados, PDF de terceros, capturas, consentimientos ni registros de participantes. Las fichas no sustituyen la lectura de los artículos ni redistribuyen sus textos completos. Los materiales originales conservan los derechos de sus titulares.

Las políticas pueden cambiar: verificar las fuentes oficiales antes de un envío. Los cuatro ejemplos no representan toda la revista y no permiten estimar probabilidades o tiempos de aceptación. Las observaciones sobre ellos se limitan a las versiones examinadas; no se dispone de sus dictámenes editoriales.

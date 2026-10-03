---
name: ieee-access-review
description: Revisa manuscritos propios o autorizados antes de enviarlos a IEEE Access, contrastando políticas oficiales, ejemplos publicados comparables, evidencia experimental, estadísticas, figuras y reproducibilidad. Úsala para una revisión previa al envío o una revisión de cambios, sin presentarla como dictamen editorial real.
---

# Revisión previa a IEEE Access

## Alcance

Realiza una revisión crítica y trazable del manuscrito que el usuario autoriza a revisar. Es asesoría al autor, no revisión independiente asignada por IEEE. No atribuyas al journal umbrales de métricas, probabilidades de aceptación ni garantías de plazos. No uses este flujo para procesar manuscritos confidenciales de terceros recibidos como revisor editorial; consulta las restricciones pertinentes.

## Fuentes y jerarquía

Lee [fuentes oficiales](references/official-sources.md) y verifica en la web las políticas aplicables antes de cada revisión importante. Diferencia expresamente:
- requisito editorial confirmado y su URL;
- práctica observada en artículos publicados, con página y límites de comparabilidad;
- criterio metodológico propuesto por quien revisa;
- preferencia de presentación del autor.

Una recomendación de RAGAS, ablaciones o más datos no es automáticamente un requisito universal de IEEE. El alcance de la evidencia exigida debe corresponder a las afirmaciones del manuscrito. Para estudios RAG, lee [evaluación y métricas](references/rag-evaluation.md).

## Calibración con artículos publicados

Cuando haya ejemplos comparables o se solicite una revisión calibrada, consulta [casos publicados](references/published-exemplars.md). Selecciona por afirmación y unidad de evaluación, no por institución, prestigio o número de métricas. Accura orienta estudios de procesos completos; Mikael y Attigeri orientan comparaciones de modelos; EduPredict orienta separación de evaluación predictiva y percepción.

Las prácticas de cuatro casos no son requisitos editoriales ni una muestra representativa de decisiones. No se conocen sus informes de revisión. Revisa coherencia interna antes de tomar cifras como referencia. No compares un índice compuesto de calidad, accuracy, F1 y escalas de percepción como porcentajes intercambiables. Que un artículo omita algo no demuestra que sea prescindible en otro; que lo incluya no lo vuelve obligatorio.

Antes de pedir nuevos experimentos, determina qué afirmación concreta requieren. Distingue entre: datos existentes que necesitan mejor descripción, comprobación con evidencia conservada y experimentos nuevos. En un estudio de servicio completo, no exigir por defecto entrenar clasificadores alternativos, RAGAS, Recall@k, ablaciones, validación multisitio o jueces nuevos. Se vuelven pertinentes si el manuscrito reivindica superioridad del componente, mejor recuperación, reducción de alucinaciones o generalización que los datos actuales no prueban. Ofrece acotar la afirmación cuando sea científicamente suficiente, sin encubrir defectos que invaliden el resultado central.

Una muestra modesta o una limitación reconocida no son bloqueantes automáticos. Tampoco basta con reconocer una limitación para neutralizarla: valora si compromete la inferencia principal. Mantén separadas la integridad de datos, comparabilidad de mediciones y declaraciones éticas de las mejoras opcionales.

## Procedimiento

1. Identifica la versión exacta, tipo de artículo propuesto, afirmación principal (servicio completo, componente o ambos) y alcance de la revisión. Usa PDF y fuentes; identifica suplementos y registros disponibles. No mezcles versiones.
2. Construye un mapa de afirmación, evidencia, localización y límite. Distingue dato confirmado, afirmación del autor, resultado recalculado, información no verificada y evidencia ausente.
3. Aplica las preguntas editoriales de las fuentes oficiales. Examina aporte frente al trabajo cercano, validez del diseño, correspondencia de resultados/conclusiones, cobertura metodológica y referencias.
4. Audita ética y procedencia sin inferir aprobación institucional. La aceptación de un aviso de datos no demuestra por sí sola consentimiento para investigar. Si aparece un formulario, verifica proyecto, participantes, versión y uso; el nombre del archivo no prueba su pertinencia. Señala contradicciones y pide solo la aclaración decisiva; continúa la revisión independiente.
5. Recalcula cuando existan datos autorizados. Respeta unidad de análisis, emparejamiento, exclusiones, empates, correcciones y escala. No reconstruyas observaciones individuales a partir de medias. No trates capturas reales como demostración automática de calidad de las etiquetas.
6. Revisa PDF renderizado, no solo extracción textual: figuras al tamaño final, etiquetas, márgenes, ecuaciones, tablas y bibliografía. Para edición usa el flujo PDF disponible. No modifiques la clase oficial para esconder defectos.
7. Asigna severidad: bloqueante (impide sostener una afirmación central o completar una declaración exigida), mayor (requiere evidencia/análisis/descripción sustancial), menor (corrección local). Evita un promedio de puntuaciones que oculte bloqueantes.
8. Entrega hallazgos con ubicación, evidencia, por qué importa, acción concreta y criterio de cierre. Distingue correcciones posibles ahora, verificación documental y nuevas pruebas. Añade qué cambia respecto de una revisión anterior; no repitas como pendientes hallazgos ya resueltos en la versión activa. Explica fortalezas y límites de la auditoría.

## Resultado y cambios

Da una recomendación simulada coherente con las categorías vigentes del journal. Si harían falta cambios sustanciales, no presentes el trabajo como aceptable con retoques menores. No pronostiques qué decidirán los revisores reales.

Por defecto, una solicitud de revisión produce un informe, no cambia los datos ni sobrescribe el paper. Cuando el usuario autorice correcciones, trabaja en nueva versión, registra cambios, compila y verifica. No inventes consentimientos, exenciones, experimentos, valores, citas o validaciones. Conserva evidencia desfavorable y límites de alcance.

Las confirmaciones del usuario son evidencia declarada: atribúyelas y concílialas con el manuscrito; no las conviertas automáticamente en documentos institucionales verificados. No contactes editores ni envíes el manuscrito sin autorización explícita.

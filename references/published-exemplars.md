# Calibración con cuatro artículos publicados

Revisión: 2026-10-03. Fuente: PDF completos aportados por el usuario, con metadatos de IEEE Access. Se examinaron texto metodológico/resultados y páginas renderizadas relevantes. Los DOI se transcriben de los PDF; no se certifica aquí la autenticidad editorial mediante consulta independiente al editor. No se dispone de dictámenes, versiones rechazadas ni historial previo a la fecha Received. Las páginas siguientes son ordinales del PDF (primera = 1); entre paréntesis figura la página impresa.

## Selección por semejanza

| Caso y DOI | Qué se evalúa | Práctica transferible | Límite de transferencia |
|---|---|---|---|
| Accura, Guevara et al., 2026. 10.1109/ACCESS.2026.3723358 | Aplicación y proceso manual frente a automatizado | Integración aplicada, comparador operativo, denominadores claros | Detección estructural con errores controlados, no respuesta factual libre |
| EduPredict, Barboza et al., 2026. 10.1109/ACCESS.2026.3675564 | Cinco modelos predictivos y percepción de profesionales | Separar rendimiento objetivo de percepción, publicar cuestionario y límites | Registros predictivos y usuarios no equivalen a consultas RAG |
| Hybrid Chatbot, Mikael et al., 2025. 10.1109/ACCESS.2025.3552501 | Módulos individuales, clasificador y modelo híbrido | Separación de etapas, corpus temático, evaluación por tarea | Su afirmación de superioridad de modelos exige comparaciones que un estudio de servicio no hereda automáticamente |
| Advanced NLP, Attigeri et al., 2024. 10.1109/ACCESS.2024.3368382 | Cinco implementaciones y respuestas predefinidas | Pseudocódigo y pruebas por tipo de consulta | No valida generación factual sustentada en documentos |

## A. Accura

- P. 2 (131912), contribuciones: integra interpretación GPT-4o, reglas JSON y ejecución determinista; añade aplicación por roles y caso empírico. Evidencia de cómo se presenta una integración aplicada, no obligación de inventar un modelo.
- P. 4 (131914), III-B: entrada, contexto del prompt, esquema, comprobaciones, un reintento y manejo del fallo; reporta gpt-4o, SDK 2.8.0, temperatura 0.2 y 800 tokens. P. 5 incluye JSON ilustrativo. Enseñanza: explicar lógica y configuración, no solo nombres de archivos.
- PP. 11–12 (131921–131922), V-A–D y tablas 4–6: cuatro conjuntos, 400,779 registros, 49 reglas asociadas a plantillas y 50 participantes. PP. 13–14, V-E y figuras 15–16: los dos procedimientos usan datasets, plantillas y errores intencionales comunes.
- PP. 14–15 (131924–131925), VI: diferencia tiempos promedio por plantilla de métricas de detección agrupadas sobre 200 ejecuciones participante-plantilla. La exactitud de definición usa 35 reglas base (34 correctas con Accura); no confundir este denominador con 49 reglas asociadas a plantillas.
- P. 18 (131928): reconoce errores controlados, supervisión de generación, alcance estructural y ausencia de evaluación estandarizada de usabilidad a largo plazo. Comparar otros modelos queda en trabajo futuro. Publicación no demuestra que todos los diseños similares serán aceptados.
- Precauciones: la fórmula F1 de p. 13 multiplica por 100 tras definir PRC y REC también como porcentajes; hay una ambigüedad de escala que no debe copiarse. La declaración de consentimiento de p. 18 indica que no aplica: no trasladar esa declaración a otro estudio ni inferir exención para otro estudio.

## B. EduPredict

- PP. 8–9 (43759–43760), V-A–D: 1,464 registros iniciales, 1,456 tras excluir ocho; partición declarada 1,165/291. Separa esos registros de diez profesionales que evalúan la aplicación. Describe una capacitación de 30 minutos y uso autónomo por siete días.
- P. 12 (43763), tablas 6–11: variables, composición de datos, perfil de usuarios, diez preguntas por dimensión, fórmulas y parámetros. P. 17 (43768), tabla 15: respuestas y estadísticos por ítem.
- P. 17: alfa por dimensión 0.42, 0.05 y 0.21; el texto limita la interpretación a resúmenes descriptivos y reconoce muestra pequeña y una institución. Enseñanza: no exigir instrumento perfecto para presentar percepción exploratoria; no venderlo como escala validada.
- Precaución verificable: p. 8 describe distribución inicial 492/972 y preservación de esa distribución en test; p. 9 informa 146/145 en test. Esa diferencia requiere explicación; no usar este artículo para afirmar que su partición está inequívocamente validada. No se auditó su código.

## C. Hybrid Chatbot

- P. 4 (50744), III-A: fuentes, limpieza, organización en siete dominios y corpus descrito como 2,253 líneas de conversación; el abstract lo describe como pares pregunta-respuesta. Mantener esa diferencia de unidad, sin asumir equivalencia.
- PP. 7 y 13 (50747, 50753): 300 consultas para evaluación; p. 7 identifica encuesta a 267 estudiantes con diez preguntas. P. 5 menciona 113 usuarios del prototipo basado en reglas: no sumar muestras ni asumir que son cohortes independientes.
- P. 14 (50754), tablas 5–7: preguntas completas, dimensiones percibidas y cumplimiento por tipo de tarea.
- PP. 15–16 (50755–50756), tablas 8–10: evaluación de módulos, comparación de clasificadores y evaluación híbrida. Es un precedente para separar esos niveles, no para imponer todas sus métricas a otro estudio.
- Inconsistencias: abstract p. 1 y conclusión p. 18 afirman accuracy 97.57%; tabla 10 p. 16 indica 96.13% y TP=477, FP=7, FN=13, TN=21. Esos conteos producen aproximadamente 96.14%. Tabla 2 p. 13 muestra 210/300 = 73.33%, aunque el cociente es 70%. No interpretar cifras como objetivo de aceptación, ni reproducirlas sin atribuir la discrepancia.
- El juicio humano sobre respuestas generativas descrito en p. 13 usa un especialista; eso no acredita por sí solo acuerdo entre jueces ni hace innecesaria una rúbrica reproducible en el manuscrito evaluado.

## D. Advanced NLP

- P. 5 (29637), IV: preguntas de portales, estudiantes y docentes, respuestas de fuentes autorizadas; alrededor de 250 preguntas con variantes.
- PP. 7–9 (29639–29641): seis algoritmos para cinco implementaciones, acompañados de explicación de entradas, preprocesamiento y selección de respuesta. Aprovechar el vínculo entre algoritmo y explicación; no exigir seis algoritmos a cualquier paper.
- P. 10 (29642), V-A–C: declara conjunto de prueba de 144 consultas y análisis separado de 150 consultas, incluidas 15 con errores ortográficos; también menciona 250 consultas ejecutadas. P. 11 tabla 2 muestra aciertos por pregunta/modelo; pp. 11–13 presentan conversaciones simples y compuestas.
- Enseñanza: una matriz de tipos de consulta y ejemplos correctos/incorrectos puede reforzar un estudio de atención universitaria. No es necesario sumar nuevas personas para describir mejor las consultas ya conservadas.
- Precauciones: no reconciliar automáticamente los recuentos 250/144/150; distinguir las etapas. Las comparaciones de respuestas predefinidas no miden respaldo factual de un generador. P. 14, referencia 12, contiene example-url.com: demuestra la necesidad de comprobar bibliografía incluso en un ejemplo publicado; no prueba por sí solo nada sobre el resto de las referencias.

## Decisiones de revisión que estos casos modifican

1. Un aporte de integración puede evaluarse como servicio completo si se delimita qué se aprendió y se compara de forma pertinente. No exigir novedad algorítmica por defecto.
2. No fijar mínimos universales de participantes, consultas, accuracy, alfa o número de comparadores basándose en estos ejemplos. Los denominadores y propósitos difieren.
3. Exigir claridad sobre qué se midió y qué respalda cada conclusión. Hay buenos precedentes para publicar cuestionarios, ejemplos y unidades de análisis; son prioridades proporcionales en el manuscrito evaluado.
4. Proponer análisis de fuentes o clasificador como experimentos nuevos cuando se afirme su eficacia específica. Si la afirmación se limita al servicio, pueden permanecer como trabajo futuro.
5. No utilizar limitaciones o errores publicados para justificar errores propios. La calibración evita exigencias innecesarias, no elimina comprobaciones de coherencia.
6. Separar datos descargados, corpus de producción, datos de prueba y participantes; no compararlos como tamaños muestrales equivalentes.

## Metadatos temporales de los PDF

| Caso | Received | Accepted | Diferencia de fechas |
|---|---|---|---|
| Accura | 2026-06-21 | 2026-08-03 | 43 días |
| EduPredict | 2026-03-10 | 2026-03-15 | 5 días |
| Hybrid | 2025-02-03 | 2025-03-12 | 37 días |
| NLP | 2024-01-10 | 2024-02-17 | 38 días |

Son intervalos impresos de cuatro casos seleccionados. No estiman el plazo esperado, no incluyen necesariamente trámites previos y no garantizan aceptación en dos meses.

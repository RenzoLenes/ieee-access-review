# Evaluación de RAG y estudios de atención al usuario

Esta matriz es orientación metodológica de la skill, no una lista obligatoria de IEEE ni una regla de aprobación.

## Referencia metodológica primaria

Es et al., RAGAs: Automated Evaluation of Retrieval Augmented Generation, EACL 2024:
https://aclanthology.org/2024.eacl-demo.16/

Distingue evaluación de recuperación, fidelidad al contexto y calidad de respuesta. Un evaluador automático basado en LLM no sustituye sin validación a jueces humanos del dominio. No asumir equivalencia entre sus métricas y un índice propio del estudio.

## Vincular métricas con afirmaciones

| Afirmación | Evidencia pertinente | Precaución |
|---|---|---|
| El servicio completa mejor las tareas | Éxito por escenario, diferencia pareada e intervalo, rúbrica y ejemplos | Unidad independiente: participante si usa ambos sistemas; no contar cada turno como persona |
| Respuestas más correctas | Corrección frente a referencia institucional fechada; errores definidos; valoración independiente | Ausencia de errores identificados no prueba corrección exhaustiva |
| Recupera mejores documentos | Recall@k, precision@k, MRR o nDCG según etiquetas y objetivo | Requiere consultas y relevancia de referencia; especificar unidad documento/fragmento y casos sin respuesta |
| Reduce alucinaciones | Proporción de afirmaciones sustentadas, contradicciones y afirmaciones sin evidencia | Presencia de enlace no demuestra respaldo de cada afirmación |
| Clasifica intenciones | Macro-F1, precisión/recobrado por clase, matriz de confusión, cobertura/fallback | Separar ejemplos del catálogo y prueba; no tratar similitud como probabilidad calibrada |
| Es más rápido | Intervalos inicio-fin idénticos, mediana, dispersión, percentiles y fallos | Latencia interna y tiempo visible al usuario no son comparables |
| Mejora percepción | Ítems, anclajes, puntuación, distribución, efectos e intervalos | Alfa global no valida dimensiones; un ítem de seguridad mide percepción, no protección técnica |
| Un componente causa la mejora | Ablación controlada con corpus, consultas y condiciones constantes | Comparar servicios completos solo sustenta el efecto conjunto observado |
| Escala y es reproducible | Snapshot, versiones, prompts, corpus, fragmentación, parámetros, costes y carga | Un repositorio actual no certifica la versión usada en pruebas anteriores |

## Diseño y estadísticas

- La cantidad de participantes no equivale a diversidad de consultas: informar escenarios, preguntas únicas y programas.
- Revisar reclutamiento, orden de uso, familiaridad previa, sesiones, ayuda proporcionada y datos faltantes.
- Para Wilcoxon describir tratamiento de ceros/empates y método; valorar supuestos y sensibilidad con prueba de signos cuando proceda. No confundir significancia con relevancia práctica.
- Bootstrap al nivel de la unidad independiente, conservando pares y medidas repetidas; informar réplicas, semilla y tipo de intervalo.
- Para índices compuestos, explicitar componentes, pesos, rango, motivación y sensibilidad. No llamar accuracy a una suma ponderada de éxito, errores y presencia de fuentes.
- Si jueces puntuaron conjuntamente, no calcular kappa o acuerdo interevaluador a partir de la puntuación consensuada. Una nueva evaluación independiente debe declararse como posterior.
- Las matrices multicriterio de selección tecnológica no son benchmarks experimentales. No exigir cambiar de arquitectura para ajustarse a una moda; pedir evidencia proporcional al aporte reivindicado.
- Proponer métricas adicionales solo si responden una pregunta del artículo. No exigir RAGAS, BLEU o ROUGE por defecto ni fijar cortes arbitrarios de aceptación.

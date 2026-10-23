![](media/image1.jpg){width="4.342462817147856in" height="0.6in"}

ESCUELA DE POSGRADO

PROGRAMA ACADÉMICO DE MAESTRÍA EN INTELIGENCIA ARTIFICIAL

**Título del trabajo de investigación**

**Predicción del riesgo de bajo rendimiento académico mediante
algoritmos de Machine Learning en estudiantes de Ingeniería de Minas,
2026**

**Trabajo de investigación para obtener el grado de maestro(a) en
Inteligencia Artificial**

**Autor(es):**

QUINTANA QUISPE, José Orlando(orcid.org/0000-001-6487-1313)

**Asesor(a)(es):**

MSc. QUISPE LLACCTARIMAY, Rubén(orcid.org/0000-0003-2550-1840)

**Curso:** Trabajo de Investigación II -- Sesión

**Línea de investigación:**

Educación y Calidad Educativa

**Línea de responsabilidad social universitaria:**

Educación de Calidad

LIMA --- PERÚ

2026

##  

### Declaratoria de autenticidad del asesor

Yo, MSc. QUISPE LLACCTARIMAY, Rubén, en mi calidad de asesor del trabajo
de investigación titulado "Predicción del riesgo de bajo rendimiento
académico mediante algoritmos de Machine Learning en estudiantes de
Ingeniería de Minas, 2020-2025", presentado por el maestrante José
Orlando Quintana Quispe, declaro que he revisado el documento en todas
sus etapas y que el mismo cumple con los estándares académicos y éticos
establecidos por la Universidad César Vallejo. Doy fe de que el trabajo
ha sido desarrollado bajo mi acompañamiento y supervisión directa.

### Declaratoria de originalidad del/os autor/es

### 

Yo, José Orlando Quintana Quispe, autor del presente trabajo de
investigación, declaro bajo juramento que el documento es de mi entera
autoría, que no ha sido presentado previamente para obtener ningún grado
académico y que respeta íntegramente las normas de integridad científica
de la Universidad César Vallejo (RCU N°0157-2025).

Asimismo, autorizo que los resultados de la presente investigación se
publiquen manteniendo mi anonimato cuando corresponda, y que los datos
anonimizados sean depositados en repositorios públicos
FAIR(Zenodo/GitHub) una vez aceptado el manuscrito para revisión por
pares.

El uso de herramientas tecnológicas basadas en inteligencia artificial
se limitó al soporte de depuración de scripts de Python y a la
estructuración de ecuaciones de búsqueda bibliográfica, las cuales se
encuentran registradas de manera transparente en los anexos. No se ha
incorporado texto generado por IA en el cuerpo del informe.

### Dedicatoria

A la memoria de mi padre y a mi madre por haber inculcado que la
educación es el camino más firme hacia la dignidad. A los estudiantes de
Ingeniería de Minas, cuya trayectoria académica inspiró cada línea de
este trabajo.

### Agradecimiento

## Expreso mi reconocimiento y profundo agradecimiento a la Institución por facilitarme el acceso a los registros académicos y socioeconómicos para materializar este estudio. Agradezco también al asesor de tesis, MSc. QUISPE LLACCTARIMAY, Rubén . por su orientación rigurosa y observaciones precisas en cada etapa del proceso. Finalmente, extiendo mi gratitud a la Universidad César Vallejo y a su programa de Maestría en Inteligencia Artificial por brindar el espacio formativo que hizo posible esta investigación.

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## **Índice de contenidos**

[Carátula](#_heading=) i

[Declaratoria de autenticidad del asesor ii](#_heading=h.h7kibhk2zkkv)

[Declaratoria de originalidad del/os autor/es iii](#_heading=)

[Dedicatoria iv](#_heading=)

[Agradecimiento v](#_heading=)

[Índice de contenidos vi](#_heading=)

[Índice de tablas vii](#_heading=)

[Índice de figuras (de corresponder) viii](#_heading=)

[Resumen ix](#_heading=)

[Abstract x](#_heading=)

[Introducción [13](#introducción)](#introducción)

[Metodología [22](#metodología)](#metodología)

[Resultados [35](#resultados)](#resultados)

[Discusión (de ser pertinente)
[56](#discusión-de-ser-pertinente)](#discusión-de-ser-pertinente)

[Conclusiones [62](#conclusiones)](#conclusiones)

[Recomendaciones [68](#recomendaciones)](#recomendaciones)

[Referencias [71](#referencias)](#referencias)

**Anexos**

## 

## 

## 

## 

## 

## **Índice de tablas**

[Tabla 1. Composición de la muestra según estado académico
[27](#_Toc242806473)](#_Toc242806473)

[Tabla 2. Estructura de la base de datos - Variables académicas
principales [28](#_Toc242806474)](#_Toc242806474)

[Tabla 3. Estructura de la base de datos - Variables socioeconómicas
principales [29](#_Toc242806475)](#_Toc242806475)

[Tabla 4. Codificación de variables categóricas principales
[29](#_Toc242806476)](#_Toc242806476)

[Tabla 5. Variables derivadas mediante ingeniería de características
[30](#_Toc242806477)](#_Toc242806477)

[Tabla 6. Resumen del proceso de depuración
[31](#_Toc242806478)](#_Toc242806478)

[Tabla 7. Herramientas tecnológicas empleadas
[32](#_Toc242806479)](#_Toc242806479)

[Tabla 8. Correspondencia entre base de datos y diseño metodológico
[33](#_Toc242806480)](#_Toc242806480)

[Tabla 9. Distribución del rendimiento académico
[36](#_Toc242806481)](#_Toc242806481)

[Tabla 10. Estadística descriptiva de variables numéricas principales
[39](#_Toc242806482)](#_Toc242806482)

[Tabla 11. Resultados de la prueba Kruskal-Wallis
[42](#_Toc242806483)](#_Toc242806483)

[Tabla 12. Resultados de la prueba Chi-Cuadrado de independencia
[43](#_Toc242806484)](#_Toc242806484)

[Tabla 13. Tabla de contingencia- Estado civil de los padres vs.
Rendimiento(porcentajes por filas) [43](#_Toc242806485)](#_Toc242806485)

[Tabla 14. Resultados de validación cruzada (5-Folds, con SMOTE)
[45](#_Toc242806486)](#_Toc242806486)

[Tabla 15. Tabla de operacionalización de variables
[1](#_Toc242806487)](#_Toc242806487)

[Tabla 16. Matriz de Consistencia [3](#_Toc242806488)](#_Toc242806488)

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## **Índice de figuras (de corresponder)**

[Fig. 1. Flujo End-to-End [23](#_Toc242806072)](#_Toc242806072)

[Fig. 2. Distribución de frecuencias del promedio ponderado general
[37](#_Toc242806073)](#_Toc242806073)

[Fig. 3. Rendimiento académico según el nivel de ingreso familiar
[40](#_Toc242806074)](#_Toc242806074)

[Fig. 4. Distribución del rendimiento según tipo de colegio
[41](#_Toc242806075)](#_Toc242806075)

[Fig. 5. Matriz de correlación de Sperman entre variables numéricas
[44](#_Toc242806076)](#_Toc242806076)

[Fig. 6. Matriz de confusión del modelo XGBoost.(Conjunto de prueba)
[46](#_Toc242806077)](#_Toc242806077)

[Fig. 7. Curva ROC Multiclase del Modelo XGBoost optimizado
[47](#_Toc242806078)](#_Toc242806078)

[Fig. 8. SHAP Summary Plot: Importancia global de variables
[48](#_Toc242806079)](#_Toc242806079)

[Fig. 9. Gráfico de dependencia SHAP: Tasa de aprobación vs. Predicción
[50](#_Toc242806080)](#_Toc242806080)

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## 

## **Resumen**

## El bajo rendimiento y la deserción son problemas graves en la formación de ingenieros de minas en el Perú. Por ello, esta investigación buscó crear una herramienta predictiva para detectar tempranamente a los estudiantes en riesgo entre 2020 y 2025. Trabajamos con un enfoque cuantitativo, analizando 833 registros históricos reales. Para que el modelo fuera justo y preciso, aplicamos técnicas como la metodología CRISP-DM y la ingeniería de características ()creando variables como tasa de aprobación y ritmo de egreso), evitamos fuga de datos, balanceamos la información con SMOTE y usamos validación cruzada. Tras usar seis algoritmos, XGBoost fue el más efectivo, logrando una exactitud del 95.31% y un F1 -Macro de 0.9270, demostrando ser robusto incluso con datos desbalanceados. Además, gracias a la inteligencia artificial explicable (SHAP), descubrimos que el éxito o fracaso no es un misterio: la tasa de aprobación, el promedio más bajo y el ritmo de egreso son los factores que más pesan. En conclusión, este trabajo no es sólo números. Alineado con el Objetivo de Desarrollo Sostenible 4 (Educación de Calidad), busca dar a las universidades una brújula para intervenir a tiempo, brindando el apoyo necesario a quienes más lo necesitan antes que sea tarde.

> Palabras clave: Machine Learning, Minería de datos, Rendimiento
> académico, Inteligencia artificial explicable, Educación superior.

## **Abstract**

> Poor academic performance and dropout rates are serious problems in
> mining engineering education in Peru. Therefore, this research sought
> to create a predictive tool to identify at-risk students early on
> between 2020 and 2025. We employed a quantitative approach, analyzing
> 833 real historical records. To ensure the model was fair and
> accurate, we applied techniques such as the CRISP-DM methodology and
> feature engineering (creating variables such as pass rate and
> graduation rate), prevented data leakage, balanced the data using
> SMOTE, and performed cross-validation. After testing six algorithms,
> XGBoost proved to be the most effective, achieving an accuracy of
> 95.31% and an F1-Macro score of 0.9270, demonstrating robustness even
> with imbalanced data. Furthermore, thanks to explainable artificial
> intelligence (SHAP), we discovered that success or failure is no
> mystery: the approval rate, the lowest GPA, and the graduation rate
> are the most influential factors. In conclusion, this work is not just
> about numbers. Aligned with Sustainable Development Goal 4 (Quality
> Education), it seeks to provide universities with a roadmap for timely
> intervention, offering the necessary support to those who need it most
> before it is too late.
>
> Keyword: Machine Learning, Data Mining, Academic Performance,
> Explanainable Artificial Intelligence, Higher Education.

## **Introducción**

> La educación universitaria enfrenta una crisis silenciosa y a la vez
> preocupante: el bajo rendimiento académico. Globalmente, las tasas de
> deserción universitaria se encuentran en rangos de entre 30% a 50%
> siempre en los primeros años de estudio, lo que representa una pérdida
> de recursos institucionales sino que además la frustración de los
> planes de vida y consecuentemente, el desperdicio de capital humano y
> su potencial \[1\]. En América latina, esta problemática se agrava
> debido a las profundas brechas socioeconómicas y educativas
> preexistentes y que los estudiantes arrastran desde la educación
> básica \[2\].
>
> Perú no es ajeno a esta realidad. Las universidades públicas, que
> albergan a la población estudiantil más vulnerable del país, reportan
> índices alarmantes de estancamiento curricular y abandono. Las
> universidades del sur del Perú ubicadas en regiones mineras con altos
> índices de pobreza y limitaciones educativas históricas, hacen frente
> al desafío de formar ingenieros de Minas competentes mientras lidia
> con estudiantes que provienen de colegios estatales con deficiencias
> formativas severas, familias con ingresos precarios y contextos
> sociales que no favorecen el estudio \[3\]. La formación de los
> ingenieros de minas en Perú se enfrenta a una contradicción que es
> necesario abordar: las tasas de abandono y el rendimiento académico
> por debajo de la media en las universidades que imparten esta
> titulación siguen siendo motivo de preocupación, a pesar de que la
> demanda profesional en el sector extractivo sigue siendo elevada
> \[4\].
>
> Las escuelas de ingeniería de minas de las universidades del sur del
> Perú constituyen un caso paradigmático. Esta carrera caracterizada por
> su alta exigencia en ciencias (matemática, física y química) y su
> rigurosa malla curricular, presentan tasas de reprobación que superan
> el 40% en cursos críticos como cálculo, física y química general. Los
> métodos tradicionales de seguimiento académico, basados en la revisión
> reactiva de actas de notas al finalizar el semestre, resultan
> completamente insuficientes o no efectivos para reducir o prevenir el
> fracaso académico. Cuando un docente identifica que un estudiante esta
> reprobado, generalmente ya es demasiado tarde, el daño está hecho, el
> estudiante ha perdido el ciclo, se han desperdiciado recursos
> económicos y, aun algo más grave, se ha visto un daño a su autoestima
> académica \[5\].
>
> La literatura de investigación ha demostrado que el bajo rendimiento
> académico no es un evento repentino, sino que se produce como un
> proceso acumulativo de problemas que inician al comenzar el primer
> semestre. Estudiantes que desaprueban uno o dos cursos en su primer
> ciclo tienen una probabilidad superior al 70% de abandonar la carrera
> antes del quinto semestre. Sin embargo, las universidades peruanas
> carecen de sistemas predictivos que identifiquen estas trayectorias de
> riesgo en tiempo real \[6\], \[7\], \[8\].
>
> En este contexto, la Inteligencia Artificial (IA) y, más
> específicamente el Aprendizaje Automático, son herramientas
> transformadoras. La Minería de Datos Educativos (Educational Data
> Mining - EDM) y las Analíticas del Aprendizaje (Learning Analytics)
> han demostrado su capacidad para predecir el rendimiento estudiantil
> con precisiones superiores al 90% en contextos controlados \[9\]. No
> obstante, su implementación en universidades públicas peruanas es
> prácticamente inexistente, limitándose a experiencias piloto aisladas
> y sin escalabilidad\[10\], \[11\].
>
> Teniendo en cuenta que se trata del uso del aprendizaje automático, en
> particular, en el ámbito académico. Según investigaciones recientes,
> modelos como Random Forest, XGBoost y las redes neuronales han
> demostrado una eficacia notable a la hora de predecir el rendimiento
> de los estudiantes en diversos escenarios \[2\]. Sin embargo, la
> mayoría de estos estudios se han llevado a cabo bien en universidades
> de países ricos, bien en programas de grado cuyos requisitos de acceso
> difieren significativamente de los de los programas de ingeniería
> minera del sur de Perú.
>
> Este estudio se enmarcó en la línea de investigación institucional
> "Educación y calidad educativa/Aprendizaje automático para la toma de
> decisiones" y aborda directamente el Objetivo de Desarrollo Sostenible
> 4 (Educación de calidad), concretamente las metas 4.3 (acceso
> equitativo a la educación superior) y 4.4 (mejora de la
> empleabilidad). Su importancia radica en que, además de la precisión
> en la predicción, el modelo propuesto ofrece interpretabilidad a
> través de los valores SHAP, lo que permite a los responsables
> académicos comprender el razonamiento que subyace a cada predicción y
> diseñar intervenciones educativas específicas.
>
> La presente investigación inició con el problema general: ¿En qué
> medida un modelo de Machine Learning permitirá predecir el rendimiento
> académico de los estudiantes de Ingeniería de Minas durante el periodo
> 2020-2025? A partir de esta pregunta, se plantean problemas
> específicos con la finalidad de determinar la importancia relativa de
> las variables predictoras académicas, personales y socioeconómicas en
> la clasificación del rendimiento académico; comparar el desempeño de
> los algoritmos de Regresión Logística, Árboles de Decisión, Random
> Forest, Gradient Boosting, XGBoost y Redes Neuronales Artificiales;
> evaluar su capacidad discriminativa mediante métricas como Accuracy,
> Precisión, Recall, F1-score y Matriz de confusión; e identificar,
> mediante técnicas de Inteligencia Artificial Explicable (SHAP), las
> variables que presentan mayor influencia en las predicciones\[12\]. De
> esta manera, el estudio no sólo busca conocer qué tan precisos pueden
> ser los modelos de aprendizaje automático, sino también comprender qué
> factores intervienen en el rendimiento académico y cómo contribuyen a
> explicar las predicciones obtenidas. Esta perspectiva resulta
> importante a explicar las predicciones obtenidas. Esta perspectiva
> resulta de gran importancia porque, en el ámbito educativo, un modelo
> predictivo resulta útil, pero su esencia aparece cuando sus resultados
> pueden interpretarse y convertirse en información que apoye la toma de
> decisiones institucionales.
>
> En correspondencia con los problemas planteados, el objetivo general
> de la investigación fué determinar en qué medida un modelo de machine
> learning permitirá predecir el rendimiento académico de los
> estudiantes de Ingeniería de Minas durante el periodo 2020- 2025,
> mediante la implementación y evaluación de diferentes algoritmos de
> aprendizaje automático aplicados a datos educativos históricos. Para
> ello, se plantean como objetivos específicos determinar la importancia
> de las variables académicas, personales y socioeconómicas en la
> clasificación del rendimiento académico; comparar el desempeño de los
> algoritmos de Regresión Logística, Árboles de Decisión, Random Forest,
> XGBoost y Redes Neuronales Artificiales; comparar su capacidad
> discriminativa mediante las métricas de evaluación Accuracy,
> Precisión, Recall, F1 -score, ROC -AUC y Matriz de confusión; e
> identificar, mediante técnicas SHAP, las variables que ejercen mayor
> influencia en las predicciones. Con ello, determinar qué modelo
> presenta el mejor desempeño predictivo, sino a su vez comprender el
> comportamiento del mismo y presentar evidencia que haga factible su
> aplicación en problemas educativos vigentes.
>
> La investigación aporta al cuerpo de conocimiento de la Minería de
> Datos Educativos (EDM) y las Analíticas del Aprendizaje al
> proporcionar evidencia empírica sobre la aplicación de algoritmos de
> ensamblaje(ensemble methods) en el contexto específico de la educación
> superior pública peruana. Muy a pesar que existen variados estudios
> internacionales sobre la predicción del rendimiento académico\[13\],
> la literatura carece de investigaciones que aborden las
> particularidades del sistema universitario peruano: desbalance severo
> de clases, variables socioeconómicas críticas y contextos regionales
> con limitaciones estructurales.\[13\]
>
> El estudio valida la aplicabilidad de la Teoría del Compromiso
> Estudiantil de Tinto y la Teoría del Capital Humano de Becker en
> entornos digitales, demostrando que las variables de integración
> académica y social pueden ser operacionalizadas mediante técnicas de
> Machine Learning para predecir trayectorias estudiantiles con alta
> precisión.\[4\], \[13\] .
>
> Este trabajo establece un protocolo metodológico riguroso y replicable
> para el desarrollo de modelos predictivos en educación superior,
> abordando desafíos técnicos críticos como:
>
> El tratamiento del desbalance de clases mediante SMOTE (Synthetic
> Minority Over-sampling Technique) aplicando exclusivamente en
> conjuntos de entrenamiento para evitar fuga de datos (data
> leakage)\[16\].
>
> La validación cruzada estratificada en 5 grupos (CV estratificada en 5
> grupos) es una técnica robusta de validación del rendimiento que
> garantiza que los resultados de las métricas reflejen la capacidad de
> generalización y no un sobreajuste\[17\].
>
> Cuando una clase predomina en el conjunto de datos, puede resultar
> engañoso dar prioridad a métricas adecuadas para datos desequilibrados
> (puntuación F1 macro, recuperación) frente a la precisión simple.
>
> El uso de técnicas de Inteligencia Artificial Explicable (XAI) y LIME
> mediante SHAP (Shapley Additive exPlanations), superando la "caja
> negra" de los algoritmos complejos y proporcionando transparencia en
> las predicciones. Este proceso de implementación permitiría que otras
> escuelas profesionales y universidades públicas del país, adopten
> estas prácticas analíticas basadas en evidencia\[18\].
>
> La futura incorporación del modelo a la gestión universitaria debe
> considerar la preparación institucional para adoptar analítica del
> aprendizaje, además del desempeño técnico del algoritmo\[19\].
>
> Los resultados obtenidos en esta investigación impactan directa e
> inmediatamente en la gestión académica de las escuelas profesionales
> de Ingeniería de Minas, sistema de Alerta Temprana Operativo, el
> modelo XGBoost optimizado, con un Recall del 98.04% para la clase
> "Bajo", puede implementarse inmediatamente como herramienta de apoyo a
> la decisión para las tutorías y bienestar universitario. Al inicio de
> cada semestre, el sistema puede identificar proactivamente a los
> estudiantes en riesgo, permitiendo intervenciones preventivas antes
> que se materialice el fracaso académico.
>
> Optimización de Recursos Limitados: Las universidades públicas
> peruanas operan con presupuesto extremadamente restringidos. El SAT
> permite dirigir los escasos recursos de tutoría, nivelación académica
> y apoyo socioeconómico exclusivamente a los estudiantes que realmente
> lo necesitan, maximizando el impacto de cada sol invertido.
>
> Personalización de Intervenciones: Los gráficos SHAP revelan no sólo
> QUIENES están en riesgo, sino POR QUÉ lo están. Cuando el modelo
> detecta que el estudiante tiene alta probabilidad de bajo rendimiento
> por su ingreso familiar y gasto en transporte, la oficina de bienestar
> universitario puede apoyar con becas de movilidad. En el caso el
> problema sea la tasa de aprobación histórica, se deberían usar como
> apoyo tutorías académicas. Previniendo así intervenciones frustradas
> sin efectividad \[18\].
>
> Al prevenir el bajo rendimiento y consecuente deserción, la
> universidad mejora sus indicadores de eficiencia terminal, fortalece
> su acreditación institucional y, lo más importante, permite que
> estudiantes de contextos vulnerables culminen sus carreras y rompan el
> ciclo socioeconómico intergeneracional. El éxito en ingeniería de
> Minas puede replicarse en otras escuelas profesionales de las
> universidades nacionales peruanas y extenderse generando un impacto
> positivo en la calidad de la educación superior pública.\[20\],
> \[21\].
>
> En el ámbito social, la investigación fomenta la creación de un
> sistema de educación superior más inclusivo y equitativo, al
> garantizar que los estudiantes de diversos orígenes académicos reciban
> la ayuda que necesitan para completar con éxito su formación
> profesional.\[22\]
>
> La disminución de los índices de reprobación y rezago académico
> beneficiara a los estudiantes y sus familias, y promovería el
> desarrollo del capital humano especializado necesario para la
> expansión a largo plazo del sector minero peruano, lo cual está en
> concordancia con los objetivos de desarrollo regional y la
> responsabilidad social universitaria.\[23\]
>
> Las estadísticas a nivel mundial indican que, a lo largo de los
> últimos cinco años, se ha producido un aumento significativo del uso
> del aprendizaje automático en la educación superior. Según \[13\], con
> el objetivo de evaluar algoritmos de ensamblaje, utilizaron como
> método una revisión sistemática integrando variables académicas
> históricas, de interacción en plataformas virtuales y socioeconómicas.
> Como resultados obtuvieron que Random Forest y Gradiente Boosting
> alcanzan altos niveles de precisión, concluyendo que superan
> frecuentemente a los métodos tradicionales de predicción del
> rendimiento académico. Por su parte \[24\], con el objetivo de
> identificar patrones de riesgo en instituciones latinoamericanas,
> aplicaron como método la integración de analítica del aprendizaje como
> minería de datos educativos (EDM). Sus resultados demostraron la
> capacidad para identificar patrones de bajo rendimiento con hasta tres
> meses de anticipación concluyendo que esto resulta conveniente para
> intervenciones que prevengan resultados adversos.
>
> En el contexto peruano, estudios recientes en universidades públicas
> peruanas mostraron resultados prometedores. \[20\], con el objetivo de
> identificar riesgos académicos, emplearon como método modelos de
> regresión logística y árboles de decisión. Obtuvieron como resultados
> elevados niveles de precisión predictiva. Concluyendo la importancia
> de los factores académicos y contextuales en los procesos de
> aprobación de cursos.\[25\]
>
> En el contexto internacional, Machine Learning aplicado en la
> educación ha experimentado un crecimiento vertiginoso en la última
> década. En la investigación \[26\] realizaron un estudio sobre la
> aplicación de modelos de aprendizaje automático en la predicción del
> rendimiento académico estudiantil, utilizando variables académicas,
> conductuales y demográficas. Se hicieron aplicaciones técnicas de
> preprocesamiento, seleccionaron características mediante Chi-cuadrado
> y variados algoritmos de clasificación incluyendo KNN, SVM, Regresión
> Logística, Árboles de Decisión y MLPC, además de modelos de ensamble,
> Mediante validación cruzada de 10 folds, la métrica de clasificación
> alcanzó una precisión máxima de 79.1%. Asimismo, el uso de SHAP
> permitió analizar e identificar la asistencia a clases y el uso de
> recursos en línea como factores que determinan el rendimiento
> académico. Se concluyó que el aprendizaje automático contribuye a
> identificar estudiantes en riesgo académico y la consecuente
> intervención en apoyo de manera oportuna \[22\].
>
> En universidades asiáticas, \[27\], con el objetivo de detectar
> patrones de riesgo académico de manera anticipada en Asia, aplicaron
> como método la integración del procesamiento de lenguaje natural y
> algoritmos de clasificación. Sus resultados permitieron intervenciones
> oportunas, concluyendo que esta integración facilita la
> personalización de alertas.
>
> A nivel global, \[28\] realizaron una revisión sistemática y evaluaron
> algoritmos de ensamblaje, usando variables académicas históricas, de
> interacción en plataformas virtuales y socioeconómicas. Su hallazgo
> concluye en que Random Forest y Gradiente Boosting logran elevados
> niveles de precisión, los que superan frecuentemente a los métodos
> estadísticos tradicionales para la predicción del rendimiento
> académico.
>
> En Latinoamérica, \[2\], \[29\] usaron analítica del aprendizaje
> integrada con minería de datos educativos (EDM) en la identificación
> de patrones de riesgo. Encontraron resultados que demuestran la
> capacidad de identificar patrones de bajo rendimiento anticipándose
> hasta con tres meses, concluyeron que esto resultaba muy conveniente
> para intervenciones preventivas\[30\].
>
> En contextos específicos de la región,\[31\], con el objetivo de
> evaluar los predictores del rendimiento , aplicaron como método el
> análisis de variables socioeconómicas e históricas. Sus resultados
> mostraron que, aunque las variables socioeconómicas influyen
> significativamente, los factores académicos históricos(desempeño y
> calificaciones previas) son los más influyentes con una importancia
> relativa del 65%, concluyendo que el historial académico es el
> predictor más robusto.
>
> En el ámbito nacional, \[20\] desarrollaron modelos de regresión
> logística y árboles de decisión en la identificación del riesgo
> académico en universidades públicas. Lograron una precisión predictiva
> del 78%, concluyeron en la importancia de los factores académicos y
> contextuales en los procesos de aprobación de cursos, también
> señalaron que había limitaciones en la calidad y estandarización de
> los datos.
>
> Recientemente, \[32\] compararon varios algoritmos de clasificación
> para predecir el rendimiento académico en estudiantes de primer año.
> Sus resultados determinaron que Random Forest y XGBoost presentaron el
> mejor desempeño predictivo (F1 -- score de 0.82), además concluyeron
> que existen limitaciones relacionadas con la incorporación de
> variables socioeconómicas y la interpretabilidad de los modelos
> complejos.
>
> Existe una brecha de conocimiento y a pesar de los avances en Learning
> Analytics y Machine Learning a nivel internacional existe escasa
> evidencia sobre modelos predictivos explicables aplicados
> específicamente a estudiantes de Ingeniería de Minas en universidades
> públicas peruanas \[32\], \[33\]. La literatura actual presenta
> limitaciones en la incorporación integral de variables socioeconómicas
> verificables, en la interpretabilidad de los modelos usando técnicas
> XAI y la validación en contextos específicos de ingeniería con altas
> tasas de deserción. Este vacío justifica la pertinencia de este
> estudio.
>
> Aunque la cantidad de datos educativos en el Perú ha aumentado durante
> los últimos años, todavía existen limitaciones relacionadas con la
> calidad, organización e integración de la información académica
> histórica. En el ámbito nacional indican que modelos basados en
> Árboles de Decisión, Regresión Logística y Random Forest presentan
> buenos niveles de precisión en la predicción del rendimiento académico
> y riesgo de reprobación, aunque inferiores a los reportados en
> contextos internacionales debido a restricciones a la disponibilidad y
> estandarización de datos \[20\], \[34\]
>
> En el artículo \[26\] usaron el aprendizaje automático en la
> predicción de finalización de programas de capacitación para el
> trabajo, donde surgió un desequilibrio entre las clases participantes
> que terminan y abandonan. Tenían 6548 registros, y usaron SMOTE para
> solucionar el desequilibro de las clases y luego se compararon las
> métricas de seis modelos predictivos. Según las métricas de evaluación
> XGBoost fue quien tuvo mejor desempeño, con un F1 de 0.920 y ROC-AUC
> de 0.9684. Estos resultados indican que el aprendizaje automático
> puede predecir a tiempo los individuos en riesgo de abandono y
> facilitar que se implementen programas que prevengan el bajo
> rendimiento.
>
> A nivel latinoamericano, \[35\] publican una revisión sistemática
> enfocada en Learning Analytics en educación superior latinoamericana,
> analizaron 83 investigaciones provenientes de 12 países. Determinaron
> que, si bien Brasil, Chile y Colombia encabezan la producción
> científica en el área, Perú aparece con apenas 3 estudios publicados,
> evidenciando una brecha amplia. Los investigadores determinaron que
> modelos entrenados en Europa o Estados Unidos no se pueden utilizar en
> Latinoamérica debido a que los sistemas educativos son diferentes, la
> cultura y la parte socioeconómica de los estudiantes, lo que indica
> que es en el entorno donde se deben desarrollar los modelos locales.
>
> Diversos estudios indican que el poder de los modelos mejora bastante
> cuando se agregan variables académicas, socioeconómicas y factores
> spicosociales. Haciendo ver la necesidad de fortalecer los procesos
> institucionales de recopilación y gestión de datos educativos \[24\].
>
> En teoría, la analítica del aprendizaje, definida como la medición, el
> análisis y la presentación de informes sobre datos relativos a la
> presentación de informes sobre datos relativos a los estudiantes y sus
> contextos, con el objetivo de comprender y optimizar el aprendizaje y
> los entornos en los que ocurre, servirá de base para este estudio
> \[36\].
>
> Además el aprendizaje automático supervisado según la cual los
> algoritmos pueden anticipar con precisión casos nunca vistos antes
> mediante el aprendizaje de funciones de mapeo a partir de datos de
> entrada y salida etiquetados\[37\], \[38\],\[39\].
>
> Por último, el estudio pondrá a prueba la hipótesis general de que el
> uso de modelos de aprendizaje automático permitirá predecir con
> precisión el rendimiento académico de los estudiantes de ingeniería
> minera durante el periodo 2020-2025, con niveles de precisión
> superiores al 80%, mediante la combinación de variables académicas y
> socioeconómicas \[13\].

## **Metodología**

El estudio tuvo un enfoque cuantitativo, de tipo aplicado y con diseño
no experimental longitudinal. Esta elección respondió a la necesidad de
analizar datos históricos sin manipular las variables, pero si
identificando patrones predictivos a lo largo del tiempo.

La unidad de análisis correspondió al registro histórico individual de
cada estudiante matriculado en la escuela profesional de ingeniería de
minas, entre los periodos académicos 2020-1 y 2025-2. La muestra estuvo
conformada por la totalidad de registros disponibles, luego del proceso
de depuración y control de calidad descrito más adelante.

La fuente de información fue la base de datos académica institucional,
anonimizada previamente para garantizar la Confidenciabliidad de los
estudiantes. Los campos considerados incluyeron variables académicas
(promedios semestrales, tasa de aprobación, número de cursos aprobados y
desaprobados), variables socioeconómicas (nivel de ingreso familiar
mensual, tipo de colegio de procedencia) y variables de contexto
familiar (estado civil de los padres, tenencia de refrigerador como
proxy de nivel socioeconómico).

El proceso de tratamiento de datos se organizó en cuatro fases
secuenciales y 16 pasos secuenciales, como se observa en la Figura 1,
para la predicción del rendimiento académico de estudiantes de
ingeniería de Minas (2020-2025), iniciando con la obtención y fusión de
datos académico -- socioeconómicos (reduciendo de 840 a 833 registros
mediante INNER JOIN), prosigue con ingeniería de características y
análisis estadístico inferencial, pasando por el modelado con 6
algoritmos evaluados mediante validación cruzada estratificada con SMOTE
(seleccionando XGBoost como óptimo con F1 -Macro: 0.9270), y finalizando
con evaluación en test set reservado (20%) que reporta 96.41% de
accuracy, complementando con análisis de Explicabilidad global (SHAP) y
local (LIME + curva ROC), todo con un mecanismo de retroalimentación que
permita ajustar variables y features según el desempeño del modelo. tal
como se ilustra en la Figura1

![[]{#_Toc242806072 .anchor}Fig. 1. Flujo
End-to-End](media/image2.png){width="6.604166666666667in"
height="4.330555555555556in"}

Fuente: Elaboración propia

Se creó una única matriz denominada "MINAS_LIMPIO_IMPUTADO_RIGUROSO.csv"
(versión 2.0) a partir de la combinación de los registros dispersos. Se
detectaron duplicados, valores atípicos incoherentes y entradas
incompletas aplicando criterios de coherencia.

En función del tipo de datos, los valores que faltaban se imputaron
utilizando los métodos estadísticos adecuados (moda para las variables
categóricas y mediana para las variables numéricas). Los métodos
requieren que las variables categóricas sean numéricas por ello, se
utilizó la codificación one-hot. En rendimiento académico las clases
involucradas son desequilibradas, por ello, se utilizó la técnica SMOTE
(Synthetic Minority Oversampling Technique) sólo para el conjunto de
entrenamiento, y en la validación cruzada de 5 folds, para reducir la
fuga de datos.

El análisis del rendimiento académico por medio técnicas de aprendizaje
automático no es simplemente colocar los datos en un algoritmo esperando
una respuesta. En el proceso de desarrollo del modelado el proceso no
siempre se documenta de manera adecuada en otras palabras el modelo
puede calcular perfectamente y quizás responder de manera equivocada.

CRISP-DM fue desarrollado como un proceso estructurado en proyectos de
minería de datos, proponiendo una secuencia de etapas que se relacionan
entre sí y que organiza el análisis desde la comprensión del problema
hasta la evaluación y uso de los resultados.\[40\] Es de carácter
iterativo y que resulta apropiado aplicarlo en el ámbito educativo,
porque los datos vienen de contextos heterogéneos y las variables
académicas, sociodemográficas y de comportamiento generalmente están muy
relacionadas.\[41\], \[41\], \[42\].

CRISP-DM tiene en su estructura seis etapas: comprensión del negocio,
comprensión de los datos, preparación de los datos, modelado, evaluación
y despliegue. A pesar de que se presentan de manera secuencial, en la
práctica no son datos que se revisan una sola vez. Sino que deben
revisarse nuevamente cuando alguna decisión debe reconsiderarse.

En la primera etapa sobre la comprensión del problema esta consisten en
definir con mucha claridad el problema y llevarlo a objetivos que puedan
ser resueltos mediante técnicas de análisis de datos. Para nuestro caso
sobre el rendimiento académico se debe establecer qué fenómeno se
pretende explicar, predecir o clasificar y cuáles son las variables que
determinan o responden a las preguntas de investigación. En esta parte
del proceso es necesario establecer los criterios que permitirán lograr
con éxito el proyecto. Es necesario determinar si el modelo que presenta
la mayor exactitud resulta adecuado para el problema planteado y si
estos resultados son útiles en esa perspectiva educativa. El aprendizaje
automático encuentra patrones de manera eficaz pero no deciden si esos
patrones tienen sentido pedagógico. Debemos decidir su significado
\[43\].

Como segunda etapa al haberse definido el problema, procedemos a
explorar las características de los datos existentes. Lo que comprenden
la identificación de las fuentes de información, el análisis de las
variables, la revisión de su distribución y detección de valores,
ausentes, inconsistentes, duplicados y aparentes valores atípicos. Aquí
esta exploración permite encontrar aspectos que generalmente pasan
inadvertidos. Una variable de apariencia sencilla, como el promedio de
calificaciones puede depender de la diferencia entre asignaturas,
semestres académicos o criterios de evaluación. También, la ausencia de
algunos registros no es un fenómeno aleatorio debido a que puede estar
relacionado con estudiantes que abandonaron sus estudios o no
participaron en algunas actividades. Una comprensión de los datos
implica también conocer su historia. Un conjunto de datos no refleja
necesariamente la realidad; comparándola con una foto muestra algo pero
también oculta lo que quedo fuera del foco de la foto \[44\].

En una tercera etapa la preparación de los datos representa un proceso
importante debido a que los datos deben sufrir una transformación para
que se utilicen en los algoritmos seleccionados. Incluye la limpieza de
registros, tratamiento de valores faltantes, eliminación de duplicados,
codificación de variables categóricas, normalización o estandarización
de variables numéricas y selección o construcción de nuevas
características. Aquí deben documentarse las transformaciones aplicadas
procurando no introducir procedimientos que produzca fuga de información
(data leakage), fenómeno que ocurre cuando la información que debería
estar disponible únicamente después del momento de predicción termina
influyendo en el entrenamiento del modelo. Cada modificación sobre los
datos debe poder reconstruirse y justificarse, de modo que otro
investigador puede comprender cómo se pasó de los registros originales
al conjunto finalmente utilizado para el modelo, adquiriendo esta etapa
un papel importante \[44\], \[45\].

En la etapa de modelado la cuarta fase o etapa es donde se seleccionan y
se usan los algoritmos de aprendizaje automático apropiados que
respondan a los objetivos definidos previamente. Para nuestro caso
utilizaremos técnicas de clasificación múltiple que es un método
supervisado \[46\]. La elección del algoritmo no se basa únicamente en
su capacidad predictiva. Sino también considerar su capacidad
interpretativa. Un modelo menos preciso, pero con capacidad
interpretativa ofrece explicaciones comprensibles en los factores
asociados al rendimiento académico y resulta más conveniente que una
solución muy compleja y cuyo funcionamiento sea difícil de interpretar.
El entrenamiento debe aplicarse a los datos no observados de manera que
genere una estimación confiable. Por ejemplo, dataset divididos en 80%
entrenamiento y 20% prueba, validación cruzada y técnicas de ajuste de
hiperparámetros manteniendo separado al conjunto de prueba durante el
proceso de optimización \[44\], \[47\].

La evaluación en el quinto paso es un punto de control en el desempeño
técnico del modelo y los objetivos del trabajo de investigación. Se
analiza si el modelo alcanza los criterios o requerimientos establecidos
y esencialmente que los resultados respondan de manera correcta a las
preguntas planteadas. En problemas de clasificación múltiple se deben
considerar la exactitud, precisión, sensibilidad, especificidad,
puntuación F1 o el área bajo la curva ROC. Ninguna métrica debería ser
objeto de interpretación de manera aislada. Es necesario examinar
ocurrencia de sesgos, errores sistemáticos y diferencias en el desempeño
entre grupos de estudiantes. Cuando hay una gran capacidad predictiva
global puede esconder resultados deficientes en determinados subgrupos.
Lo que puede generar una paradoja importante: Un modelo no puede ser
estadísticamente bueno y socialmente problemático al mismo tiempo. Se
debe comprobar que existe coherencia entre le objetivos de la
investigación los datos utilizados junto con el modelo obtenido y las
conclusiones generadas o producto del desarrollo del trabajo de
investigación.

Finalmente, en la última fase o etapa respecto al despliegue e
interpretación de resultados CRISP-DM que es no necesariamente la
implementación inmediata del sistema automatizado sino a cómo serán
presentados y usados los conocimientos obtenidos. En la investigación
académica la presentación, visualización, análisis de variables
importantes y las conclusiones que se orientan a tomar decisiones se
materializan. Por ello CRISP-DM establece una conexión entre la
dimensión técnica y la dimensión investigativa del estudio. EL
aprendizaje automático deja de ser una colección de algoritmos aislados
y se integra en procesos sistemático en donde cada decisión puede
examinarse, documentarse y si es necesario revisarse.

CRISP-DM usado en el rendimiento académico permite el seguimiento,
reproductibilidad y coherencia metodológica del estudio. Su principal
fortaleza no es solamente ordenar en etapas el análisis, sino producir
conocimiento válido para comprender un problema educativo concreto. El
algoritmo puede ser el mejor y más rápido; la responsabilidad de hacer
las preguntas correctas sigue siendo responsabilidad del humano.

En el análisis y comparación usamos seis algoritmos: regresión
logística, árbol de decisión, bosque aleatorio, Gradient Boosting,
XGBoost y red neuronal multicapa. También, se utilizaron los valores
SHAP (Shapley Additive Explanations) para interpretar el modelo de mejor
desempeño; en modelos basados en árboles usamos TreeExplainer.

La investigación estuvo según el Código de Ética en Investigación de la
Universidad César Vallejo (RCU N.º 0157-2025). Posterior al análisis,
los datos se anonimizaron y se obtuvo la autorización institucional
requerida. Eliminando toda información de identificación directa de los
estudiantes.

De manera central este avance no se limita a demostrar que se dispone de
datos, sino garantizar que dicha información ha sido correctamente
organizada, validad y convertida en un insumo confiable para el análisis
estadístico posterior. Como señala \[48\], la sistematización de los
datos representa una fase crítica en toda investigación cuantitativa,
pues de ella depende directamente la validez y confiabilidad de los
resultados que se obtengan.

Este representa evidencias del proceso de codificación, organización en
base de datos, depuración y control de calidad aplicado a la información
recolectada sobre el rendimiento académico de los estudiantes de
Ingeniería de Minas, considerando tanto variables académicas como
socioeconómicas.

Datos académicos institucionales: Registro oficial de la escuela
profesional de Ingeniería de Minas, correspondiente al periodo 2020-1 a
2025-2. Contiene información de 840 estudiantes con 18 variables
académicas(código de estudiante, estado académico, tipo de ingreso,
semestre de ingreso, año de ingreso, semestres cursados, cursos
aprobados, cursos desaprobados, cursos matriculados, promedio ponderado
general, entre otros).

Fichas socioeconómicas: Reporte de fichas socioeconómicas aplicadas a
los estudiantes de Ingeniería de Minas en el Mismo periodo. Contiene
3,902 registros con 106 variables que comprenden datos demográficos,
familiares, económicos, de vivienda, hábitos de estudio, salud, entre
otros.

Luego de fusionar los datos mediante inner join por el campo
CODESTUDIANTE, se obtuvo un dataset consolidado de 833 registros válidos
con 125 columnas que constituye la muestra efectiva para el análisis.

  ------------------------------------------
  Estado académico Frecuencia   Porcentaje
  ---------------- ------------ ------------
  Estudiante       310          37.21%
  activo                        

  Egresado         318          38.18%

  Retiro           47           5.64%

  Abandono         37           4.44%

  Renuncia         28           3.36%

  Sin matrícula    26           3.12%

  Sancionado       54           6.48%

  Reserva          7            0.84%

  Retiroreserva    6            0.72%

  Total            833          100.00%
  ------------------------------------------

  : []{#_Toc242806473 .anchor}Tabla 1. Composición de la muestra según
  estado académico

Nota: Datos obtenidos del archivo MINAS_FUSIONADO_COMPLETO.csv

Siguiendo las indicaciones de la Guía de elaboración de trabajos de
investigación de la UCV(2026) ,se organizó la base de datos considerando
que cada fila representa un participante (n = 3,784) y cada columna
corresponde a una variable definida en la operacionalización. Los
nombres de las variables fueron codificados de manera clara y
consistente con los instrumentos aplicados

+----+----------------------------+------------+--------------------------+----------+
| N° | Nombre de variable         | Tipo       | Etiqueta / Descripción   | Origen   |
+:==:+============================+============+==========================+==========+
| 1  | CODESTUDIANTE              | Numérica   | Código único del         | Original |
|    |                            |            | estudiante               |          |
+----+----------------------------+------------+--------------------------+----------+
| 2  | ESCUELA                    | Categórica | Escuela profesional      | Original |
|    |                            |            |                          |          |
|    |                            |            | (Ingeniería de Minas)    |          |
+----+----------------------------+------------+--------------------------+----------+
| 3  | CLASIFICACION_ACTUAL       | Categórica | Estado académico actual  | Original |
|    |                            |            |                          | ️         |
+----+----------------------------+------------+--------------------------+----------+
| 4  | MODALIDAD_INGRESO          | Categórica | Modalidad de ingreso     | Original |
|    |                            |            |                          |          |
|    |                            |            | (CEPRE, Ordinario, COAR, |          |
|    |                            |            | etc.)                    |          |
+----+----------------------------+------------+--------------------------+----------+
| 5  | SEMESTRE_INGRESO           | Categórica | Semestre de ingreso (ej. | Original |
|    |                            |            | 20201)                   |          |
+----+----------------------------+------------+--------------------------+----------+
| 6  | ANIO_INGRESO               | Numérica   | Año de ingreso           | Original |
|    |                            |            | (2008-2024)              |          |
+----+----------------------------+------------+--------------------------+----------+
| 7  | SEMESTRES_CURSADOS         | Numérica   | Total, de semestres      | Original |
|    |                            |            | cursados                 |          |
+----+----------------------------+------------+--------------------------+----------+
| 8  | CURSOS_APROBADOS           | Numérica   | Total, de cursos         | Original |
|    |                            |            | aprobados                |          |
+----+----------------------------+------------+--------------------------+----------+
| 9  | CURSOS_DESAPROBADOS        | Numérica   | Total, de cursos         | Original |
|    |                            |            | desaprobados             |          |
+----+----------------------------+------------+--------------------------+----------+
| 10 | CURSOS_MATRICULADOS        | Numérica   | Total, de cursos         | Original |
|    |                            |            | matriculados             |          |
+----+----------------------------+------------+--------------------------+----------+
| 11 | PROMEDIO_PONDERADO_GENERAL | Numérica   | Promedio ponderado       | Original |
|    |                            |            | acumulado                |          |
+----+----------------------------+------------+--------------------------+----------+
| 12 | PROMEDIO_SEMESTRE_MAX      | Numérica   | Mejor promedio semestral | Original |
+----+----------------------------+------------+--------------------------+----------+
| 13 | PROMEDIO_SEMESTRE_MIN      | Numérica   | Menor promedio semestral | Original |
+----+----------------------------+------------+--------------------------+----------+
| 14 | TASA_APROBACION            | Numérica   | CURSOS_APROBADOS /       | Derivada |
|    |                            |            |                          |          |
|    |                            |            | (CURSOS_APROBADOS        |          |
|    |                            |            |                          |          |
|    |                            |            | \+ CURSOS_DESAPROBADOS)  |          |
+----+----------------------------+------------+--------------------------+----------+
| 15 | ESTABILIDAD_ACADEMICA      | Numérica   | PROMEDIO_SEMESTRE_MAX    | Derivada |
|    |                            |            |                          |          |
|    |                            |            | \- PROMEDIO_SEMESTRE_MIN |          |
+----+----------------------------+------------+--------------------------+----------+
| 16 | RITMO_EGRESO               | Numérica   | CURSOS_APROBADOS /       | Derivada |
|    |                            |            | SEMESTRES_CURSADOS       |          |
+----+----------------------------+------------+--------------------------+----------+
| 17 | EFICIENCIA_ACADEMICA       | Numérica   | CURSOS_UNICOS /          | Derivada |
|    |                            |            | CURSOS_MATRICULADOS      |          |
+----+----------------------------+------------+--------------------------+----------+
| 18 | INDICE_REPETICION          | Numérica   | CURSOS_REPETIDOS_COUNT / | Derivada |
|    |                            |            | CURSOS_APROBADOS         |          |
+----+----------------------------+------------+--------------------------+----------+

  --------------------------------------------------------------------------
   N°  Nombre de variable              Tipo         Etiqueta / Descripción
  ---- ------------------------------- ------------ ------------------------
   1   CODESTUDIANTE                   Numérica     Código único del
                                                    estudiante

   2   ESCUELA                         Categórica   Escuela profesional
                                                    (Ingeniería de Minas)

   3   ESTADO                          Categórica   Estado académico actual

   4   TIPO_INGRESO                    Categórica   Modalidad de ingreso
                                                    (CEPRE, Ordinario, COAR,
                                                    etc.)

   5   SEMESTRE_INGRESO                Categórica   Semestre de ingreso (ej.
                                                    20201)

   6   ANIO_INGRESO                    Numérica     Año de ingreso
                                                    (2008--2024)

   7   SEMESTRES_CURSADOS              Numérica     Total, de semestres
                                                    cursados

   8   CURSOS_APROBADOS                Numérica     Total, de cursos
                                                    aprobados

   9   CURSOS_DESAPROBADOS             Numérica     Total, de cursos
                                                    desaprobados

   10  CURSOS_MATRICULADOS             Numérica     Total, de cursos
                                                    matriculados

   11  PROMEDIO_PONDERADO_GENERAL      Numérica     Promedio ponderado
                                                    acumulado

   12  PROMEDIO_SEMESTRE_MAX           Numérica     Mejor promedio semestral

   13  PROMEDIO_SEMESTRE_MIN           Numérica     Menor promedio semestral
  --------------------------------------------------------------------------

  : []{#_Toc242806474 .anchor}Tabla 2. Estructura de la base de datos -
  Variables académicas principales

  ---------------------------------------------------------------------
   N°   Nombre de variable     Tipo         Etiqueta / Descripción
  ----- ---------------------- ------------ ---------------------------
    1   SEXO                   Categórica   Género del estudiante

    2   ESTADO_CIVIL           Categórica   Estado civil

    3   DEPARTAMENTO           Categórica   Departamento de origen

    4   TIPO_COLEGIO           Categórica   Tipo de colegio de
                                            procedencia

    5   ESTADO_CIVIL_PADRES    Categórica   Estado civil de los padres

    6   INGRESO_FAMILIAR       Categórica   Rango de ingreso familiar
                                            mensual

    7   FUENTE_INGRESO         Categórica   Fuente principal de
                                            ingresos

    8   TIPO_VIVIENDA          Categórica   Tenencia de la vivienda

    9   MATERIAL_PAREDES       Categórica   Material predominante en
                                            paredes

   10   SERVICIOS_BASICOS      Categórica   Acceso a servicios básicos
  ---------------------------------------------------------------------

  : []{#_Toc242806475 .anchor}Tabla 3. Estructura de la base de datos -
  Variables socioeconómicas principales

Se asignaron valores numéricos a todas las variables categóricas,
manteniendo una lógica consistente en toda base de datos:

  -----------------------------------------------------------
  Variable               Valor        Etiqueta
                         codificado   
  ---------------------- ------------ -----------------------
  SEXO                   0            Masculino

  SEXO                   1            Femenino

  TIPO_COLEGIO           0            Estatal

  TIPO_COLEGIO           1            Particular

  ESTADO_CIVIL_PADRES    0            Casados

  ESTADO_CIVIL_PADRES    1            Convivientes

  ESTADO_CIVIL_PADRES    2            Separados

  ESTADO_CIVIL_PADRES    3            Divorciados

  INGRESO_FAMILIAR       0            Menos de S/. 950.00

  INGRESO_FAMILIAR       1            De S/. 951.00 a S/.
                                      1500.00

  INGRESO_FAMILIAR       2            De S/. 1501.00 a S/.
                                      2500.00

  INGRESO_FAMILIAR       3            Más de S/. 2500.00

  RENDIMIENTO            0            Bajo (\< 11)

  RENDIMIENTO            1            Regular (11--13.99)

  RENDIMIENTO            2            Alto (≥ 14)
  -----------------------------------------------------------

  : []{#_Toc242806476 .anchor}Tabla 4. Codificación de variables
  categóricas principales

A partir de las variables originales se construyeron tres variables
derivadas que enriquecen el análisis:

  -------------------------------------------------------------------------
     Variable derivada    Fórmula                  Interpretación
  ----------------------- ------------------------ ------------------------
      TASA_APROBACION     CURSOS_APROBADOS /       Proporción de cursos
                          (CURSOS_APROBADOS +      aprobados sobre el total
                          CURSOS_DESAPROBADOS)     

   ESTABILIDAD_ACADEMICA  PROMEDIO_SEMESTRE_MAX −  Variabilidad del
                          PROMEDIO_SEMESTRE_MIN    rendimiento a lo largo
                                                   de la carrera

       RITMO_EGRESO       CURSOS_APROBADOS /       Velocidad promedio de
                          SEMESTRES_CURSADOS       aprobación por semestre
  -------------------------------------------------------------------------

  : []{#_Toc242806477 .anchor}Tabla 5. Variables derivadas mediante
  ingeniería de características

Tal y como recomiendan \[49\] y \[50\], se llevó a cabo un proceso
riguroso de depuración de la base de datos, el cual comprendió las
siguientes acciones:

Eliminación de identificadores personales: se removieron las columnas
CODESTUDIANTE, CODIGO, DNI, NOMBRES, APE_PAT, APE_MAT,
PROMEDIOS_POR_SEMESTRE_JSON e HISTORIAL_JSON para garantizar el
anonimato de cada individuo y evitar la fuga de datos (data leakage).

Respecto al tratamiento de datos faltantes, se aplicó imputación por
mediana para variables numéricas y por la moda para variables
categóricas, siguiendo las recomendaciones de \[51\].

El proceso de depuración, como se observa en la Tabla 6, permitió
comprobar que el dataset académico presentaba una alta calidad, ya que
no se identificaron valores nulos, registros duplicados ni datos fuera
de los rangos establecidos (0% en los tres casos). En cambio, el dataset
socioeconómico contenía 3,040 registros duplicados, originados por la
existencia de múltiples fichas semestrales correspondientes a un mismo
estudiante. Para resolver esta situación, se aplicó la técnica
drop_duplicates, con la finalidad de eliminar los registros repetidos y
evitar inconsistencias en el análisis. Posteriormente, la integración de
ambos conjuntos de datos mediante un INNER JOIN permitió conservar 833
de los 840 registros académicos originales, lo que representa una
retención del 99.17%. Los siete registros restantes no pudieron
incorporarse debido a que los estudiantes correspondientes no contaban
con una ficha socioeconómica registrada. Finalmente, los 671 valores
nulos que persistieron en el dataset fusionado fueron tratados durante
la fase de preprocesamiento mediante técnicas de imputación por mediana
y moda, según la naturaleza de las variables, tal y como se detalla en
el pipeline del trabajo.

  ---------------------------------------------------------------------
  Tipo de revisión           Registros    Errores      Errores
                             revisados    detectados   corregidos
  -------------------------- ------------ ------------ ----------------
  Datos faltantes (dataset   840          0            0
  académico)                                           

  Datos faltantes (dataset   3,902        4,499 celdas Imputados en
  socioeconómico)                         (1.09%)      fusión

  Duplicados (dataset        840          0            0
  académico)                                           

  Duplicados (dataset        3,902        3,040        3,040
  socioeconómico)                         (77.91%)     

  Valores fuera de rango     840          0            0
  (0-20)                                               

  Inconsistencias lógicas    840          0            0
  (valores negativos)                                  

  Registros sin emparejar    7            7            Excluidos (INNER
  (solo académico)                                     JOIN)

  Registros sin emparejar    29           29           Excluidos (INNER
  (solo socioeconómico)                                JOIN)

  Dataset final fusionado    833          671 celdas   Imputados en
                                          nulas        Script 1
                                          residuales   
  ---------------------------------------------------------------------

  : []{#_Toc242806478 .anchor}Tabla 6. Resumen del proceso de depuración

Luego del proceso de depuración, la base de datos final termino con 833
casos válidos para el análisis estadístico, representando el 96.93% de
los registros originales fusionados.

Para el proceso se sistematización se utilizaron las siguientes
herramientas tecnológicas, conforme a las exigencias del enfoque
cuantitativo:

  ------------------------------------------------------------
     Herramienta     Versión       Uso específico
  ------------------ ------------- ---------------------------
        Python       3.11          Procesamiento, fusión y
                                   análisis de datos

        pandas       2.1.4         Manipulación de DataFrames
                                   y limpieza

        NumPy        1.26.2        Operaciones numéricas y
                                   manejo de arrays

        SciPy        1.12.0        Pruebas estadísticas
                                   inferenciales
                                   (Kruskal-Wallis,
                                   Chi-cuadrado)

     scikit-learn    1.4.0         Modelado de Machine
                                   Learning y validación
                                   cruzada

       XGBoost       2.0.3         Modelo de clasificación
                                   multiclase (mejor modelo:
                                   F1-Macro 0.9270)

   imbalanced-learn  0.12.0        Balanceo de clases mediante
                                   SMOTE

         SHAP        0.44.0        Explicabilidad del modelo
                                   (Explainable AI)

     Matplotlib /    3.8.2 /       Visualización de datos
       Seaborn       0.13.1        

   Jupyter Notebook  ---           Entorno de desarrollo y
                                   trazabilidad del pipeline
  ------------------------------------------------------------

  : []{#_Toc242806479 .anchor}Tabla 7. Herramientas tecnológicas
  empleadas

El uso combinado de estas herramientas permitió garantizar la
integridad, consistencia y trazabilidad de los datos a lo largo de todo
el proceso.

Como se observa en la Tabla 8, se observa la correspondencia entre base
de datos y diseño metodológico, esta correspondencia permite asegurar
que los datos organizados sean pertinentes y adecuados para responder a
las preguntas de investigación y contrastar las hipótesis formuladas.
Como resultados, se obtuvo un dataset final conformado por 833
estudiantes y 125 variables operacionalizadas, cuya construcción siguió
un proceso metodológico orientado a preservar la consistencia y
confiabilidad de la información. Para ello, se integraron los registros
académicos institucionales con las fichas socioeconómicas mediante un
proceso de fusión validado con INNER JOIN, que permitió conservar el
99.17% de los registros académicos originales. Asimismo, se aplicaron
técnicas de ingeniería de características (feature engineering) para
generar variables relevantes para el análisis y SMOTE para equilibrar la
distribución de las clases de la variable objetivo multiclase. En
conjunto, estos procedimientos permitieron estructurar una base de datos
adecuada para el desarrollo de los modelos predictivos y el análisis del
rendimiento académico, procurando reducir las limitaciones asociadas a
la calidad de los datos y al desbalance entre categorías.

La base de datos construida guarda plena correspondencia con el diseño
metodológico aprobado para esta investigación:

  ---------------------------------------------------------------------
    Elemento del diseño    Correspondencia en la base de datos
  ------------------------ --------------------------------------------
   Enfoque: Cuantitativo   Variables numéricas (21) y categóricas (103)
                           codificadas mediante One-Hot Encoding y
                           Label Encoding; análisis estadístico
                           inferencial (Kruskal-Wallis, Chi-cuadrado,
                           Spearman)

           Nivel:          Pruebas de asociación (Chi-cuadrado,
   Predictivo/Explicativo  Kruskal-Wallis), correlaciones de Spearman y
                           modelado predictivo multiclase con 6
                           algoritmos de Machine Learning

  Diseño: No experimental, Datos recolectados sin manipulación de
        longitudinal       variables, corte longitudinal 2020--2025
       retrospectivo       agregado por estudiante

   Población: Estudiantes  833 registros de estudiantes con información
   de Ingeniería de Minas  académica y socioeconómica completa (99.17%
                           de retención del dataset académico original
                           de 840 registros)

   Unidad de análisis: El  Cada fila representa un estudiante único (n
         estudiante        = 833), con variables académicas, personales
                           y socioeconómicas consolidadas

  Técnica de recolección:  Datos institucionales del sistema académico
    Análisis documental    y fichas socioeconómicas del periodo
                           20201--20252

   Instrumento: Ficha de   124 variables predictoras operacionalizadas
  extracción estandarizada (incluyendo 4 variables derivadas por
                           feature engineering: Tasa de Aprobación,
                           Estabilidad Académica, Ritmo de Egreso,
                           Eficiencia Académica e Índice de Repetición)

     Variable objetivo     Rendimiento académico multiclase: Bajo
                           (\<11), Regular (11-13.99), Alto (≥14) ---
                           basado en Promedio Ponderado General

    Algoritmos evaluados   Regresión Logística, Árbol de Decisión,
                           Random Forest, Gradient Boosting, XGBoost
                           (mejor modelo: F1-Macro = 0.9270) y Red
                           Neuronal MLP

   Métricas de evaluación  Accuracy, Precisión, Recall, F1-Macro,
                           F1-Weighted, ROC-AUC multiclase y Matriz de
                           Confusión

         Técnica de        SHAP (Shapley Additive Explanations) para
       Explicabilidad      interpretación global y local del modelo
                           óptimo.(Nota LIME se descartó por
                           incompatibilidad con el preprocesamiento)

    Técnica de balanceo    SMOTE (Synthetic Minority Over-sampling
                           Technique) aplicado en validación cruzada
                           estratificada de 5 folds
  ---------------------------------------------------------------------

  : []{#_Toc242806480 .anchor}Tabla 8. Correspondencia entre base de
  datos y diseño metodológico

Esta correspondencia asegura que los datos organizados sean directamente
utilizables para responder a las preguntas de investigación y probar las
hipótesis planteadas.

## 

## 

## 

## **Resultados**

La matriz final tuvo con registros correspondientes al periodo 2020-1 a
2025-2, que pertenecen a la escuela profesional de Ingeniería de Minas,
permitió identificar el rendimiento estudiantil y evaluar los modelos de
aprendizaje automático. Los hallazgos se presentan de acuerdo al orden
establecido en los objetivos específicos de la investigación, con el
propósito de mantener una correspondencia directa entre preguntas
planteadas, los procedimientos analíticos y resultados obtenidos.

En relación al primer objetivo específico, dirigido a determinar la
importancia relativa entre variables predictoras de carácter académico,
personal y socioeconómico en la clasificación del rendimiento académico,
se realizó un análisis descriptivo de la variable objetivos y de las
características de la población en estudio.

Los resultados indican que existe una distribución asimétrica entre las
categorías de rendimiento. Como se muestra en la Tabla 9, el nivel
regular concentro la mayor proporción de estudiantes con 61.94%, seguido
de nivel Bajo, que representó el 30.49%. de otra forma el nivel alto
comprendió el 7.57% del total de estudiantes.

Esta distribución muestra un marcado desbalance de clases debido a la
categoría Alto. Por cada estudiante clasificado en el nivel Alto se
encuentran aproximadamente quince estudiantes en el nivel Regular. El
problema no es despreciable ya que un modelo entrenado sobre esta forma
de distribución podría aprender y memorizar la clase mayoritaria y
presentar un desempeño aparentemente elevado no logrando clasificar a ls
estudiantes en las categorías menos representativas. Por ello el
desbalance identificado constituyó uno de los desafíos en metodológicos
del estudio. Una manera como se reduce su efecto en aplicar la técnica
de SMOTE(Synthetic Minority Over- sampling Technique), cuyo objetivo es
generar observaciones sintéticas de las clases minoritarias. Esta
técnica fue aplicada exclusivamente sobre conjuntos de entrenamiento
dentro del proceso de validación cruzada, evitando su aplicación previa
a la aparición de los datos. Este paso metodológico evita la fuga de
información entre los conjuntos de entrenamiento y validación por lo que
permite obtener una estimación más confiable del comportamiento de los
modelos en datos no observados. La distribución observada permite
establecer una consideración importante en la interpretación posterior
de los datos. Debido a que la categoría Alto presenta una representación
menor que la categoría regular y Bajo, las métricas de desempeño no
deben interpretarse de manera aislada. Considerando que será necesario
examinar métricas que son sensibles al desbalance de clases y analizar
el comportamiento específico del modelo en cada categoría de
rendimiento.

En consecuencia, como se observa en la Tabla 9, el análisis exploratorio
inicial permitió caracterizar a la población de estudio y obtener
información relevante para fundamentar las decisiones adoptadas durante
las etapas de preparación y modelado de los datos. Asimismo, la
distribución de las clases evidenció que la predicción del rendimiento
académico representa un desafío que va más allá de una tarea de
clasificación convencional, debido al desbalance existente entre las
categorías Bajo, Regular y Alto. Esta diferencia resulta especialmente
notoria en la clase Alto, que representa únicamente el 7.57% de la
población estudiada. Esta distribución debe tenerse en cuenta al
entrenar y evaluar los modelos, pues la escasa presencia de esta
categoría puede dificultar su identificación y reducir la precisión de
las predicciones.

Por otro lado, la variable del rendimiento académico se clasificó en
tres niveles Bajo, Regular y Alto de acuerdo con los criterios
establecido en el reglamente institucional. Esta categorización permitió
estructurar la variable objetivo del estudio y establecer una base
consistente para entrenar los modelos de aprendizaje automático y
evaluar su capacidad para distinguir entre los distintos niveles de
rendimiento de los estudiantes.

La variable rendimiento académico fue categorizada en tres niveles según
el reglamento institucional:

  ------------------------------------------------------------
      Nivel de      Rango de         Frecuencia   Porcentaje
     rendimiento    promedio                      
  ----------------- ---------------- ------------ ------------
        Bajo        0.00 -- 10.99    254          30.49%

       Regular      11.00 -- 13.99   516          61.94%

        Alto        14.00 -- 20.00   63           7.57%

        Total       ---              833          100.00%
  ------------------------------------------------------------

  : []{#_Toc242806481 .anchor}Tabla 9. Distribución del rendimiento
  académico

Nota: se observa una distribución con predominio del nivel Regular
(61.94%), mientras que la clase Alto representa la minoría (7.57%). Esta
distribución asimétrica negativa (skewness = -1.802) justifica la
aplicación de técnicas de balanceo de clases mediante SMOTE durante el
modelado predictivo.

El análisis estadístico descriptivo de las principales variables
numéricas presentados en la Tabla 2 permitió complementar la
caracterización del rendimiento académico y aproximarse a la trayectoria
formativa de los estudiantes durante el periodo de estudio. Los
resultados evidencian una variación importante en los indicadores
asociados a la permanencia y el desempeño académico.

La Figura 2. muestra la distribución de frecuencias del Promedio
Ponderado General (PPG) de los estudiantes de Ingeniería de Minas entre
2020 y 2025. Se observa una distribución asimétrica negativa (con sesgo
hacia la izquierda), donde la mayor concentración de datos (la moda) se
encuentra en el rango de 11 a 14 puntos y a la presencia de registros
bajos que prolongan la distribución hacia la izquierda. Esta
característica se refleja en que la media (11.17) es inferior a la
mediana (12.07). También se identifica un grupo reducido de registros
próximos a cero, y que podrían estar relacionado a estudiantes retirados
o con registros académicos sin clasificación, aspecto que debe
verificarse en la base de datos. Metodológicamente esta distribución
muestra rendimiento académico heterogéneo. Por lo que, el desbalance
entre las categorías de rendimiento debe evaluarse directamente mediante
la frecuencia de la variable objetivo. En este contexto, el uso de
F1-Macro resulta adecuado para evaluar el desempeño del modelo XGBoost
cuando las clases presentan diferentes tamaños, mientras que SMOTE puede
emplearse sobre el conjunto de entrenamiento para mejorar la
representación de las clases minoritarias.

![[]{#_Toc242806073 .anchor}Fig. 2. Distribución de frecuencias del
promedio ponderado
general.](media/image3.png){width="6.604166666666667in"
height="3.5493055555555557in"}

En la Tabla 10 el promedio ponderado general presenta una media de 11.17
y una mediana de 12.07, con una desviación estándar de 3.09. se observa
una asimetría negativa pronunciada (-1.802) y una curtosis de 3.284
(corresponde a una distribución leptocúrtica), indicando que la mayoría
de calificaciones están concentradas en el rango medio-bajo(entre 10 y
13 puntos), con una cola extendida hacia valores bajos y muy pocos casos
de rendimiento alto (máximo de 16). Esto valida estadísticamente el
desbalance de clases observado en la variable objetivo.

Existe evidencia de una alta dispersión en las variables de progreso.
Mientras que la mediana de semestres cursados es 6, la desviación
estándar es de 4.48, y un máximo de 17 semestres. De manera similar, los
cursos aprobados muestran una desviación estándar muy alta (19.58) en
relación con su media (25.94). confirmando la coexistencia de dos
poblaciones dentro de la muestra: estudiantes con progreso lineal y
estudiantes con rezago académico significativo o trayectorias
discontinuas.

En el caso de la ingeniería de características, se observa que la tasa
de aprobación presenta una media del 76% (0.76), pero con una asimetría
negativa(-1.506). Lo que sugiere, la existencia de un subgrupo crítico
con tasas de aprobación muy bajas (percentil 25% en 0.682),
convirtiéndolo en un predictor discriminante clave. En el caso de la
estabilidad académica la diferencia media entre el mejor y peor semestre
es de 4.44 puntos, y casos extremos de hasta 16.67 puntos de oscilación.
Lo que demuestra que el rendimiento de los estudiantes no es lineal,
validando la necesidad de modelos no lineales (como XGBoost) capaces de
capturar esta volatilidad. Con respecto al ritmo de egreso este tiene
una mediana de 4 cursos aprobados por semestre y una desviación estándar
de 1.62, esta variable normaliza el progreso, permitiendo que el modelo
identifique a estudiantes que, a pesar de tener cursos aprobados,
avanzan a una velocidad inferior a la esperada por la malla curricular.
La estadística descriptiva muestra que los datos no siguen una
distribución normal homogénea. La alta dispersión, la asimetría negativa
en las variables de éxito y la presencia de valores atípicos en las
trayectorias de rezago justifican plenamente el uso de la validación
cruzada estratificada, el balanceo con SMOTE y la selección de
algoritmos basados en árboles de decisión, los cuales son inherente
robustos consecuencia de estas distribuciones.

En segundo lugar, el promedio mínimo semestral y el ritmo de egreso
completan el grupo de variables académicas más influyentes.

  ------------------------------------------------------------------------------------------------------
  Estadístico   PPGENERAL   SEMESTRES   CURSOS      CURSOS         TASA          ESTABILIDAD   RITMO
                            CURSADOS    APROBADOS   DESAPROBADOS   APROBACION    ACADEMICA     EGRESO
  ------------- ----------- ----------- ----------- -------------- ------------- ------------- ---------
  count         833         833         833         833            833           833           833

  mean          11.174      6.615       25.944      5.58           0.76          4.439         3.789

  Desviación    3.091       4.478       19.577      5.578          0.269         3.796         1.624
  estándar                                                                                     

  Mínimo        0           1           0           0              0             0             0

  Percentil 25% 10.49       2           8           1              0.682         1.57          3

  Mediana 50%   12.07       6           23          4              0.846         3.84          4

  Percentil 75% 13.09       10          42          8              0.955         6.12          5

  Máximo        16          17          64          33             1             16.67         6.667

  median        12.07       6           23          4              0.846153195   3.84          3.99996

  Asimetría     -1.802      0.36        0.416       1.286          -1.506        0.913         -0.61
  (skewness)                                                                                   

  kurtosis      3.284       -1.116      -1.081      1.537          1.485         0.245         -0.19
  ------------------------------------------------------------------------------------------------------

  : []{#_Toc242806482 .anchor}Tabla 10. Estadística descriptiva de
  variables numéricas principales

Nota: Datos procesados con Python (pandas, scipy). La asimetría negativa
del promedio ponderado indica una ligera concentración hacia valores
altos.

El segundo objetivo específico, está centrado en comparar la eficiencia
de los algoritmos de aprendizaje automático mediante métricas de
evaluación, requiere examinar primero algunos aspectos del desempeño
académico. Según se aprecia en la Figura 3, el promedio ponderado se
mantuvo cerca de los 11,5 puntos en los diferentes niveles de ingreso
familiar mensual. No obstante, en los estudiantes provenientes de
hogares con ingresos inferiores a los 950 soles se observó una mayor
variabilidad en las calificaciones, incluyendo valores considerablemente
bajos, próximos a cero. Estos resultados indican que, si bien el nivel
socioeconómico no mostró diferencias importantes en el promedio
académico, los menores ingresos podrían estar relacionados con una mayor
presencia de casos de rendimiento muy bajo. Dicho de otra manera, las
diferencias no aparecieron tanto en el estudiante "típico", sino en
aquellos casos extremos donde las dificultades académicas son más
evidentes.

![[]{#_Toc242806074 .anchor}Fig. 3. Rendimiento académico según el nivel
de ingreso familiar.](media/image4.png){width="6.604166666666667in"
height="3.7319444444444443in"}

La Figura 4 muestra que las medianas del rendimiento académico son
similares en la mayoría de los tipos de colegio, situándose
aproximadamente entre 11 y 13 puntos, lo que sugiere que el origen
educativo no determina diferencias marcadas en el rendimiento central.
Sin embargo, se observan diferencias en la dispersión y forma de las
distribuciones: los colegios particulares y estatales presentan mayor
concentración alrededor de 12 a 13 puntos, mientras que los parroquiales
muestran una mayor asimetría y presencia de valores bajos. Por su parte,
los colegios militares presentan una mediana relativamente menor,
cercana a 10 puntos. Agrupando estos resultados muestran que el tipo de
colegio parece relacionarse más con la variabilidad y el riesgo de bajo
rendimiento que con diferencias sustanciales en el rendimiento
promedio.![](media/image5.png){width="6.604166666666667in"
height="4.3902777777777775in"}

[]{#_Toc242806075 .anchor}Fig. 4. Distribución del rendimiento según
tipo de colegio.

Para comprobar si las diferencias observadas eran estadísticamente
significativas, se aplicó la prueba no paramétrica de Kruskal-Wallis,
debido a que el promedio ponderado general no cumple con el supuesto de
normalidad, de acuerdo con la prueba de Shapiro-Wilk (p\<0.05). Como se
muestra en la Tabla 11, el análisis arrojó un estadístico H = 6.9414 y
p- valor = 0.225. Dado que este p-valor es superior al nivel de
significancia establecido 0.05, no se rechaza la hipótesis nula. En
consecuencia, se concluye que no existen diferencias estadísticamente
significativas en el rendimiento académico según el tipo de colegio de
procedencia en la muestra de 833 estudiantes analizados..

  -----------------------------------------------------
  Concepto                  Valor
  ------------------------- ---------------------------
  Estadístico H             6.9414

  p-valor                   0.2250

  Nivel de significancia    0.05
  (α)                       

  Decisión                  No Rechazar H₀

  Conclusión                No existen diferencias
                            estadísticamente
                            significativas en el
                            rendimiento académico según
                            el tipo de colegio de
                            procedencia
  -----------------------------------------------------

  : []{#_Toc242806483 .anchor}Tabla 11. Resultados de la prueba
  Kruskal-Wallis

Interpretación: Los estudiantes provenientes de colegios particulares no
presentan un promedio ponderado significativamente diferente al de
aquellos provenientes de colegios estatales (p = 0.2250 \> 0.05).

Así mismo se aplicó la prueba de Chi-cuadrado de independencia para
analizar la posible relación entre el estado civil de los padres y el
nivel de rendimiento académico. Como se muestra en la Tabla 12, se
obtuvo un estadístico de χ² = 6.5339, con 6 grados de libertad y un p \<
0.3661, al ser p \<0.05, no se rechaza la hipótesis nula, indicando esto
que una asociación estadísticamente significativa entre ambas variables.
Este resultado sugiere que, en nuestro análisis, el estado civil de los
padres no presenta una relación significativa con el nivel de
rendimiento académico. Esta relación se aprecia con mayor claridad en la
tabla 5, donde se presenta la distribución porcentual por filas. Los
estudiantes cuyos padres estaban casados registraron la mayor proporción
de rendimiento Alto (6.8%), mientras que aquellos cuyos padres eran
divorciados presentaron la menor proporción en este nivel (3.7%) y, a la
vez, la mayor concentración en el nivel Bajo(38.9%). Estos resultados
sugieren que el contexto familiar podría estar relacionado con el
desempeño académico, aunque la asociación estadística, por sí misma, no
permite afirmar que el estado civil de los padres sea una causa directa
del rendimiento estudiantil.

La Tabla 12 muestra que la prueba Chi-Cuadrado obtuvo un χ² = 6.5339.
con 6 grados de libertad y un p-valor = 0.36611. debido a que el p-valor
es mayor que α = 0.05, no se rechaza la hipótesis nula. Por lo tanto, no
existe una relación estadísticamente significativa entre el estado civil
de los padres y el rendimiento académico de los estudiantes de
Ingeniería de Minas. En los datos analizados, ambas variables pueden
considerarse independientes.

  -----------------------------------------------------
  Concepto                  Valor
  ------------------------- ---------------------------
  Estadístico χ²            6.5339

  p-valor                   0.36611

  Grados de libertad        6

  Nivel de significancia    0.05
  (α)                       

  Decisión                  No rechazar H₀

  Conclusión                No existe dependencia
                            estadísticamente
                            significativa entre el
                            estado civil de los padres
                            y el rendimiento académico
  -----------------------------------------------------

  : []{#_Toc242806484 .anchor}Tabla 12. Resultados de la prueba
  Chi-Cuadrado de independencia

  -----------------------------------------------------------------
  ESTADO_CIVIL_PADRES    Rendimiento   Rendimiento    Rendimiento
                         Alto(%)       Bajo(%)        Regular(%)
  ---------------------- ------------- -------------- -------------
  Casados                7             21.6           71.4

  Convivientes           3.14          28.3           68.55

  Divorciados            5.68          37.5           56.82

  Separados              11.63         29.07          59.3
  -----------------------------------------------------------------

  : []{#_Toc242806485 .anchor}Tabla 13. Tabla de contingencia- Estado
  civil de los padres vs. Rendimiento(porcentajes por filas)

Nota: Los porcentajes representan la distribución dentro de cada
categoría de estado civil de los padres.

El tercer objetivo, Figura 5, específico analizó las relaciones entre
las principales variables académicas mediante la correlación de
Spearman. Los resultados presentan una relación positiva moderada entre
el promedio ponderado y los cursos aprobados (p = 0.391), y una relación
negativa fuerte con los cursos desaprobados (p = -0.742). también se
observan correlaciones muy fuertes entre el promedio ponderado y la tasa
de aprobación (p = 0.931) y el ritmo de egreso (p = 0.857), evidenciando
una estrecha asociación entre rendimiento, eficiencia y continuidad
académica. La relación más alta como se observa se presenta entre cursos
aprobados y semestres cursados (p = 0.913). En resumen, los resultados
muestran asociaciones importantes entre las variables académicas, aunque
no implican causalidad.

![](media/image6.png){width="6.604166666666667in"
height="5.945138888888889in"}

[]{#_Toc242806076 .anchor}Fig. 5. Matriz de correlación de Sperman entre
variables numéricas.

Nota: Coeficientes de correlación de Spearman calculados con método
pairwise. La triangular superior se omitió para facilitar la lectura.
Los valores cercanos a 1 (azul) indican correlación positiva fuerte,
mientras que los valores cercanos a -1 (rojo) indican correlación
negativa fuerte.

El cuarto objetivo específico, Figura 6, está orientado a determinar el
mejor modelo predictivo para predecir el rendimiento académico,
comparando seis algoritmos de clasificación multiclase. Los resultados
muestran evidencia de una clara ventaja de los modelos de ensamble,
especialmente los que se basan en boosting. El modelo XGBoost obtuvo
métricas F1-Macro de 0.9270 ± 0.0325 y un Accuracy de 0.9531± 0.0169 en
la validación cruzada estratificada de cinco pliegues. Le siguieron
Gradient Boosting (0.9096), Árbol de Decisión (0.8684), Random Forest
(0.8635), Regresión Logística (0.8020) y Red Neuronal Multicapa
(0.7747). Para controlar el desbalance de las clases, se aplicó SMOTE
únicamente sobre los datos de entrenamiento dentro de cada pliegue,
evitando que los datos de validación fueran alterados. Esta estrategia
redujo el riesgo de fuga de datos (data leakage) y permitió obtener una
estimación más confiable de la capacidad de generalización. En resumen,
los resultados confirman que XGBoost presentó la mejor capacidad
predictiva, siendo seleccionado como el modelo más apropiado para el
rendimiento académico.

  --------------------------------------------------------------------------------------
  Modelo      Accuracy        F1-Macro    F1-Weighted   Precision-Macro   Recall-Macro
  ----------- --------------- ----------- ------------- ----------------- --------------
  Regresión   0.8884 ± 0.007  0.8020 ±    0.8879 ±      0.8035 ± 0.0247   0.8025 ±
  Logística                   0.0248      0.0075                          0.0279

  Árbol de    0.9232 ± 0.0108 0.8684 ±    0.9236 ±      0.8635 ± 0.0179   0.8760 ±
  Decisión                    0.0068      0.010                           0.0118

  Random      0.9292 ± 0.0060 0.8635 ±    0.9262 ±      0.9073 ± 0.0322   0.8366 ±
  Forest                      0.0317      0.007                           0.0336

  Gradient    0.9436±0.0112   0.9096 ±    0.9438 ±      0.9041 ± 0.0096   0.9184 ±
  Boosting                    0.0133      0.0117                          0.0289

  XGBoost     0.9531 ± 0.0169 0.9270 ±    0.9531 ±      0.9304 ± 0.0331   0.9272 ±
                              0.0325      0.0169                          0.0417

  Red         0.8860 ± 0.0171 0.7747 ±    0.8820 ±      0.7905 ± 0.0540   0.7650 ±
  Neuronal                    0.0502      0.0187                          0.0453
  (MLP)                                                                   
  --------------------------------------------------------------------------------------

  : []{#_Toc242806486 .anchor}Tabla 14. Resultados de validación cruzada
  (5-Folds, con SMOTE)

Nota: Métricas calculadas mediante validación cruzada estratificada de 5
pliegues con balanceo de clases mediante SMOTE aplicado exclusivamente
en los conjuntos de entrenamiento. Los valores representan media ±
desviación estándar.

Para la evaluación del modelo XGBoost sobre el conjunto de prueba
independiente, correspondiente al 20 % de los datos (n= 167), confirmó
su elevado desempeño predictivo, tal y como se observa en la matriz de
confusión de la Figura 6, el modelo clasifica correctamente 50 de las 51
estudiantes de la clase bajo, alcanzando un Recall de 98.04% y
registrando solo un caso clasificado erróneamente como Regular.
Resultado que es especialmente importante en un posible sistema de
alerta temprana, debido a que detectar oportunamente a los estudiantes
con bajo rendimiento puede facilitar activar las acciones de apoyo. De
otra manera, el modelo obtuvo una precisión del 100% en la clase Alto,
acertando correctamente las 10 predicciones realizadas, mientras que
para la clase Regular alcanzó un 96.19%. en la categoría Alto, el
F1-score fue de 0.8696, cuyo resultado debe interpretarse considerando
que se trata de una clase minoritaria, con apenas 13 estudiantes en el
conjunto de prueba. En términos generales, XGBoost alcanzó una Accuracy
de 96.41 demostrando una elevada capacidad para clasificar correctamente
a estudiantes que no participaron en su entrenamiento. En conjunto,
estos resultados muestran que el modelo distingue las tres categorías de
rendimiento con un margen de error pequeño, especialmente en la
identificación de los estudiantes que tienen bajo desempeño académico.

![[]{#_Toc242806077 .anchor}Fig. 6. Matriz de confusión del modelo
XGBoost.(Conjunto de
prueba)](media/image7.png){width="5.07240813648294in"
height="4.001388888888889in"}

Nota: Los valores en las celdas representan el número de estudiantes
clasificados correctamente (diagonal) e incorrectamente (fuera de la
diagonal). El Recall del 98.04% para la clase Bajo evidenció una mínima
presencia de falsos negativos (sólo 1), , condición esencial para el
sistema de alerta temprana.

En la Figura 7 mostramos la curva ROC multiclase del modelo XGBoost
optimizado, y su poder de predicción de los tres niveles (alto, Bajo y
Regular) en estudiantes de ingeniería

Los tres valores AUC se encuentran muy por sobre el umbral de 0.9
significa que tiene una capacidad discriminativa excelente. La clase
Bajo rendimiento tiene el más alto AUC (0.997), respaldando nuestro
objetivo del estudio, lo que confirmaría que el modelo identifica con
alta precisión a los estudiantes en riesgo académico, esto facilitaría
la implementación oportuna y consecuentemente habilitar estrategias de
intervención, así como su aplicación en sistemas de alerta temprana en
la gestión académica universitaria.

![[]{#_Toc242806078 .anchor}Fig. 7. Curva ROC Multiclase del Modelo
XGBoost optimizado](media/image8.png){width="5.215277777777778in"
height="3.9885564304461942in"}

El quinto objetivo, ilustrado en la Figura 8, consistió en descubrir qué
variables pesan más en las predicciones del modelo. Para ello usamos
SHAP Summary Bar Plot, una técnica de inteligencia artificial explicable
que mide el impacto promedio absoluto de cada característica,
diferenciando entre las tres clases de rendimiento: Clase 0 (Alto),
Clase 1 (Bajo) y Clase 2 (Regular). La tasa de aprobación es el
predictor más fuerte del modelo, sobre todo para detectar estudiantes en
riesgo de bajo rendimiento (Clase 1). Esto tiene sentido: un estudiante
que reprueba muchos cursos difícilmente tendrá un buen promedio. Le
siguen en importancia el promedio del semestre más bajo y el semestre
más alto, dos indicadores que retratan la trayectoria real del
estudiante, con sus altibajos. Otras variables académicas relevantes
fueron el promedio del último semestre, el número de cursos desaprobados
y el ritmo de egreso. En cambio, los factores socioeconómicos, ingreso
familiar, tipo de vivienda, tenencia de computadora o refrigerador,
colegio de procedencia, quedaron relegados al final del ranking, con
aporte mínimo. En otras palabras, el modelo observa primero el historial
académico antes que el contexto familiar o social. Esto no significa que
lo socioeconómico sea irrelevante, sino que , para predecir el
rendimiento, lo que el estudiante ha hecho en sus estudios pesa más que
se dónde viene. El gráfico muestra el promedio de los valores absolutos
de SHAP por variable y por clase, lo que permite comparar de forma justa
la contribución de cada una dentro del modelo.

.

![](media/image9.png){width="5.574548337707786in"
height="5.652777777777778in"}

[]{#_Toc242806079 .anchor}Fig. 8. SHAP Summary Plot: Importancia global
de variables

*Nota:* Las variables se presentan en orden descendente según su
importancia global. La coloración en la figura representa a las
distintas categorías, la clase 0 es Alto de color verde, la clase 1 es
Bajo de color rosa, y la clase 2 es Regular de color azul.

La Figura 9 permitió medir la importancia global de las características
mediante el promedio de los valores absolutos de SHAP(mean(\|SHAP\|)).
Los resultados muestran una tendencia clara, es decir, las variables
relacionadas con la trayectoria académica tienen un peso mucho mayor en
las predicciones que las variables de carácter socioeconómicas. La tasa
de aprobación ocupó el primer lugar del ranking, con una contribución
explicativa notablemente superior a la del resto de características. Su
influencia fue especialmente importante en la Clase 1 (Bajo), lo que
indica que constituye el predictor más relevante para identificar a los
estudiantes que podrían encontrarse en riesgo académico. Lo siguieron
promedio de semestre mínimo, en segundo lugar, también con una fuerte
influencia sobre la Clase 1, y promedio de semestre máximo, en tercer
lugar, cuyo impacto se concentró principalmente en la Clase 0 (Alto).
Esto sugiere que los estudiantes con mejor desempeño tienden a presentar
promedios semestrales elevados. En cuarto y quinto lugar se ubicaron
promedio de último semestre y cursos desaprobados, completando el grupo
de variables académicas con mayor capacidad predictiva. De otra manera,
características como ritmo de egreso, curso aprobado y diversos
indicadores socioeconómicos, entre ellos la actividad de danza, tenencia
de refrigerador, ingreso familiar, seguro SIS y tipo de vivienda, se
observa una contribución mucho menor y se ubicaron en la parte inferior
del ranking.

Esto está relacionado con la Teoría del comportamiento de Tinto \[4\],
que resalta la importancia de la integración y experiencia académica en
la permanencia y el éxito universitario. En este sentido, el modelo
parece encontrar una señal bastante clara: para predecir el rendimiento
académico, es interesante observar cómo ha sido el desempeño académico
del estudiante a lo largo de su vida universitaria y que únicamente las
características socioeconómicas de las que parte.

![](media/image10.png){width="5.616067366579178in"
height="6.060416666666667in"}

[]{#_Toc242806080 .anchor}Fig. 9. Gráfico SHAP: Tasa de aprobación y
Predicción.

Nota. Los resultados SHAP muestran que la tasa de aprobación es por un
gran margen, la variable que más influyo en las predicciones del modelo.
En importancia sigue el promedio mínimo semestral, el promedio máximo
semestral, el promedio del último semestre y el número de cursos
desaprobados. Todas estas cinco variables académicas dominan la
capacidad predictiva del modelo. Los factores socioeconómicos (ingreso
familiar, tenencia de refrigerador o tipo de vivienda) y otras
características categóricas son de influencia marginal en comparación.
Significando que el desempeño académico histórico del estudiante es
decisivamente más importante que sus características socioeconómicas en
la predicción del rendimiento a futuro.

La Figura 10 muestra que existe una dependencia entre la tasa de
aprobación y el bajo rendimiento y que esta relación no es lineal. Se
observan cambios pronunciados en ciertos umbrales, y su efecto en las
predicciones varía dependiendo del valor de la tasa. Cuando esta
disminuye por debajo de -0.5, los valores SHAP se incrementan con
rapidez y se aproximan a +4, esto indica una contribución relevante a
que el modelo clasifique al estudiante en la categoría de bajo
rendimiento. A diferencia de cuando la tasa es superior a 0, los valores
SHAP se vuelven negativos y pueden alcanzar cifras como -3.

Lo que sugiere que, a partir de ese punto, la variable influye a que se
reduzca la probabilidad de esa clasificación. Dicho de otra manera,
mientras que los valores bajos de la tasa de aprobación refuerzan la
predicción de un rendimiento académico deficiente, los valores más altos
tienden a actuar en sentido opuesto. .

En la Fig. 10, el gráfico permite observar cómo es la relación entre el
promedio mínimo semestral y la tasa de aprobación, interacción que
permite observar los colores. Los puntos azules, correspondientes a
promedios mínimos más bajos, se agrupan principalmente en las áreas
donde las tasas de aprobación son menores. A diferencia de los puntos
magenta se presentan en los valores más altos, esto refleja una
trayectoria académica más estable. Y es que, aunque este comportamiento
no demuestra por sí solo una relación causal, si indica rastros de que
mantener un historial favorable de aprobación puede contribuir a
disminuir el riesgo de bajo rendimiento académico.

Globalmente estos resultados permiten entender la razón por la que
XGBoost alcanzó un valor superior al de la Regresión Logística. Esto se
debe a como cada modelo interpreta los datos. Como los modelos basados
en árboles de decisión son capaces de reconocer relaciones no lineales,
detectar cambios bruscos e identificar combinaciones de variables que
influyen en el resultado, la regresión logística parte de una estructura
más limitada para representar patrones complejos. Dicho de otra manera,
es como tener una gran idea del recorrido, pero difícilmente reflejará
todos sus giros. Esa es la razón de que cuando los datos presentan
comportamientos menos evidentes o relaciones que cambian según la
circunstancia, XGBoost puede adaptarse mejor y ofrecer predicciones más
precisas.

![Fig. 10. Efecto tasa de aprobación en predecir Rendimiento
Bajo.](media/image11.png){width="6.604166666666667in"
height="4.107638888888889in"}

Nota: El gráfico muestra una relación inversa clara: cuando la tasa de
aprobación es baja, es decir, valores negativos en el eje horizontal,
los valores SHAP son positivos y altos cercanos a 4, esto indica que
esta condición aumenta significativamente la probabilidad de clasificar
al estudiante en bajo rendimiento. De manera contraria, si la tasa de
aprobación es grande esto generan valores SHAP negativos, entre -2 a -3,
lo que reduce la probabilidad. La dispersión vertical de los puntos y su
coloración según el promedio mínimo semestral muestran que el efecto de
la tasa de aprobación varía según la interacción con el desempeño
histórico del estudiante.

.

En la categoría de bajo rendimiento, el modelo alcanza un Recall de
0.9804, esto quiere decir, que identificó correctamente al 98.04% de los
estudiantes con esta característica. Este resultado tiene implicaciones
directas en el diseño de un sistema de alerta temprana. Un Recall de
98.04% en la clase "Bajo" significa que el modelo identifica
prácticamente a todos los estudiantes en riesgo antes de que el problema
escale, lo que permite activar tutorías, nivelaciones o apoyo
socioeconómico mientras se pueda intervenir. En la práctica el modelo no
solo predice un resultado académico: reduce el costo operativo de los
falsos negativos, que en este contexto son mucho más graves que una
alerta innecesaria.

Este resultado deja claro que la calidad de las predicciones no depende
solamente del algoritmo elegido. Detrás de un buen modelo hay un trabajo
previo anticipado de selección de variables y limpieza de datos que
muchas veces pasa como sin importancia, pero esto es lo que marca la
diferencia entre un resultado útil y un resultado que simplemente se ve
bien en un artículo científico. En el contexto educativo, donde las
decisiones se ven planes de vida afectadas, ese rigor en la preparación
de los datos no es opcional.

La integración de las variables académicas históricas y socioeconómicas,
junto con la aplicación de SMOTE exclusivamente sobre los conjuntos de
entrenamiento dentro de cada pliegue, permitió abordar el desbalance
existente entre las clases (516 Regular, 254 Bajo y 63 Alto) sin
comprometer la validez de la evaluación mediante data leakage. De esta
manera, los resultados obtenidos ofrecen una estimación más real de la
capacidad del modelo para generalizar ante estudiantes que no
participaron en su entrenamiento\[52\]. A este desempeño predictivo se
agrega el análisis de Inteligencia Artificial Explicable (XAI) mediante
valores SHAP (Shapley Additive exPlanations), que permitió comprender
qué variables estaban detrás de las predicciones. Los resultados
mostraron que la tasa de aprobación, el promedio semestre mínimo y el
promedio semestre máximo fueron las características con mayor
influencia, mientras que las variables socioeconómicas tuvieron una
contribución considerablemente menor: En conclusión, estos resultados
muestran que el modelo no solo es capaz de anticipar el rendimiento
académico con un alto nivel de precisión, sino que también permite
comprender cuáles son los factores que más intervienen en sus
predicciones. En otras palabras, XGBoost no se limita a decir qué podría
ocurrir, sino que, además, ofrece evidencia sobre señales académicas
están por detrás de esa predicción. Por ello, el modelo se presenta como
una herramienta potencialmente útil para identificar de manera temprana
a estudiantes en riesgo y apoyar la toma de decisiones institucionales
en las instituciones de educación superior universitaria.

La fase final de CRISP-DM consiste en planificar la implementación
operativa del modelo en el entorno institucional, asegurando que los
resultados de la investigación se traduzcan en una herramienta útil para
la toma de decisiones académicas. Aunque el presente estudio se limita
al desarrollo y validación del modelo predictivo, se propone un plan de
despliegue que es adoptado por la escuela profesional de Ingeniería de
Minas\[53\].

Para el despliegue en el entorno institucional, el modelo XGBoost se
acopla al sistema de gestión académica mediante una arquitectura modular
de tres niveles.

El primer componente es un módulo de extracción de datos que, al empezar
cada semestre, consultará automáticamente el registro académico e
histórico y las fichas socioeconómicas de los estudiantes matriculados.
El segundo componente es el motor de predicción, que aplica el pipeline
de preprocesamiento (imputación, codificación one-hot, estandarización)
y ejecuta el modelo XGBoost para generar clasificaciones de riesgo (Bajo
Regular y Alto) junto con valores SHAP que explican cada predicción. El
tercer componente es un dashboard de visualización accesible para
tutores y responsables de bienestar universitario, que muestra listados
de estudiantes en riesgo por probabilidad, gráficos de importancia de
variables, recomendaciones de intervención basadas en los factores SHAP
dominantes\[54\].

En relación con el plan de implementación por fases, el despliegue se
estructura de manera gradual en tres etapas. La primera etapa que dura
entre uno y tres meses es etapa piloto y que consiste en ejecutar el
modelo de manera retrospectiva sobre el semestre actual, comparando las
predicciones con el rendimiento real al final del periodo para validar
la efectividad en condiciones operativas. En la segunda etapa sería una
implementación controlada de cuatro a seis meses, implica integrar el
modelo al sistema de matrícula, generando alertas automáticas para los
tutores asignados, quienes reciben reportes individuales de estudiantes
en riesgo con recomendaciones específicas(tutoría y orientación de algún
servicio de OBU). En la etapa tres, operación continua, establece un
ciclo de retroalimentación donde los resultados de las intervenciones se
registran y utilizan para reentrenar el modelo semestralmente, mejorando
su precisión con datos actualizados \[55\].

En el monitoreo y mantenimiento del modelo, con el fin de garantizar la
vigencia del modelo a lo largo del tiempo, se establece un protocolo de
monitoreo de tres indicadores clave. El indicador de deriva de datos
(data drift) compara la distribución de las variables predictoras en
cada semestre con la distribución histórica, alertando cuando se
detectan cambios significativos que podrían afectar la precisión del
modelo. El indicador de desempeño predictivo evalúa trimestralmente la
exactitud y sensibilidad del modelo sobre los estudiantes cuyo
rendimiento ya se conoce, estableciendo un umbral mínimo de F1 -- score
de 0.85 para activar reentrenamiento. El indicador de impacto
institucional mide la correlación entre las predicciones del modelo y
las tasas de deserción y reprobación, verificando que el sistema
contribuye de manera efectiva en la mejora de los indicadores académicos
\[56\].

Para las consideraciones éticas y de privacidad, el despliegue del
modelo respeta estrictamente la ley de protección de datos personales
Ley N°29733 y el código de ética en Investigación de la Universidad
César Vallejo (RCU N°0157-2025). Todos los datos se anonimizan antes del
procesamiento, eliminando identificadores directos (DNI, nombres,
códigos de estudiante). Las predicciones se utilizan exclusivamente como
herramienta de apoyo a la decisión, nunca como criterio único para
sanciones académicas o restricciones de matrícula. Los estudiantes
tienen derecho a conocer que existen sistemas de predicción de
rendimiento y solicitar explicaciones sobre las predicciones que les
afecten, en cumplimiento con los principios de transparencia algorítmica
y derecho a la explicación establecidos en la doctrina de Inteligencia
Artificial Explicable (XAI) \[57\].

Con respecto a las limitaciones del despliegue, es importante reconocer
que el modelo fue entrenado con datos de una sola institución y en un
periodo específico (2020-2025), por lo que su aplicación en otras
universidades o carreras requiere validación externa y posible
recalibración. Asimismo, la ausencia de variables psicosociales y
conductuales limita la capacidad del modelo para capturar dimensiones
importantes del rendimiento académico, por lo que se recomienda
complementar las predicciones con evaluaciones cualitativas realizadas
por tutores y psicólogos educativos \[58\].

## **Discusión (de ser pertinente)**

En esta investigación los resultados obtenidos confirman que los
algoritmos de aprendizaje automático, y en particular el modelo XGBoost,
son altamente efectivos en la predicción del rendimiento académico en
estudiantes de Ingeniería de Minas de una universidad pública del sur de
Perú. Bajo un esquema de validación cruzada estratificada de cinco
particiones, el Modelo XGBoost tiene una métrica F1-Macro de 0.9270 ±
0.0325 y una precisión de 0.9531 ± 0.0169. Cifras que no sólo superan
ampliamente el umbral del 80% establecido en la hipótesis general, sino
que la baja desviación estándar entre particiones indica que el modelo
generaliza bien y no depende de un subconjunto particular de los datos.

Al evaluar el modelo sobre el conjunto de prueba (hold-out del 20%), se
registró una exactitud de 0.9641 y un F1-Macro de 0.9101. No obstante,
la sensibilidad (Recall) de 0.9804 obtenida en la clase "Bajo"
constituye el resultado de mayor peso técnico para el despliegue de un
sistema de Alerta Temprana. Al identificar al 98.04% de los estudiantes
en situación de riesgo, el modelo suprime drásticamente la tasa de
falsos negativos, satisfaciendo así el requisito operacional fundamental
para evitar que casos de vulnerabilidad académica pasen desapercibidos.

Estos resultados están en concordancia con lo que reportan \[13\] y
\[33\] en sus revisiones sobre los modelos de ensamble aplicados a la
predicción del desempeño estudiantil: los métodos basados en boosting y
baagging, como Random Forest y XGBoost, muestran un rendimiento
consistentemente superior frente a los modelos lineales tradicionales.
La razón técnica es clara, estos algoritmos capturan interacciones de
orden alto y relaciones no lineales entre las variables predictoras de
forma automática, sin depender de transformaciones manuales previas
sobre los datos. Frente a estudios previos desarrollados en contextos
latinoaméricanos, las métricas obtenidas en este trabajo resultan más
altas. Por ejemplo, \[5\] alcanzó una precisión del 78% y \[32\] reportó
un F1-score de 0.82. Esta brecha no se explica por el volumen de datos
disponibles, sino por las decisiones metodológicas tomadas durante el
preprocesamiento. Tres aspectos resultaron determinantes: primero, la
integración conjunta de variables académicas y socioeconómicas en un
mismo espacio de características, en lugar de modelarlas por separado;
segundo, la aplicación de ingeniería de características para construir
variables derivadas como la tasa de aprobación y el ritmo de egreso, que
condensan información de la trayectoria estudiantil en indicadores más
discriminantes; y tercero, la aplicación correcta de SMOTE
exclusivamente sobre los conjuntos de entrenamiento dentro de cada fold
de la validación cruzada, evitando así la contaminación de los datos de
validación con instancias sintéticas, una práctica que, de no
considerarse, infla artificialmente las métricas por data leakage.

Este último hecho es foco de atención especial. Una práctica común, pero
equivocada, consiste en aplicar el sobre muestreo sobre todo el dataset
antes de partirlo en folds, lo que filtra información sintética al
conjunto de validación cruzada estratificada de cinco pliegues. De esta
manera, los datos de validación mantuvieron su distribución original,
sin instancias sintéticas, y las métricas de evaluación reflejan la
capacidad real de generalización del modelo sobre datos no vistos.

Esta estrategia de aislamiento del sobre muestreo dentro del pipeline de
validación es, una práctica estándar para evitar la fuga de datos o data
leakage en problemas con clases desbalanceadas, y coincide con lo
recomendado por Kwakye \[59\] en sus directrices sobre evaluación
robusta de modelos predictivos.

El análisis de Explicabilidad con valores SHAP puso en evidencia que el
modelo se apoya exclusivamente en indicadores de trayectoria académica
para tomar sus decisiones. El ranking de importancia lo encabezó la tasa
de aprobación, seguido del promedio semestral mínimo, el promedio
semestral máximo, el ritmo de egreso y el número de cursos desaprobados.
Es interesante desde el punto de vista interpretativo es el patrón de
contribución, tasas de aprobación bajas y promedios mínimos reducidos
impulsan la predicción hacia la clase "Bajo", mientras que un ritmo de
egreso alto contribuye positivamente a la clasificación en "Alto". Este
comportamiento es congruente con lo reportado por Al-Ameri et al.\[60\]
y Balcioğlu y Artar \[61\], quienes también identificaron el historial
académico previo como el predictor dominante en modelos de este tipo.
Más allá del ranking global, la ventaja de SHAP radica en que permite
descomponer cada predicción individual y cuantificar cuánto aporta cada
característica al resultado final, algo que Lundberg y Lee \[18\] y
Qiang et al. \[62\] señalan como clave para la transparencia de modelos
de caja negra.

Por otro lado, las variables socioeconómicas, ingreso familiar, tipo de
colegio, tenencia de computadora o internet, condiciones de vivienda,
aportaron muy poco al poder predictivo del modelo. Sus valores SHAP
fueron consistentemente bajos, lo que indica que el modelo apenas las
usa para discriminar entre clases. Este resultado no es sorprendente y
coincide con lo encontrado por Saldaña et al. \[63\] y López et
al.\[64\], quienes también reportaron que, una vez que se incorporan
variables de historial académico, los factores contextuales pierden peso
relativo en la clasificación.

Los hallazgos en la práctica coinciden con los postulados de la Teoría
del Capital Humano de Becker, evidenciando que, al ingresar a la
educación superior, la trayectoria académica acumulada opera como un
predictor del desempeño futuro con un peso muy superior al de las
condiciones socioeconómicas de origen. Al examinar la importancia de las
variables en la ingeniería de características, resulta claro que los
indicadores de historial académico aportan señales más directas y un
mayor poder discriminativo al modelo en comparación con las métricas de
contexto familiar. Esto no implica que el entorno socioeconómico carezca
de relevancia, sino que su impacto parece estar mediado o absorbido por
el rendimiento previo del estudiante. Esta lectura se sostiene al
contrastar las pruebas de inferencia estadística. La prueba no
paramétrica de Kruskal-Wallis descartó la existencia de diferencias
significativas en el rendimiento según el tipo de colegio de procedencia
( H = 6.94; p 0 0.225). De igual forma, el estadístico Chi-cuadrado de
independencia no arrojó evidencia suficiente para establecer una
asociación entre el estado civil de los padres y el nivel de rendimiento
(χ² = 6.53; p = 0.366), lo que ratifica la preeminencia de las variables
académicas sobre las socioeconómicas en este contexto.

Ambos p-valores, muy por encima del umbral de 0.05, indican que estas
variables socioeconómicas, analizadas de forma aislada, no aportan
suficiente poder explicativo para discriminar entre niveles de
rendimiento en esta muestra. Es un hallazgo congruente con lo que
encuentre en la literatura de Educational Data Mining \[65\], en
muestras de tamaño moderado, las variables académicas históricas tienden
a dominar el poder predictivo frente a las variables de contexto.

La matriz de Spearman permitió identificar estrechas entre las variables
académicas. La tasa de aprobación mostró una correlación muy fuerte con
el promedio ponderado general (p = 0.931), mientras que cursos aprobados
presento una asociación igualmente elevada con semestres cursados (p =
0.913). estas asociaciones respaldan la utilidad de variables derivadas,
ya que permiten resumir de manera más clara la trayectoria académica de
los estudiantes y comprender mejor su evolución a lo largo de los
estudios.

Al evaluar el desempeño de los seis algoritmos , XGBoost obtiene el
mejor F1-Macro (0.9270), seguido de Gradient Boosting (0.9096), Árbol de
Decisión (0.8684), Random Forest (0.8635), Regresión Logística (0.8020)
y Red Neuronal Multicapa (0.7747). La superioridad de los modelos
basados en boosting coincide con lo reportado en recientes estudios
sobre minería de datos educativos\[26\], \[27\], \[61\]. Asimismo, el
hecho de que la Regresión Logística superara a la Red Neuronal Multicapa
evidencia que una mayor complejidad algorítmica no garantiza
necesariamente mejores resultados, en línea con lo señalado en estudios
que tratan sobre modelado interpretable en educación superior \[12\],
\[60\].

En el contexto de un Sistema de Alerta Temprana (SAT), académico, el
Recall de 98.04% obtenido para la clase "Bajo" tiene una lectura
operativa directa y de cada 51 estudiantes realmente en riesgo, el
modelo identificó 50, dejando pasar sólo uno. Esta cifra cobra sentido
cuando se analiza la matriz de costos asociada a los errores de
clasificación. Un falso positivo, etiquetar como "Bajo" a un estudiante
cuyo rendimiento es Regular o Alto, implica básicamente una revisión
tutorial adicional, un costo operativo bajo y sin consecuencias
negativas para el alumno. Un falso negativo, en cambio, significa dejar
sin acompañamiento a un estudiante que efectivamente está en riesgo, lo
que en la práctica se traduce en reprobación, rezago o abandono.
\[2\],\[9\], \[66\].

Dada esta asimetría, el modelo prioriza deliberadamente la sensibilidad
sobre la precisión en la clase crítica, una decisión de diseño coherente
con el propósito preventivo del SAT: intervenir antes de que la
dificultad académica se consolide. Las acciones que se habilitan con
esta detección temprana, tutorías focalizadas, cursos de nivelación,
seguimiento de bienestar universitario, son mucho más efectivos cuando
se activan en las primeras semanas del ciclo que cuando se aplican a
mitad de semestre, cuando el estudiante ya acumuló varias
desaprobaciones. Este enfoque preventivo, además, se alinea con los
principios de responsabilidad social universitaria al orientar los
recursos institucionales hacia quienes más los necesitan, tal y como lo
discuten Hilliger et al.\[2\], Kotorov et al. \[66\] y Kwakye \[59\] en
sus trabajos sobre analíticas del aprendizaje aplicadas a la retención
estudiantil.

No basta con observar métricas favorables; es fundamental cuestionar la
solidez de estos resultados. El principal punto de controversia radica
en la variable tasa de aprobación, variable que guarda una correlación
casi directa con la variable objetivo. Si bien su construcción fue hecha
a partir de los registros históricos no configura una fuga de datos en
el sentido estricto, su inclusión en el conjunto de características
puede estar inflando artificialmente los indicadores de desempeño. Esto
genera un riesgo latente, el modelo podría estar dependiendo en exceso
de estas variables endógenas y perder robustez al desplegarse en un
entorno de producción real. Para proteger la validez externa del
estudio, la literatura reciente \[32\], \[47\] sugiere limitar el
feature engineering a predictores estrictamente exógenos, lo que
permitiría evaluar la verdadera capacidad de generalización del
algoritmo.

Como limitación del estudio, cabe mencionar que la información analizada
corresponde a una sola universidad. Aunque los resultados son
alentadores en este escenario específico, sería poco riguroso desde el
punto de vista metodológico pretender que funcionen igual en otras
instituciones sin antes verificarlo. Cada universidad tiene su propia
dinámica, diferentes formas de organizarse, distintos recursos,
estudiantes con características particulares y maneras diversas de
enseñar. Por eso, no se puede simplemente copiar y pegar el modelo en
otro lado y esperar que funciones. Siguiendo lo que plantean \[11\],lo
razonable es ser muy cuidadoso al momento de generalizar estos
resultados y, más bien, poner a prueba el modelo en otras universidades.
Sólo así sabremos realmente si es robusto y si puede adaptarse a
contextos diferentes del original. De otra manera, hay que se honestos,
el promedio ponderado sirve para tener una idea del rendimiento
académico, pero se queda corto. La universidad es mucho más que sacar
buenas notas. Formarse profesionalmente implica desarrollar habilidades
prácticas, trabajar las competencias socioemocionales, involucrarse en
investigación y prepararse para el mundo laboral. Por esa razón,
coincidiendo con \[52\], sería valioso que próximos estudios agreguen
estas dimensiones en sus modelos. Así tendríamos una visión más completa
y real de lo que viven los estudiantes durante su formación.

Resulta fundamental reconocer las limitaciones propias de este estudio.
Aunque disponer de 833 estudiantes brinda un volumen de datos aceptable,
la categoría de alto rendimiento quedó representada con apenas 63
registros, lo que introduce un desbalance que puede comprometer la
estabilidad de algunas estimaciones. Esta situación resulta
especialmente delicada al trabajar con algoritmos complejos, ya que la
escasez de casos en grupos minoritarios suele debilitar la solidez de
los hallazgos y limitar el alcance de las conclusiones, un riesgo
documentado por \[53\]. Por ello, los resultados obtenidos ofrecen una
perspectiva valiosa sobre el problema, pero exigen una lectura cuidadosa
que contemple tanto la capacidad predictiva del modelo como las
restricciones impuestas por la distribución de la muestra.

Partiendo de los que encontramos, existen varias opciones para seguir
investigando. Sería muy útil probar el modelo en otras universidades
públicas, usar datos a lo largo del tiempo para ver cómo cambia el
desempeño de los alumnos y aplicar métodos de inteligencia artificial
explicable más avanzados. Todo esto ayudaría a mejorar la precisión de
las predicciones y aprovechar mejor la herramienta en la gestión
universitaria, tal y como sugieren \[46\], \[54\] y \[55\]. En resumen,
los datos confirman que XGBoost funciona muy bien para predecir el
rendimiento en Ingeniería de Minas, ya que superó las metas de desempeño
que se propusieron. También comprobamos que el historial académico de
los estudiantes influye mucho más en los resultados que su situación
socioeconómica. Este hallazgo es clave porque nos ayuda a entender mejor
qué factores definen el éxito de un alumno y nos da bases para crear
estrategias de tutoría y acompañamiento mucho más específicas y que
funcionen de manera real.

## **Conclusiones**

En síntesis, el modelo XGBoost logró predecir de manera precisa el
rendimiento académico de los estudiantes de Ingeniería de Minas entre
2020 y 2025, lo que lo convierte en un recurso muy útil para anticipar
resultados y entender a fondo cómo se desenvuelven los alumnos. Al
aplicar una validación cruzada estratificada de cinco pliegues y usar
SMOTE para balancear las clases, el modelo obtuvo un F1-Macro de
0.9270±0.0325 junto con una exactitud de 0.9531±0.0169. cuando probamos
el modelo con un conjunto de prueba independiente de 167 registros que
nunca había visto, la exactitud general llegó hasta 96.41% y el F1-Macro
a 0.9101. Con estos números, el modelo superó el 80% con una gran
diferencia y que fue planteado en la hipótesis general. Estos hallazgos
dejan claro que los algoritmos de aprendizaje supervisado son una opción
muy sólida para predecir el rendimiento en una universidad pública .
Además, nuestros resultados coinciden con lo que encontraron \[33\] y
\[28\], quienes también resaltan que los algoritmos de ensamblaje
funcionan muy bien para predecir el desempeño en carreras de ingeniería.

Los valores SHAP revelaron que las variables vinculadas al historial
académico del estudiante tuvieron el mayor peso al momento de clasificar
su rendimiento. La tasa de aprobación encabezó el ranking de
importancia, seguida en orden por el promedio más bajo alcanzado en
algún semestre, el promedio más alto, el promedio del último periodo
cursado y la cantidad de materias desaprobadas. El ritmo de egreso, por
su parte, ocupó una posición intermedia dentro de este ordenamiento. Al
revisar con más cuidado estos hallazgos, se advierte que los estudiantes
con tasas de aprobación bajas y promedios mínimos reducidos tienden a
ubicarse en la categoría de bajo rendimiento. En cambio, quienes
muestran un ritmo de egreso más acelerado suelen clasificarse dentro del
grupo de alto rendimiento. Este comportamiento confirma algo que los
docentes ya observaban desde hace tiempo. Las calificaciones del último
ciclo no bastan para entender cómo va un estudiante. Lo que realmente
cuenta es el historial completo que ha tenido durante la carrera, con
sus avances, sus equivocaciones y sus momentos difíciles. Esa historia
acumulada dice mucho más sobre el desempeño que cualquier nota tomada de
manera aislada.

Los factores socioeconómicos como el ingreso familiar, el tipo de
colegio de procedencia, la disponibilidad de equipos tecnológicos y las
características de la vivienda mostraron una influencia notablemente
menor frente a las variables académicas. De hecho, estos elementos
ocuparon los últimos lugares en el ranking de importancia que arrojo el
análisis SHAP. Este comportamiento coincide con lo que encontraron
Tarrillo Saldaña \[60\] y López et al. \[61\], quienes demostraron que
el historial académico funciona como un predictor muy sólido del
desempeño estudiantil, con una relevancia relativa cercana al 65%. Los
resultados de este estudio confirman que, en el contexto analizado, la
trayectoria académica previa ofrece señales más confiables para
anticipar el rendimiento que ciertas variables del entorno
socioeconómico. Aunque las condiciones materiales forman parte de la
realidad de los estudiantes y no pueden ignorarse, los datos muestran
que el historial académico tiene mayor capacidad explicativa y
predictiva sobre los resultados educativos. Desde la perspectiva del
modelo, seguir la evolución formativa del estudiante resulta más
revelador que examinar de forma aislada sus circunstancias familiares o
materiales.

Para darle más solidez a los hallazgos, se aplicaron también pruebas
estadísticas inferenciales que permitieron explorar si existían brechas
reales en el desempeño de los estudiantes según su origen educativo. En
concreto, se recurrió a la prueba de Kruskal -- Wallis, una herramienta
no paramétrica ideal cuando los datos no siguen una distribución normal,
con el propósito de contrastar el rendimiento académico entre los
distintos tipos de colegio de procedencia. Al hacer la prueba, se obtuvo
un estadístico H de 6.94 con un p-valor de 0.225, cifra muy por encima
del umbral de significancia de 0.05 que se había fijado de antemano.
Esto quiere decir que no hubo evidencia estadística suficiente para
rechazar la hipótesis nula, es decir, no se pudo demostrar que el tipo
de colegio del que proviene el estudiante marque una diferencia real en
su rendimiento universitario. En términos simples, los datos analizados
no respaldan la idea de que venir de un colegio estatal, particular,
parroquial o militar determine de manera significativa si un estudiante
tendrá mejor o peor desempeño en la carrera. Esta conclusión resulta
relevante porque, aunque en el ámbito social se suele asumir que el
origen educativo pesa mucho en la trayectoria universitaria, los números
de esta muestra apuntan a que otros factores, particularmente los
vinculados al historial académico acumulado durante la carrera, tienen
un peso explicativo mucho mayor.

Al no alcanzar el nivel de significancia estadística, no se encontraron
diferencias significativas entre los estudiantes procedentes de colegios
estatales, particulares, parroquiales, militares, adventistas y
paraestatales. De forma similar, la prueba Chi-cuadrado de independencia
aplicada entre el estado civil de los padres y el nivel de rendimiento
produjo un estadístico χ² = 6.53 y un p-valor de 0.366,lo que permitió
descartar una asociación estadísticamente significativa entre ambas
variables.

Aunque estos resultados pueden parecer, a primera vista, poco
compatibles con algunos antecedentes de la literatura internacional,
adquieren mayor sentido cuando se consideran las características del
contexto estudiado. En una universidad pública peruana y,
específicamente, en la carrera de Ingeniería de Minas, los procesos de
admisión pueden contribuir a cierta homogeneización del perfil académico
inicial de los estudiantes. No significa que las condiciones de origen
carezcan de importancia en términos sociales; significa, más bien, que
en los datos analizados no mostraron suficiente evidencia estadística
para explicar las diferencias observadas en el rendimiento. La matriz de
correlación de Spearman reforzó, por otro lado, la consistencia de las
relaciones entre las variables académicas. La tasa de aprobación
presentó una correlación muy fuerte con el promedio ponderado general (p
= 0.931), mientras que los cursos aprobados mostraron una gran
correlación con los semestres cursados (p = 0.913). estas relaciones
evidenciaron una importante coherencia interna de los datos y
respaldaron la incorporación de variables derivadas mediante ingeniería
de características.

Al comparar los seis algoritmos evaluados, XGBoost presento el mejor
desempeño, con un F1-Macro de 0.9270. le siguieron Gradient Boosting,
con 0.9096; Árbol de Decisión, con 0.8684; Random Forest, con 0.8635;
Regresión Logística, con 0.8020; y, finalmente, Red Neuronal Multicapa,
con 0.7747. La diferencia entre XGBoost y Gradient Boosting fue
relativamente reducida (Δ=0.0174); sin embargo, ambos métodos basados en
boosting superaron de manera consistente a las demás alternativas
evaluadas. Este comportamiento coincide con los resultados descritos por
Sánchez- Sánchez et al.\[32\] y Pan y Dai \[34\], quienes identificaron
a los algoritmos de ensamblaje basados en árboles como alternativas de
alto desempeño para la predicción del rendimiento académico.

Un resultado particularmente interesante fue que la Regresión Logística
superó a la Red Neuronal Multicapa en todas las métricas evaluadas. A
menudo nos dejamos deslumbrar por los algoritmos más elaborados y
olvidamos un principio básico de la ciencia de datos, ya que tener más
capas o parámetros no garantiza que el modelo prediga mejor. En nuestro
caso, la Red Neuronal Multicapa mostró resultados bastante inestables
entre los pliegues de la validación cruzada, con una desviación estándar
de 0.0502 en elF1 -- Macro. Esta fluctuación nos indica que el modelo es
muy sensible a la forma en que se inicializan los pesos y al
desequilibrio de las clases minoritarias en los datos. Al final, los
resultados nos confirman que no hace falta construir una arquitectura
gigante para obtener buenos resultados, pues dependiendo del problema,
un algoritmo más simple y directo puede funcionar mucho mejor.

Aplicar SMOTE únicamente sobre los datos de entrenamiento en cada uno de
los pliegues de la validación cruzada resultó ser una decisión
metodológica acertada para enfrentar el desbalance de las clases. La
distribución original mostraba 516 estudiantes en la categoría Regular,
254 en Bajo y apenas 63 en Alto, lo que obligaba a tomar precauciones
para no sesgar la evaluación. Al restringir el sobre muestreo al
conjunto de entrenamiento de cada partición, los datos de validación
mantuvieron su distribución real y no se contaminaron con instancias
sintéticas. Esta práctica reduce de forma considerable el riesgo de fuga
de información, un problema que suele inflar las métricas de manera
engañosa y dar la falsa impresión de que el modelo generaliza bien
cuando en realidad solo está memorizando patrones artificiales. Los
resultados obtenidos bajo este esquema ofrecen una estimación más
honesta de la capacidad predictiva, en línea con lo que recomiendan Yuan
et al. \[53\] en su revisión sistemática sobre modelos predictivos del
éxito estudiantil.

Cuando se probó el modelo XGBoost con el conjunto de prueba reservado,
los resultados confirmaron su solidez. Para la clase Bajo, que es la más
crítica desde el punto de vista de un sistema de alerta temprana, el
modelo logró un Recall del 98.04%, lo que significa que detectó
correctamente a 50 de los 51 estudiantes en esa categoría y sólo
confundió a uno, clasificándolo como Regular. En la clase Alto alcanzó
una precisión del 100% al acertar las 10 predicciones que le
correspondían, mientras que para la clase Regular la precisión fue del
96.19%. el F1-score de la categoría Alto quedó en 0.8696, una cifra que
conviene leer con cautela porque esa clase apenas estuvo representada
por 13 casos en el conjunto de prueba. Cuando la muestra es tan pequeña,
cualquier error individual tiene un peso desproporcionado sobre las
métricas, de modo que una variación mínima puede cambiar los indicadores
sin que ello refleje un cambio real en el comportamiento del modelo.

Estos hallazgos demuestran que es viable usar el modelo XGBoost para
implementar un sistema de alerta temprana en la universidad, a pesar de
las limitaciones propias de la investigación. Que el algoritmo logre
detectar a tiempo a los alumnos en riesgo es clave para cumplir con el
deber institucional de acompañarlos. Más allá de las métricas y los
datos duros, hay estudiantes reales que necesitan tutoría o apoyo
pedagógico antes de que sus problemas se vuelvan imposibles de resolver.
La verdadera utilidad de estas herramientas radica en poder actuar
pronto, cuando todavía se puede cambiar el rumbo académico de un alumno.
También es importante entender que no todos los errores del modelo pesan
lo mismo. Si el sistema alerta sobre un alumno que en realidad va bien,
sólo hace falta una revisión rápida y no genera un daño real. Pero, si
el modelo falla al no detectar a un alumno que, si está en problemas, se
pierde la oportunidad de ayudarlo a tiempo. Esta diferencia en el costo
de los errores es crucial. Un falso positivo se resuelve fácilmente con
una segunda mirada, mientras que un falso negativo deja que el bajo
rendimiento avance en silencia y se convierta en una situación mucho más
difícil de solucionar después.

Ahí es donde se nota el verdadero aporte de herramientas como XGBoost
dentro de una universidad. Este algoritmo no solo se limita a decir qué
estudiante podría fallar, sino que entrega información útil para que las
autoridades actúen antes de que el problema se agrave, distribuyan mejor
los recursos de tutoría y acompañen de forma más cercana a quienes lo
necesitan. Claro está, el modelo por si solo no soluciona nada. Para que
funciones en la práctica tiene que ir de la mano con decisiones bien
pensadas, un seguimiento constante y acciones concretas sobre el
terreno. Al final, la tecnología educativa vale la pena cuando deja de
ser solo una calculadora y se convierte en una forma real de detectar
necesidades y abrir puertas de apoyo para los estudiantes. Por otro
lado, el uso de valores SHAP permitió abrir la caja negra del modelo y
entender cómo toma sus decisiones, además de ordenar las variables según
su peso real. De todas las características analizadas, la tasa de
aprobación histórica resultó ser la que más influye a la hora de
detectar bajo rendimiento, seguida de cerca por el promedio más bajo y
el promedio más alto que el estudiante tuvo en su trayectoria. Estos
hallazgos tienen mucho valor porque muestran que cada predicción no sale
de la nada, sino que se apoyan en datos académicos concretos que cuentan
la historia real del estudiante. Así, la información que entrega el
modelo va más allá de señalar a alguien en riesgo, ya que también da
pistas sobre qué está pasando detrás de esa situación.

Lo más valioso de este análisis es que no se limita a predecir quien
tendrá problemas académicos. Al combinar XGBoost con SHAP, el modelo no
solo identifica a los estudiantes en riesgo, sino que muestra
exactamente qué variables pesan más en cada predicción. Esto les da un
uso mucho más práctico a los resultados, ya que, en vez de solo alertar
sobre un posible bajo rendimiento, nos indica qué factores académicos
específicos requieren atención inmediata. Entender estas causas es
fundamental para que las instituciones puedan intervenir a tiempo y de
forma efectiva. Nuestros hallazgos a vinculan con lo planteado por Ahmed
et al. \[37\] y Qiang et al. \[38\], quienes resaltan que la
Inteligencia Artificial Explicable es clave para crear modelos
educativos transparentes y fáciles de interpretar a la hora de tomar
decisiones institucionales.

Loa resultados obtenidos indican que este modelo puede servir como un
apoyo importante para la toma de decisiones en el entorno universitario,
siempre que entendamos sus predicciones como señales de alerta temprana
y no como sentencias irrevocables que marquen el destino académico del
alumno. Es fundamental recordar que ningún algoritmo puede abarcar toda
la complejidad del proceso educativo. Detrás de cada dato numérico hay
una personal con una historia de vida única, dificultades específicas y
fortalezas que no siempre quedan reflejadas en las variables
cuantitativas que utilizamos. La ventaja del método SHAP radica en que
nos permite saber exactamente qué factores están influyendo más en los
resultados. Esta transparencia es clave para diseñar estrategias de
apoyo bien dirigidas, como tutorías personalizadas, cursos de refuerzo o
reorientación de la malla curricular. Poner en marcha estas acciones
durante los primeros semestres resulta especialmente conveniente, ya que
ayuda a corregir las dificultades iniciales antes de que se conviertan
en barreras insalvables que pongan en riesgo la continuidad del
estudiante en la universidad. En definitiva, el valor de este modelo no
reside únicamente en su precisión para predecir calificaciones, sino en
su capacidad para brindar a la institución un sistema que anticipe
cuándo un estudiante está en situación de vulnerabilidad. Detectar el
riesgo académico cuando los problemas ya son evidentes suele derivar en
intervenciones tardías y con menor efectividad. Por el contrario, la
anticipación que ofrece el modelo permite a la universidad activar
mecanismos de acompañamiento en el momento adecuado, aumentando las
posibilidades de cambiar el rumbo y mejorar el historial académico del
alumno.

La capacidad predictiva deja de ser solo un cálculo estadístico y se
convierte en una herramienta con sentido humano, porque permite actuar a
tiempo antes de que los problemas académicos se agraven. Al final, lo
que realmente importa de la tecnología educativa no es qué tan bien
acierta un pronóstico, sino que tan útil resulta para tomar decisiones
en el momento justo y cambiar el rumbo de un estudiante que, sin ese
apoyo, posiblemente no terminaría su carrera.

## **Recomendaciones**

Sería muy valioso que las autoridades académicas y el equipo de tutoría
de Ingeniería de Minas integren el modelo XGBoost dentro de un sistema
de alerta temprana en la universidad. La idea es identificar desde el
inicio de cada ciclo a los estudiantes que podrían tener problemas con
sus notas, para darles apoyo antes de que la situación se complique.
Actuar a tiempo marca una gran diferencia en la vida universitaria del
alumno, ya que permite resolver las dificultades cuando apenas están
empezando y evitar que se conviertan en obstáculos imposibles de superar
\[62\].

Esta propuesta tiene mucho sentido por los buenos resultados que arrojó
el algoritmo en las pruebas, sobre todo por alcanzar un 98.04% de
sensibilidad o Recall para la clase de bajo rendimiento. Ese número nos
dice que el modelo es muy bueno para no dejar pasar por alto a los
chicos que realmente están en riesgo. Además, XGBoost se lleva muy bien
con distintos tipos de datos, lo que nos permite mezclar en el análisis
tanto el historial académico como la situación socioeconómica de cada
estudiante para entender mejor que está pasando. Por todo esto, conectar
este modelo con los sistemas de gestión que ya usa la universidad sería
un gran paso, ya que así se podrían generar reportes automáticos y
personalizados mostrando el nivel de riesgo de cada alumno.

Estos reportes servirían como una herramienta útil para los tutores, ya
que ayudarían a distribuir mejor los recursos disponibles y a brindar
acompañamiento pedagógico a los estudiantes que realmente lo necesiten.
Al final, adoptar este tipo de enfoque va más allá de simplemente
predecir quién podría desaprobar. Se convierte en una forma concreta,
basada en datos reales, de diseñar acciones específicas, promover que
los estudiantes se queden en la universidad y asegurar que terminen su
carrera. Por otro lado, conviene que la dirección de Bienestar
Universitario y los responsables de las políticas estudiantiles
aprovechen los resultados del análisis SHAP para orientar las
intervenciones según las particularidades de cada alumno. De este modo,
las decisiones dejarían de basarse en criterios generales y podrían
considerar las variables que más pesan en cada caso. Así sería posible
aplicar estrategias de acompañamiento más precisas y adaptadas a la
realidad de cada estudiante, con el fin de mejorar la retención y el
avance académico. Identificar a tiempo las señales de riesgo marca una
diferencia real cuando se quiere prevenir el bajo rendimiento. En este
estudio, la tasa de aprobación y el promedio mínimo semestral fueron los
factores con mayor peso en las predicciones. Por eso, tendría sentido
priorizar tutorías académicas intensivas para los estudiantes con bajo
rendimiento o con dificultades recurrentes a lo largo de su carrera, de
modo que reciban el apoyo necesario para mejorar su desempeño y avanzar
con más seguridad. Del mismo modo, cuando el riesgo detectado esté
vinculado a condiciones familiares o económicas, habría que complementar
las tutorías con mecanismos de apoyo socioeconómico. Es importante tener
presente que la predicción no debe convertirse en una etiqueta
definitiva sobre el estudiante, sino en una señal que permite actuar a
tiempo.

A los investigadores y docentes de la Maestría en Inteligencia
Artificial y áreas relacionadas les convendría poner a prueba el mismo
protocolo metodológico en otras carreras y universidades públicas del
país. De esa forma se podría ver si los resultados se mantienen cuando
cambia el contexto institucional o la región, y sobre todo comprobar si
el modelo sigue funcionando bien con estudiantes que no formaron parte
del estudio original. Para que la comparación sea justa, hay que
mantener los mismos pasos de integración de datos, construcción de
variables derivadas, balanceo de clases y uso de métrica de evaluación
que no se dejen engañar por el desbalance. Por otro lado, la oficina de
Planificación y Calidad Académica debería revisar cómo se recogen,
organizan y actualizan los datos académicos y socioeconómicos. Durante
el trabajo se notaron vacíos de información y formatos muy distintos
entre registros, lo que deja claro que un buen modelo no depende solo
del algoritmo que se elija, sino de qué tan limpios y completos estén
los datos desde el inicio. Sería útil contar con un repositorio único
donde toda la información esté centralizada y sea fácil de consultar.
Sumado a eso, aplicar rutinas automáticas de validación y hacer
revisiones periódicas de calidad ayudaría a detectar errores a tiempo y
mantener los registros al día. Acumular datos no basta si no son
confiables, coherentes y reflejan lo que realmente pasa en la
institución. Pro eso se propone actualizar las bases de datos cada
semestre, de modo que siempre estén listas para apoyar tanto el análisis
como las decisiones importantes.

También conviene que las próximas investigaciones incluyan variables
psicosociales y conductuales como la autosuficiencia académica, la
motivación, los hábitos de estudio y la participación en actividades
extracurriculares. El rendimiento universitario no depende sólo de las
notas o de los indicadores curriculares acumulados. Hay factores
personales y experiencias del día a día que influyen de manera decisiva
en cómo aprende cada estudiante. Explorar estas dimensiones ayudaría a
entender mejor las brechas de rendimiento y a explicar por que algunos
estudiantes avanzan con naturalidad mientras que otros tropiezan,
incluso cuando partieron con perfiles académicos similares. Para ello
resulta útil aplicar instrumentos ya validados y, siempre que sea
posible, hacer un seguimiento longitudinal que permita ver cómo
evolucionan estos factores a lo largo de la carrera. Así se logra una
mirada más completa y cercana de la realidad estudiantil, capaz de
orientar nuevas investigaciones y de diseñar estrategias de
acompañamiento que respondan a lo que los estudiantes realmente
necesitan.

Al fin y al cabo, el rendimiento académico es mucho más que una cifra o
un conjunto de datos registrados en una base de datos; detrás de cada
resultado hay una experiencia personal, con sus propios desafíos,
esfuerzos y circunstancias.

## **Referencias**

\[1\] «Perú: seguimiento de buenas prácticas del derecho a la educación
superior alrededor del mundo; iniciativas de políticas sobre el derecho
a la educación superior en Perú - UNESCO Biblioteca Digital». Accedido:
9 de octubre de 2026. \[En línea\]. Disponible en:
https://unesdoc.unesco.org/ark:/48223/pf0000385633

\[2\] I. Hilliger *et al.*, «Identifying needs for learning analytics
adoption in Latin American universities: A mixed-methods approach», *The
Internet and Higher Education*, vol. 45, p. 100726, abr. 2020, doi:
10.1016/j.iheduc.2020.100726.

\[3\] «Ministerio de Educación - MINEDU». Accedido: 26 de mayo de 2026.
\[En línea\]. Disponible en: https://www.gob.pe/minedu

\[4\] V. Tinto, *Leaving College: Rethinking the Causes and Cures of
Student Attrition*. University of Chicago Press, 2012. Accedido: 27 de
septiembre de 2026. \[En línea\]. Disponible en:
https://www.perlego.com/book/1851055/leaving-college-rethinking-the-causes-and-cures-of-student-attrition-pdf

\[5\] K. M. Aguilar Lopez, «Predictive modeling based on machine
learning strategies to forecast student dropout at a Peruvian
university: A case study».

\[6\] «Prediction and Explainability of School Dropout in Peru Using
Machine Learning and Explainable Artificial Intelligence \| IEEE
Journals & Magazine \| IEEE Xplore». Accedido: 9 de octubre de 2026.
\[En línea\]. Disponible en:
https://ieeexplore.ieee.org/document/11443270

\[7\] D.-M. Cordova-Esparza *et al.*, «Predicting and Preventing School
Dropout with Business Intelligence: Insights from a Systematic Review»,
*Information*, vol. 16, p. 326, abr. 2025, doi: 10.3390/info16040326.

\[8\] A. González-Nucamendi, J. Noguez, L. Neri, V. Robledo-Rella, y R.
García-Castelán, «Predictive analytics study to determine undergraduate
students at risk of dropout», *Frontiers in Education*, vol. 8, oct.
2023, doi: 10.3389/feduc.2023.1244686.

\[9\] F. J. García-García, M. I. Gómez-Núñez, y C. Molla-Esparza,
«Applications of learning analytics in the study of academic performance
in higher education: A meta-review with an educational perspective»,
*High Educ*, jun. 2026, doi: 10.1007/s10734-026-01709-y.

\[10\] S. Boujmiraz, H. Darhmaoui, y A. Drissi el maliani, «Predicting
student performance: A comprehensive review of machine learning, deep
learning, and explainable AI approaches», *Computers and Education:
Artificial Intelligence*, vol. 10, p. 100548, jun. 2026, doi:
10.1016/j.caeai.2026.100548.

\[11\] M. Yagci, «Educational data mining: prediction of students'
academic performance using machine learning algorithms», *Smart Learning
Environments*, vol. 9, mar. 2022, doi: 10.1186/s40561-022-00192-z.

\[12\] S. Wang y B. Luo, «Academic achievement prediction in higher
education through interpretable modeling», *PLOS ONE*, vol. 19, n.^o^ 9,
p. e0309838, sep. 2024, doi: 10.1371/journal.pone.0309838.

\[13\] K. Alalawi, R. Athauda, y R. Chiong, «Contextualizing the current
state of research on the use of machine learning for student performance
prediction: A systematic literature review», *Engineering Reports*, vol.
5, n.^o^ 12, p. e12699, 2023, doi: 10.1002/eng2.12699.

\[14\] R. realidadeconomica.es, «Gary Becker y la teoría de la economía
del capital humano en la educación y el trabajo \| Realidad Económica».
Accedido: 2 de octubre de 2026. \[En línea\]. Disponible en:
https://www.realidadeconomica.es/gary-becker-y-la-teoria-de-la-economia-del-capital-humano-en-la-educacion-y-el-trabajo/41658

\[15\] B. Yem, T. R. Dash, y B. Harth, «Discussion and analysis of
educational disparities through human capital perspective», *Front.
Educ.*, vol. 11, abr. 2026, doi: 10.3389/feduc.2026.1747554.

\[16\] H. He y E. A. Garcia, «Learning from Imbalanced Data», *IEEE
Trans. on Knowl. and Data Eng.*, vol. 21, n.^o^ 9, pp. 1263-1284, sep.
2009, doi: 10.1109/TKDE.2008.239.

\[17\] S. Raschka, «Machine Learning with PyTorch and Scikit-Learn»,
Sebastian Raschka, PhD. Accedido: 6 de octubre de 2026. \[En línea\].
Disponible en:
https://sebastianraschka.com/books/machine-learning-with-pytorch-and-scikit-learn/

\[18\] S. Lundberg y S.-I. Lee, «A Unified Approach to Interpreting
Model Predictions», 25 de noviembre de 2017, *arXiv*: arXiv:1705.07874.
doi: 10.48550/arXiv.1705.07874.

\[19\] E. Freitas *et al.*, «MMALA: Developing and Evaluating a Maturity
Model for Adopting Learning Analytics», *Journal of Learning Analytics*,
vol. 11, n.^o^ 1, pp. 67-86, mar. 2024, doi: 10.18608/jla.2024.8099.

\[20\] K. M. Aguilar Lopez, Y. Carbajal Ortega, D. G. Martinez Hilario,
y S. A. A. Rodriguez Carrillo, «Predictive modeling based on machine
learning strategies to forecast student dropout at a Peruvian
university: A case study», ago. 2023, Accedido: 28 de mayo de 2026. \[En
línea\]. Disponible en:
https://laccei.org/LACCEI2024-CostaRica/meta/FP1316.html

\[21\] C. L. Kok, C. K. Ho, L. Chen, Y. Y. Koh, y B. Tian, «A Novel
Predictive Modeling for Student Attrition Utilizing Machine Learning and
Sustainable Big Data Analytics», *Applied Sciences*, vol. 14, n.^o^ 21,
p. 9633, ene. 2024, doi: 10.3390/app14219633.

\[22\] H. Sahlaoui, E. A. ABDELLAOUI ALAOUI, A. Nayyar, A. Said, y M.
Jaber, «Predicting and Interpreting Student Performance Using Ensemble
Models and Shapley Additive Explanations», *IEEE Access*, vol. PP, pp.
1-1, oct. 2021, doi: 10.1109/ACCESS.2021.3124270.

\[23\] «2023 Global Education Monitoring Report, Technology in
education: a». Accedido: 6 de octubre de 2026. \[En línea\]. Disponible
en:
https://www.unesco.org/en/articles/2023-global-education-monitoring-report-technology-education-tool-whose-terms

\[24\] I. Hilliger *et al.*, «Identifying needs for learning analytics
adoption in Latin American universities: A mixed-methods approach», *The
Internet and Higher Education*, vol. 45, p. 100726, abr. 2020, doi:
10.1016/j.iheduc.2020.100726.

\[25\] «Predicting student success: a state-of-the-art systematic
review of models and factors \| Journal of Applied Research in Higher
Education \| Emerald Publishing». Accedido: 6 de octubre de 2026. \[En
línea\]. Disponible en:
https://www.emerald.com/jarhe/article-abstract/doi/10.1108/JARHE-08-2025-0674/1342710/Predicting-student-success-a-state-of-the-art?redirectedFrom=fulltext

\[26\] A. Sandeepa y A. Mascrenghe, «Predicting School Students'
Academic Performance Using Ensemble Machine Learning Techniques», en
*2025 Moratuwa Engineering Research Conference (MERCon)*, ago. 2025, pp.
108-113. doi: 10.1109/MERCon67903.2025.11217054.

\[27\] Md. M. Islam, F. H. Sojib, Md. F. H. Mihad, M. Hasan, y M.
Rahman, «The integration of explainable AI in Educational Data Mining
for student academic performance prediction and support system»,
*Telematics and Informatics Reports*, vol. 18, p. 100203, jun. 2025,
doi: 10.1016/j.teler.2025.100203.

\[28\] A. Almalawi, B. Soh, A. Li, y H. Samra, «Predictive Models for
Educational Purposes: A Systematic Review», *Big Data and Cognitive
Computing*, vol. 8, n.^o^ 12, p. 187, dic. 2024, doi:
10.3390/bdcc8120187.

\[29\] «Identifying needs for learning analytics adoption in Latin
American universities: A mixed-methods approach \| Request PDF».
Accedido: 6 de octubre de 2026. \[En línea\]. Disponible en:
https://www.researchgate.net/publication/338728652_Identifying_needs_for_learning_analytics_adoption_in_Latin_American_universities_A_mixed-methods_approach

\[30\] E. V. Díaz, I. Hilliger, C. Gonzalez, S. Celis, M.
Pérez-Sanagustín, y J. Broisin, «The Mediating Role of Learning
Analytics: Insights into Student Approaches to Learning and Academic
Achievement in Latin America», *Journal of Learning Analytics*, vol. 11,
n.^o^ 1, pp. 6-20, mar. 2024, doi: 10.18608/jla.2024.8149.

\[31\] «Factores socioeconómicos y académicos asociados al bajo
rendimiento académico en estudiantes de educación superior \| Revista
Científica Pakamuros». Accedido: 6 de octubre de 2026. \[En línea\].
Disponible en:
https://revistas.unj.edu.pe/index.php/pakamuros/article/view/271

\[32\] A. M. Sánchez-Sánchez, J. D. Mello-Román, M. Segura, y A.
Hernández, «Identifying the Determinants of Academic Success: A Machine
Learning Approach in Spanish Higher Education», *Systems*, vol. 12,
n.^o^ 10, p. 425, oct. 2024, doi: 10.3390/systems12100425.

\[33\] A. Turkmenbayev, E. Abdykerimova, S. Nurgozhayev, G. Karabassova,
y D. Baigozhanova, «The application of machine learning in predicting
student performance in university engineering programs: a rapid review»,
*Front. Educ.*, vol. 10, p. 1562586, sep. 2025, doi:
10.3389/feduc.2025.1562586.

\[34\] S. Pan y W. Dai, «Research on Student Performance Prediction
Based on Random Forest Algorithm», *Proceedings of the 2024
International Symposium on Artificial Intelligence for Education*, 2024,
Accedido: 6 de octubre de 2026. \[En línea\]. Disponible en:
https://www.semanticscholar.org/paper/Research-on-Student-Performance-Prediction-Based-on-Pan-Dai/8ac006a01d580c81cfedb6bfad77899d4ff24bc3

\[35\] M. Pérez-Sanagustín, I. Hilliger, J. Maldonado-Mahauad, y R.
Pérez-Álvarez, «Building Institutional Capacity for Learning Analytics:
Top-Down & Bottom-Up Initiatives», *IEEE Revista Iberoamericana de
Tecnologias del Aprendizaje*, vol. 17, n.^o^ 3, pp. 281-289, ago. 2022,
doi: 10.1109/RITA.2022.3191413.

\[36\] P. D. Long y G. Siemens, «Penetrare la nebbia: tecniche di
analisi per l'apprendimento», *Italian Journal of Educational
Technology*, vol. 22, n.^o^ 3, pp. 132-137, dic. 2014, doi:
10.17471/2499-4324/195.

\[37\] N. U. R. Junejo, M. W. Nawaz, Q. Huang, X. Dong, C. Wang, y G.
Zheng, «Accurate multi-category student performance forecasting at early
stages of online education using neural networks», *Sci Rep*, vol. 15,
p. 16251, may 2025, doi: 10.1038/s41598-025-00256-3.

\[38\] S. I. Kampezidou, A. Tikayat Ray, A. P. Bhat, O. J. Pinon
Fischer, y D. N. Mavris, «Fundamental Components and Principles of
Supervised Machine Learning Workflows with Numerical and Categorical
Data», *Eng*, vol. 5, n.^o^ 1, pp. 384-416, mar. 2024, doi:
10.3390/eng5010021.

\[39\] I. H. Sarker, «Machine Learning: Algorithms, Real-World
Applications and Research Directions», *SN COMPUT. SCI.*, vol. 2, n.^o^
3, p. 160, mar. 2021, doi: 10.1007/s42979-021-00592-x.

\[40\] C. Schröer, F. Kruse, y J. M. Gómez, «A Systematic Literature
Review on Applying CRISP-DM Process Model», *Procedia Computer Science*,
vol. 181, pp. 526-534, ene. 2021, doi: 10.1016/j.procs.2021.01.199.

\[41\] «¿Qué es el machine learning? \| IBM». Accedido: 6 de octubre de
2026. \[En línea\]. Disponible en:
https://www.ibm.com/mx-es/think/topics/machine-learning

\[42\] «CRISP-DM process model application - LeapSpace -
ScienceDirect.com». Accedido: 6 de octubre de 2026. \[En línea\].
Disponible en:
https://www.sciencedirect.com/leapspace/conversation/d9dd949a-5a5e-4d3d-b773-5b8cff4ef100

\[43\] «¿Qué es machine learning? Definición, tipos y ejemplos \| SAP».
Accedido: 6 de octubre de 2026. \[En línea\]. Disponible en:
https://www.sap.com/latinamerica/resources/what-is-machine-learning

\[44\] S. Tripathi, D. Muhr, M. Brunner, H. Jodlbauer, M. Dehmer, y F.
Emmert-Streib, «Ensuring the Robustness and Reliability of Data-Driven
Knowledge Discovery Models in Production and Manufacturing», *Front.
Artif. Intell.*, vol. 4, jun. 2021, doi: 10.3389/frai.2021.576892.

\[45\] C. Schröer, F. Kruse, y J. M. Gómez, «A Systematic Literature
Review on Applying CRISP-DM Process Model», *Procedia Computer Science*,
vol. 181, pp. 526-534, ene. 2021, doi: 10.1016/j.procs.2021.01.199.

\[46\] N. U. R. Junejo, M. W. Nawaz, Q. Huang, X. Dong, C. Wang, y G.
Zheng, «Accurate multi-category student performance forecasting at early
stages of online education using neural networks», *Sci Rep*, vol. 15,
p. 16251, may 2025, doi: 10.1038/s41598-025-00256-3.

\[47\] S. Kapoor y A. Narayanan, «Leakage and the reproducibility crisis
in machine-learning-based science», *Patterns*, vol. 4, n.^o^ 9, sep.
2023, doi: 10.1016/j.patter.2023.100804.

\[48\] «Hernández-Sampieri, R. & Mendoza, C (2018). Metodología de la
investigación. Las rutas cuantitativa, cualitativa y mixta \| RUDICS».
Accedido: 29 de septiembre de 2026. \[En línea\]. Disponible en:
https://virtual.cuautitlan.unam.mx/rudics/?p=2612

\[49\] «Field, A.P. (2018) Discovering Statistics Using IBM SPSS
Statistics. 5th Edition, Sage, Newbury Park. - References - Scientific
Research Publishing». Accedido: 29 de septiembre de 2026. \[En línea\].
Disponible en:
https://www.scirp.org/reference/referencespapers?referenceid=3504991

\[50\] A. P. Merino, *Análisis de datos con SPSS 13 Base*.
McGraw-Hill/Interamericana de España, 2005.

\[51\] «Hair, J. F., Babin, B. J., Anderson, R. E., & Black, W. C.
(2019). Multivariate Data Analysis (8th ed.). Cengage Learning. -
References - Scientific Research Publishing». Accedido: 29 de septiembre
de 2026. \[En línea\]. Disponible en:
https://www.scirp.org/reference/referencespapers?referenceid=3935304

\[52\] V. Realinho, J. Machado, L. Baptista, y M. V. Martins,
«Predicting Student Dropout and Academic Success», *Data*, vol. 7, n.^o^
11, p. 146, nov. 2022, doi: 10.3390/data7110146.

\[53\] A. Shimaoka, R. Cordeiro Ferreira, y A. Goldman, «The Evolution
of CRISP-DM for Data Science: Methods, Processes and Frameworks», vol.
4, pp. 28-43, oct. 2024, doi: 10.5753/reviews.2024.3757.

\[54\] E. Staneviciene, D. Gudoniene, V. Punys, y A. Kukstys, «A Case
Study on the Data Mining-Based Prediction of Students' Performance for
Effective and Sustainable E-Learning», *Sustainability*, vol. 16, n.^o^
23, p. 10442, ene. 2024, doi: 10.3390/su162310442.

\[55\] A. M. Shimaoka, R. C. Ferreira, y A. Goldman, «The evolution of
CRISP-DM for Data Science: Methods, processes and frameworks», *SBC
Reviews on Computer Science*, vol. 4, n.^o^ 1, pp. 28-43, oct. 2024,
doi: 10.5753/reviews.2024.3757.

\[56\] C. Schröer, F. Kruse, y J. Marx Gómez, «A Systematic Literature
Review on Applying CRISP-DM Process Model», *Procedia Computer Science*,
vol. 181, pp. 526-534, ene. 2021, doi: 10.1016/j.procs.2021.01.199.

\[57\] E. López-Meneses, P. C. Mellado-Moreno, C. Gallardo Herrerías, y
N. Pelícano-Piris, «Educational Data Mining and Predictive Modeling in
the Age of Artificial Intelligence: An In-Depth Analysis of Research
Dynamics», *Computers*, vol. 14, n.^o^ 2, p. 68, feb. 2025, doi:
10.3390/computers14020068.

\[58\] Y. Zhang, Y. Yun, R. An, J. Cui, H. Dai, y X. Shang, «Educational
Data Mining Techniques for Student Performance Prediction: Method Review
and Comparison Analysis», *Frontiers in Psychology*, vol. 12, dic. 2021,
doi: 10.3389/fpsyg.2021.698490.

\[59\] S. Kwakye, «Towards Transparent and Interpretable Predictions of
Student Performance Using Explainable AI», jun. 2025, doi:
10.15123/uel.8zx64.

\[60\] A. Al-Ameri, W. Al-Shammari, A. Castiglione, M. Nappi, C. Pero, y
M. Umer, «Student Academic Success Prediction Using Learning Management
Multimedia Data With Convoluted Features and Ensemble Model», *J. Data
and Information Quality*, vol. 17, n.^o^ 3, p. 12:1-12:16, sep. 2025,
doi: 10.1145/3687268.

\[61\] Y. S. Balcioğlu y M. Artar, «Predicting academic performance of
students with machine learning», *Information Development*, vol. 41,
n.^o^ 3, pp. 896-915, sep. 2025, doi: 10.1177/02666669231213023.

\[62\] M. Qiang, Z. Liu, y R. Zhang, «Explainable AI in education:
integrating educational domain knowledge into the deep learning model
for improved student performance prediction», *Sci Rep*, vol. 16, n.^o^
1, p. 9515, feb. 2026, doi: 10.1038/s41598-026-40538-y.

\[63\] O. T. Saldaña, J. M. Huamán, W. M. C. Camacho, y O. H. C.
Cabrera, «Factores socioeconómicos y académicos asociados al bajo
rendimiento académico en estudiantes de educación superior», *Revista
Científica Pakamuros*, vol. 11, n.^o^ 4, pp. 1-15, dic. 2023, doi:
10.37787/pakamuros-unj.unj02355.

\[64\] C. A. T. López, J. V. P. Huaytan, H. E. L. Gómez, J. M. S. Soto,
y J. H. O. Fernández, «Predicción del rendimiento académico mediante
modelos de regresión logística y el análisis discriminante», abr. 2024,
doi: 10.5281/zenodo.11490539.

\[65\] C. Chaka, «Educational data mining, student academic performance
prediction, prediction methods, algorithms and tools: an overview of
reviews», *1*, vol. 18, n.^o^ 2, pp. 58-69, ago. 2022, doi:
10.20368/1971-8829/1135578.

\[66\] I. Kotorov, Y. Krasylnykova, M. Pérez-Sanagustín, F. Mansilla, y
J. Broisin, «Supporting Decision-Making for Promoting Teaching and
Learning Innovation: A Multiple Case Study», *Journal of Learning
Analytics*, vol. 11, n.^o^ 1, pp. 21-36, mar. 2024, doi:
10.18608/jla.2024.8131.

## 

## Anexos

**Anexo 1.** Tabla de operacionalización de variables o tabla de
categorización (según el enfoque de la investigación)

+----------------+------------------+-----------------+-------------------+-----------------------------------------------------------+-----------------+
| **Variable**   | **Definición     | **Definición    | **Dimensiones**   | **Indicadores**                                           | **Escala**      |
|                | conceptual**     | operacional**   |                   |                                                           |                 |
+:==============:+==================+=================+===================+===========================================================+=================+
| Variable       | Conjunto de      | Se evaluará     | Exactitud del     | Accuracy = $\frac{TP + TN}{TP + TN + FP + FN}$            | Razón           |
| Independiente: | algoritmos y     | mediante el     | modelo            |                                                           |                 |
| Machine        | técnicas de      | desempeño de    |                   | Donde:                                                    |                 |
| Learning       | inteligencia     | los algoritmos  |                   |                                                           |                 |
|                | artificial       | de              |                   | TP = Verdaderos Positivos                                 |                 |
|                | implementados    | clasificación   |                   |                                                           |                 |
|                | para procesar    | desarrollados   |                   | TN = Verdaderos Negativos                                 |                 |
|                | datos históricos | para la         |                   |                                                           |                 |
|                | y generar        | predicción del  |                   | FP = Falsos Positivos                                     |                 |
|                | clasificaciones  | rendimiento     |                   |                                                           |                 |
|                | predictivas      | académico,      |                   | FN = Falsos Negativos                                     |                 |
|                | sobre el         | empleando       |                   |                                                           |                 |
|                | desempeño        | métricas de     |                   | (Rainio, Teuho y Klén 2024; Martinović, Dokic y Pudić     |                 |
|                | estudiantil.     | evaluación      |                   | 2025)                                                     |                 |
|                |                  | reconocidas en  |                   |                                                           |                 |
|                |                  | Machine         |                   |                                                           |                 |
|                |                  | Learning.       |                   |                                                           |                 |
|                |                  |                 +-------------------+-----------------------------------------------------------+-----------------+
|                |                  |                 | Precisión del     | Precision =$\frac{TP}{TP + FP}$                           | Razón           |
|                |                  |                 | modelo            |                                                           |                 |
|                |                  |                 |                   | Donde:                                                    |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | TP = Verdaderos Positivos                                 |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | FP = Falsos Positivos                                     |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | (Rainio, Teuho y Klén 2024)                               |                 |
|                |                  |                 +-------------------+-----------------------------------------------------------+-----------------+
|                |                  |                 | Sensibilidad del  | Recall =$\frac{TP}{TP + FN}$                              | Razón           |
|                |                  |                 | modelo            |                                                           |                 |
|                |                  |                 |                   | Donde:                                                    |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | TP = Verdaderos Positivos                                 |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | FN = Falsos Negativos                                     |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | (Rainio, Teuho y Klén 2024)                               |                 |
|                |                  |                 +-------------------+-----------------------------------------------------------+-----------------+
|                |                  |                 | Capacidad         | F1-Score =2x$\frac{Precision*Recall}{Precision + Recall}$ | Razón           |
|                |                  |                 | predictiva        |                                                           |                 |
|                |                  |                 |                   | Donde:                                                    |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | Precision = Precisión del modelo                          |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | Recall = Sensibilidad del modelo                          |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | (Rainio, Teuho y Klén 2024)                               |                 |
|                |                  |                 +-------------------+-----------------------------------------------------------+-----------------+
|                |                  |                 | Capacidad         | ROC-AUC = Área bajo la curva ROC                          | Razón           |
|                |                  |                 | discriminativa    |                                                           |                 |
|                |                  |                 |                   | Donde:                                                    |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | ROC = Receiver Operating Characteristic                   |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | AUC = Area Under the Curve                                |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | Valores entre 0.5 (aleatorio) y 1.0 (perfecto)            |                 |
|                |                  |                 |                   |                                                           |                 |
|                |                  |                 |                   | (Fawcett 2006)                                            |                 |
|                |                  |                 +-------------------+-----------------------------------------------------------+-----------------+
|                |                  |                 | Interpretabilidad | Valores SHAP                                              | S               |
+----------------+------------------+-----------------+-------------------+-----------------------------------------------------------+-----------------+
| Variable       | Grado de logro   | Se medirá a     | Desempeño         | Promedio ponderado acumulado (escala 0-20)                | Razón           |
| Dependiente:   | alcanzado por el | través de       | académico         |                                                           | (Promedio,      |
| Rendimiento    | estudiante de    | indicadores     |                   | N° de cursos desaprobados(conteo)                         | Créditos)       |
| académico      | Ingeniería de    | académicos      |                   |                                                           |                 |
|                | Minas respecto a | institucionales |                   | \% de créditos aprobados                                  |                 |
|                | los objetivos    | que reflejen el |                   | =$\frac{Créditos\ aprobados}{Créditos\ matriculados}x100$ |                 |
|                | educativos       | desempeño y     |                   |                                                           |                 |
|                | institucionales, | progreso del    |                   |                                                           |                 |
|                | el cual será     | estudiante,     |                   |                                                           |                 |
|                | clasificado por  | clasificándolo  |                   |                                                           |                 |
|                | el modelo para   | en categorías   |                   |                                                           |                 |
|                | identificar el   | de rendimiento  |                   |                                                           |                 |
|                | riesgo de bajo   | según umbrales  |                   |                                                           |                 |
|                | rendimiento.     | establecidos.   |                   |                                                           |                 |
|                |                  |                 +-------------------+-----------------------------------------------------------+-----------------+
|                |                  |                 | Progreso          | Estado académico: Matricula regular/irregular             | Nominal         |
|                |                  |                 | académico         |                                                           | (Estado)        |
|                |                  |                 |                   | Clasificación del rendimiento:                            |                 |
|                |                  |                 |                   | Satisfactorio/Insatisfactorio                             | Clasificación   |
|                |                  |                 |                   |                                                           | binaria: 0=Bajo |
|                |                  |                 |                   | Codificación binaria:                                     | rendimiento,    |
|                |                  |                 |                   |                                                           | 1=Satisfactorio |
|                |                  |                 |                   | 0=Bajo rendimiento, 1=Satisfactorio                       |                 |
+----------------+------------------+-----------------+-------------------+-----------------------------------------------------------+-----------------+

: []{#_Toc242806487 .anchor}Tabla 15. Tabla de operacionalización de
variables

+------------------+--------------------+---------------------+-----------------------------------------+---------------------------+
| **PROBLEMA       | **OBJETIVO         | **HIPOTESIS         | **VARIABLES/DIMENSIONES**               | **METODOLOGIA**           |
| GENERAL**        | GENERAL**          | GENERAL**           |                                         |                           |
+:=================+====================+=====================+=========================================+===========================+
| ¿Cuál es la      | Accuracy/F1-score) | Los modelos de      | Variable Independiente:                 | Tipo: Aplicada            |
| capacidad        | superior al 80% en | Machine Learning    |                                         |                           |
| predictiva de    | la predicción del  | alcanzarán una      | Algoritmos de Machine Learning          | Enfoque: Cuantitativo     |
| los Modelos de   | rendimiento        | precisión           | Dimensiones e indicadores:              |                           |
| Machine Learning | académico de los   | (Accuracy/F1-Score) |                                         | Nivel:                    |
| sobre el         | estudiantes de     | superior al 80% en  | • Exactitud del modelo                  | Predictivo/Explicativo    |
| rendimiento      | Ingeniería de      | la predicción del   |                                         |                           |
| académico de los | Minas durante el   | rendimiento         | → Accuracy = (TP+TN)/(TP+TN+FP+FN)      | Diseño: No experimental,  |
| estudiantes de   | periodo 2020-2025, | académico de los    |                                         | longitudinal              |
| Ingeniería de    | mediante la        | estudiantes de      | • Precisión del modelo                  | retrospectivo             |
| Minas durante el | combinación de     | Ingeniería de Minas |                                         |                           |
| periodo          | variables          | durante el periodo  | → Precision = TP/(TP+FP)                | Población y muestra:      |
| 2020-2025?       | académicas,        | 2020-2025, mediante |                                         |                           |
|                  | personales y       | la combinación de   | • Sensibilidad del modelo               | P:\~840 registros         |
|                  | socioeconómicas.   | variables           |                                         | académicos de estudiantes |
|                  |                    | académicas,         | → Recall = TP/(TP+FN)                   | de Ingeniería de Minas    |
|                  |                    | personales y        |                                         | matriculados en una       |
|                  |                    | socioeconómicas.    | • Capacidad predictiva                  | universidad nacional      |
|                  |                    |                     |                                         | peruana (2020-2025)       |
|                  |                    |                     | → F1-Score =                            | M:\~833 registros válidos |
|                  |                    |                     | 2×(Precision×Recall)/(Precision+Recall) | (Tras fusión y            |
|                  |                    |                     |                                         | depuración), divididos en |
|                  |                    |                     | • Capacidad discriminativa              | registros 666 registros   |
|                  |                    |                     |                                         | para entrenamiento y 167  |
|                  |                    |                     | → ROC-AUC                               | validación/prueba.(80/20) |
|                  |                    |                     |                                         | Técnicas: Análisis        |
|                  |                    |                     | • Interpretabilidad                     | documental sistemático de |
|                  |                    |                     |                                         | registros institucionales |
|                  |                    |                     | → Valores SHAP                          | y Minería de Datos.       |
|                  |                    |                     |                                         |                           |
|                  |                    |                     | Variable Dependiente: Rendimiento       | Instrumentos: Ficha de    |
|                  |                    |                     | Académico Dimensiones:                  | extracción datos          |
|                  |                    |                     |                                         | estandarizada (Validación |
|                  |                    |                     | • Desempeño académico                   | por juicio de expertos).  |
|                  |                    |                     |                                         |                           |
|                  |                    |                     | → Promedio ponderado acumulado (0-20),  | Método de análisis de     |
|                  |                    |                     | N° de cursos desaprobados, % de         | datos: -Estadística       |
|                  |                    |                     | créditos aprobados. • Progreso          | descriptiva e inferencial |
|                  |                    |                     | académico                               | (Kruskal-Wallis,          |
|                  |                    |                     |                                         | Chi-cuadrado).            |
|                  |                    |                     | → Estado de matrícula, clasificación    | -Validación cruzada       |
|                  |                    |                     | binaria (0=Bajo rendimiento,            | k-fold (k 0 5).           |
|                  |                    |                     | 1=Satisfactorio)                        |                           |
|                  |                    |                     |                                         | Evaluación:               |
|                  |                    |                     |                                         |                           |
|                  |                    |                     |                                         | \- Matriz de confusión,   |
|                  |                    |                     |                                         | métricas multiclase(      |
|                  |                    |                     |                                         | Accuracy,F1-Macro, curva  |
|                  |                    |                     |                                         | ROC-AUC).                 |
|                  |                    |                     |                                         |                           |
|                  |                    |                     |                                         | Interpretabilidad:        |
|                  |                    |                     |                                         |                           |
|                  |                    |                     |                                         | \- SHAP(Shapley Additive  |
|                  |                    |                     |                                         | Explanations) para XAI    |
|                  |                    |                     |                                         | (Inteligencia Artificial  |
|                  |                    |                     |                                         | Explicable).              |
|                  |                    |                     |                                         | -Herramientas:Python      |
|                  |                    |                     |                                         | 3.x,pandas, Scikit-learn, |
|                  |                    |                     |                                         | XGBoost, SHAP             |
|                  |                    |                     |                                         |                           |
|                  |                    |                     |                                         |                           |
|                  |                    |                     |                                         |                           |
|                  |                    |                     |                                         |                           |
+------------------+--------------------+---------------------+                                         |                           |
| **PROBLEMAS      | **OBJETIVOS        | **HIPÓTESIS         |                                         |                           |
| ESPECÍFICOS**    | ESPECÍFICOS**      | ESPECÍFICAS**       |                                         |                           |
+------------------+--------------------+---------------------+                                         |                           |
| 1\. ¿Cuál es la  | 1\. Identificar la | 1\. Las variables   |                                         |                           |
| importancia      | importancia de las | académicas          |                                         |                           |
| relativa de las  | variables          | (promedio           |                                         |                           |
| variables        | predictoras        | ponderado, tasa de  |                                         |                           |
| predictoras      | (académicas,       | aprobación, cursos  |                                         |                           |
| (académicas,     | personales y       | desaprobados)       |                                         |                           |
| personales y     | socioeconómicas)   | presentarán una     |                                         |                           |
| socioeconómicas) | en la capacidad    | mayor importancia   |                                         |                           |
| en la capacidad  | predictiva de los  | relativa en la      |                                         |                           |
| predictiva de    | modelos de Machine | capacidad           |                                         |                           |
| los modelos de   | Learning para la   | predictiva de los   |                                         |                           |
| Machine Learning | clasificación del  | modelos de Machine  |                                         |                           |
| para la          | rendimiento        | Learning,           |                                         |                           |
| clasificación    | académico.         | explicando          |                                         |                           |
| del rendimiento  |                    | aproximadamente el  |                                         |                           |
| académico?       |                    | 65% de la varianza  |                                         |                           |
|                  |                    | del rendimiento, en |                                         |                           |
|                  |                    | comparación con las |                                         |                           |
|                  |                    | variables           |                                         |                           |
|                  |                    | personales y        |                                         |                           |
|                  |                    | socioeconómicas.    |                                         |                           |
+------------------+--------------------+---------------------+                                         |                           |
| 2\. ¿Cuál es el  | 2\. Crear y        | 2\. Los modelos de  |                                         |                           |
| desempeño        | entrenar modelos   | ensamblaje (Random  |                                         |                           |
| predictivo de    | predictivos de     | Forest y XGBoost)   |                                         |                           |
| los modelos de   | aprendizaje        | obtendrán un        |                                         |                           |
| Regresión        | automático         | desempeño           |                                         |                           |
| Logística,       | utilizando         | predictivo          |                                         |                           |
| Árboles de       | técnicas de        | significativamente  |                                         |                           |
| Decisión, Random | Regresión          | superior (F1-Score  |                                         |                           |
| Forest, ¿XGBoost | Logística, Árboles | \> 0.90) en         |                                         |                           |
| y Redes          | de Decisión,       | comparación con los |                                         |                           |
| Neuronales       | Random Forest,     | modelos lineales    |                                         |                           |
| Artificiales al  | XGBoost y Redes    | (Regresión          |                                         |                           |
| ser entrenados   | Neuronales         | Logística) y de     |                                         |                           |
| con datos        | Artificiales.      | árbol simple (Árbol |                                         |                           |
| históricos de    |                    | de Decisión), al    |                                         |                           |
| estudiantes de   |                    | ser entrenados con  |                                         |                           |
| Ingeniería de    |                    | el dataset          |                                         |                           |
| Minas?           |                    | histórico de        |                                         |                           |
|                  |                    | estudiantes.        |                                         |                           |
+------------------+--------------------+---------------------+                                         |                           |
| 3\. ¿Existen     | 3\. Evaluar y      | 3\. Existirán       |                                         |                           |
| diferencias      | comparar la        | diferencias         |                                         |                           |
| significativas   | eficacia de los    | estadísticamente    |                                         |                           |
| en la eficacia   | modelos de         | significativas (p   |                                         |                           |
| predictiva       | predicción         | \< 0.05) en el      |                                         |                           |
| (Accuracy,       | utilizando         | desempeño           |                                         |                           |
| Precision,       | métricas como la   | predictivo entre    |                                         |                           |
| Recall, F1-Score | exactitud, la      | los distintos       |                                         |                           |
| y ROC-AUC) entre | precisión, la      | algoritmos de       |                                         |                           |
| los distintos    | recuperación       | Machine Learning    |                                         |                           |
| algoritmos de    | (recall), el       | evaluados, siendo   |                                         |                           |
| Machine Learning | índice F1 y el     | XGBoost y Random    |                                         |                           |
| evaluados?       | área bajo la curva | Forest los que      |                                         |                           |
|                  | ROC.               | presenten los       |                                         |                           |
|                  |                    | mayores valores de  |                                         |                           |
|                  |                    | F1-Score y ROC-AUC. |                                         |                           |
+------------------+--------------------+---------------------+                                         |                           |
| 4\. ¿De qué      | 4\. Determinar el  | 4\. La aplicación   |                                         |                           |
| manera la        | mejor modelo con   | de SHAP permitirá   |                                         |                           |
| aplicación de    | mayor capacidad    | identificar de      |                                         |                           |
| técnicas de      | predictiva y       | manera válida e     |                                         |                           |
| Inteligencia     | aplicar técnicas   | interpretable que   |                                         |                           |
| Artificial       | de Explainable AI  | la Tasa de          |                                         |                           |
| Explicable       | (SHAP) para        | Aprobación, el      |                                         |                           |
| (SHAP) permite   | identificar las    | Promedio Ponderado  |                                         |                           |
| identificar e    | variables con      | General y el número |                                         |                           |
| interpretar las  | mayor influencia   | de Cursos           |                                         |                           |
| variables que    | en las             | Desaprobados son    |                                         |                           |
| más influyen en  | predicciones.      | las variables con   |                                         |                           |
| la predicción    |                    | mayor impacto       |                                         |                           |
| del rendimiento  |                    | (valores SHAP       |                                         |                           |
| académico?       |                    | absolutos más       |                                         |                           |
|                  |                    | altos) en la        |                                         |                           |
|                  |                    | predicción del      |                                         |                           |
|                  |                    | rendimiento         |                                         |                           |
|                  |                    | académico,          |                                         |                           |
|                  |                    | facilitando la toma |                                         |                           |
|                  |                    | de decisiones       |                                         |                           |
|                  |                    | institucionales.    |                                         |                           |
+------------------+--------------------+---------------------+-----------------------------------------+---------------------------+

: []{#_Toc242806488 .anchor}Tabla 16. Matriz de Consistencia

**Anexo 2.** Instrumentos de recolección de datos

**Anexo 3.** Ficha de validación de contenido para un instrumento

![](media/image12.png){width="6.017658573928259in"
height="8.198611111111111in"}

![](media/image13.png){width="6.100528215223097in"
height="8.509070428696413in"}

![](media/image14.png){width="6.268055555555556in"
height="8.284127296587927in"}

![](media/image15.emf)

![](media/image16.png){width="6.190277777777778in"
height="8.25542104111986in"}

![](media/image17.png){width="6.178472222222222in"
height="8.129133858267716in"}

![](media/image18.png){width="6.220138888888889in"
height="8.230655074365703in"}

![](media/image19.emf)

![](media/image20.png){width="6.017361111111111in"
height="8.266574803149606in"}

![](media/image21.png){width="5.963888888888889in"
height="8.456574803149607in"}

![](media/image22.png){width="6.267361111111111in"
height="8.154761592300963in"}

![](media/image23.emf)

**Anexo 4.** Consentimiento Informado (según corresponda).

**Anexo 5.** Asentimiento informado (según corresponda).

**Anexo 6.** Solicitud de autorización para realizar la investigación en
una institución (de corresponder).

**Anexo 7.** Autorización de uso de información de una institución (de
corresponder).

![](media/image24.png){width="5.600485564304462in"
height="6.725582895888014in"}
![](media/image25.png){width="5.767166447944007in"
height="6.517230971128609in"}

![](media/image26.png){width="5.18378280839895in"
height="7.2089577865266845in"}![](media/image27.emf)

![](media/image28.png){width="5.808836395450569in"
height="8.16737423447069in"}

![](media/image29.emf)

![](media/image30.png){width="5.625487751531058in"
height="7.709001531058617in"}![](media/image31.png){width="5.933847331583552in"
height="8.16737423447069in"}![](media/image32.png){width="5.962121609798775in"
height="8.293257874015747in"}

![](media/image33.png){width="5.925513998250219in"
height="8.084034339457569in"}![](media/image34.png){width="5.833838582677165in"
height="8.142372047244095in"}![](media/image35.png){width="5.850507436570429in"
height="8.142372047244095in"}![](media/image36.png){width="6.00051946631671in"
height="8.225713035870516in"}

**Anexo 8.** Resultados del análisis de consistencia interna (de
corresponder)

**Anexo 9.** Reporte de similitud del software Turnitin

**Anexo 10.** Análisis complementario. Donde se incluirá el cálculo de
tamaño de muestra u otros cálculos requeridos para la investigación.

Evidencia 1: Captura de la base de datos en Microsoft Excel mostrando
las 20 primeras filas y todas las columnas de variable académicas, con
encabezados claramente identificados.

Evidencia 2: Captura del script de Python (MiTesisUCV2026)utilizado para
la fusión de datasets, limpieza, imputación y generación de variables
derivadas.

Evidencia 3: Archivo MINAS_FUSIONADO_COMPLETO.csv con los 3,784
registros consolidados.
![](media/image37.png){width="6.604166666666667in"
height="3.720138888888889in"}

Evidencia 4: Archivo MINAS_LIMPIO_IMPUTADO_RIGUROSO.csv con el dataset
final depurado y listo para análisis.
![](media/image38.png){width="6.604166666666667in"
height="3.910416666666667in"}

Evidencia 5: Gráfico de distribución del promedio ponderado
general(figura_01_distribucion_promedio.png)![](media/image3.png){width="6.604166666666667in"
height="3.8159722222222223in"}

Evidencia 6: Boxplot promedio ponderado según el tipo de
ingreso(figura_02_boxplot_ingresovs_promedio.png)![](media/image4.png){width="6.604166666666667in"
height="3.8819444444444446in"}

Evidencia 7: Violin plot de rendimiento según tipo de colegio
(figura_03_violin_colegio_vs_promedio.png)![](media/image5.png){width="6.604166666666667in"
height="4.590277777777778in"}

Evidencia 8: Mapa de calor de correlaciones (figura
04_heatmap_correlación.png)![](media/image6.png){width="6.604166666666667in"
height="6.253472222222222in"}

Evidencia 9: Matriz de confusión del modelo
XGBoost(figura_05_matriz_confusion_multiclase.png)![](media/image39.png){width="6.604166666666667in"
height="5.209722222222222in"}

Evidencia 10: grafico SHAP de importancia de variables
(figura_08_shap_impotance_bar.png)

![](media/image40.png){width="6.604166666666667in"
height="7.352083333333334in"}

Evidencia 11: Tablas de resultados estadísticos en formato CSV
(tabla_01_estadistica_descriptiva.csv,
tabla_05_resultados_validacion_cruzada.csv).

![](media/image41.png){width="6.604166666666667in"
height="3.9243055555555557in"}

**Anexo 11.** Otras evidencias, donde se incluirán fotografías, planos,
documentos o cualquier otro que ayude a esclarecer más la investigación.

**Nota:**

Les recordamos la importancia de elaborar el trabajo de investigación
con la mayor rigurosidad posible. Para ello, les recomendamos revisar la
**Guía de Trabajos Conducentes a Grados y Títulos**, donde encontrarán
las pautas necesarias para completar los capítulos indicados en el
esquema de su informe.

¡Mucho éxito en su elaboración!

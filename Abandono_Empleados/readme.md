# Análisis de Rotación de Empleados (Employee Attrition)
## Descripción del Proyecto

Este proyecto analiza los factores asociados a la rotación de empleados en una empresa, utilizando un conjunto de datos con información detallada de 1.470 empleados. El objetivo es identificar patrones y características que influyen en la probabilidad de que un empleado deje la empresa, permitiendo diseñar estrategias de retención de talento.

## Objetivo del Modelo Predictivo

El objetivo es desarrollar un modelo que prediga la probabilidad de abandono de los empleados, ayudando a:

* Identificar factores críticos de rotación.
* Anticipar riesgos de abandono en distintos roles o grupos de empleados.
* Implementar medidas proactivas para mejorar la retención de talento.

## Descripción de los Datos
* **Total de registros:** 1.470 empleados.
* **Variables numéricas:** 26, incluyendo edad, ingreso mensual, años en la empresa, número de empresas anteriores, etc.
* **Variables categóricas:** 9, incluyendo género, estado civil, puesto de trabajo, departamento, nivel educativo, etc.
* **Datos faltantes:** Ninguno.

## Análisis Exploratorio
### Distribución de Variables Numéricas

* Histogramas y diagramas de caja para observar la distribución, dispersión y valores atípicos.
* Boxplots de MonthlyIncome por Gender y JobRole para identificar diferencias salariales.

## Correlación

* Matriz de correlación para identificar relaciones entre variables numéricas y su influencia potencial en la rotación.

## Rotación de Empleados

* Por Edad: Mayor rotación en empleados jóvenes (25-35 años).
* Por Puesto de Trabajo: Alta rotación en Laboratory Technician y Sales Representative; baja en Manager y Research Director.
* Por Estado Civil: Empleados solteros muestran mayor probabilidad de abandonar.
* Por Nivel Educativo: Mayor rotación en niveles intermedios (2 y 3).
* Por Distancia desde Casa: Empleados que viven más lejos tienen mayor propensión a rotar.
* Por Ingreso Mensual: Distribuciones similares entre géneros; medianas más altas en roles directivos.

## Preprocesamiento

* Transformación de variables categóricas con One-Hot Encoding.
* Escalado de variables numéricas con MinMaxScaler.
* Eliminación de variables no informativas: EmployeeNumber, EmployeeCount, StandardHours, Over18.
* Transformación de variables binarias (Attrition, OverTime) a 0 y 1.

## Visualizaciones Clave

* Histogramas de variables numéricas.
* Countplots para Age, JobRole, MaritalStatus y Education en función de Attrition.
* KDE plots de DistanceFromHome según rotación.
* Boxplots de MonthlyIncome por Gender y JobRole.
* Heatmap de correlación entre variables numéricas.

## Conclusiones

* La rotación es más frecuente en empleados jóvenes, solteros y en ciertos roles específicos.
* Factores como distancia desde el hogar y nivel educativo intermedio están asociados a mayor abandono.
* Puestos directivos y estratégicos presentan mayor estabilidad.
* Los insights permiten diseñar políticas de retención proactivas y dirigidas a los grupos de mayor riesgo.

## Próximos Pasos
* Entrenamiento de modelos predictivos (Regresión Logística, Random Forest, XGBoost) para estimar la probabilidad de rotación.
* Evaluación de modelos con métricas como Accuracy, F1-Score y AUC.
* Creación de dashboards para monitoreo continuo de rotación y estrategias de retención.

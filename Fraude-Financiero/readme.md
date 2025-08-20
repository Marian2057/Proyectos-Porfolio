# 💳 Análisis de Transacciones Financieras y Detección de Fraude  

Este proyecto explora y analiza un conjunto de datos de **transacciones financieras**, aplicando técnicas de exploración de datos, análisis descriptivo, reducción de dimensionalidad y modelado predictivo para la detección de fraude.  

---

## 📂 Exploración de Datos  

- Se cargó y examinó el dataset, identificando **datos duplicados y valores nulos**.  
- El conjunto de datos contiene principalmente **variables numéricas** y una **columna de fechas**.  
- Se realizaron **resúmenes estadísticos** para comprender la distribución de los datos.  

---

## 📊 Análisis Descriptivo  

- Se evaluaron las **variables numéricas**, observando alta variabilidad en los montos de transacción.  
- La **tasa de fraude es baja**, solo 0.89% de las transacciones fueron marcadas como fraudulentas.  
- Se compararon transacciones legítimas y fraudulentas, observando **diferencias significativas en montos y escenarios de fraude**.  

---

## 🔗 Correlación entre Variables  

- Se evaluaron relaciones entre variables, incluyendo:  
  - Correlaciones **temporales**.  
  - Correlaciones **positivas entre características asociadas al fraude**.  
  - Correlaciones entre **actividad del cliente** y del **terminal**.  

---

## 🧩 Análisis de Componentes Principales (PCA)  

- Se aplicó **PCA** para reducir la dimensionalidad del conjunto de datos numéricos.  
- Se logró conservar al menos **95% de la varianza original**, facilitando la visualización y modelado.  

---

## ⏱️ Variables de Fecha y Hora  

- Se extrajeron características a partir de la columna `TX_DATETIME`:  
  - Año, mes, día  
  - Hora y minuto  
- Esto permitió capturar **patrones temporales** en las transacciones.  

---

## 🤖 Modelado Predictivo  

- Se utilizó **RandomForestClassifier** para predecir transacciones fraudulentas.  
- El modelo mostró **rendimiento sólido**, con buena capacidad de detección.  
- Las **variables más importantes** para la predicción fueron:  
  - `TX_FRAUD_SCENARIO`  
  - `TERMINAL_ID_RISK_7DAY_WINDOW`  
  - `TX_AMOUNT`  

---

## 🚀 Conclusiones  

- El análisis permite una visión integral de las transacciones financieras y sus riesgos de fraude.  
- Las técnicas aplicadas (EDA, PCA, extracción de features temporales y Random Forest) **facilitan la identificación de transacciones sospechosas**.  
- Este enfoque puede ser útil para **prevención de fraude** y **toma de decisiones en servicios financieros**.  

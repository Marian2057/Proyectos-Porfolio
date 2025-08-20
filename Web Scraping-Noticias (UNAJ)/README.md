




<img width="1029" height="283" alt="image" src="https://github.com/user-attachments/assets/a1d0cdbe-6735-4160-a4fc-01edb2672157" />


# 📰 Trabajo Práctico Final – Captura de la Información  
**Diplomatura de Vinculación – Introducción a la Ciencia de Datos**  
**Universidad Nacional Arturo Jauretche**  
 
---

## 📌 Introducción  
Este proyecto tiene como objetivo realizar **scraping de noticias políticas** desde el portal [Infobae](https://www.infobae.com/politica/).  
El trabajo permite **obtener, procesar y analizar** información textual proveniente de medios digitales, aplicando técnicas de **Procesamiento de Lenguaje Natural (NLP)** y visualización de datos.  

---

## ⚙️ Librerías utilizadas  
- `requests` → Solicitudes HTTP.  
- `BeautifulSoup (bs4)` → Parseo e interpretación de HTML.  
- `pandas` → Manipulación y análisis de datos.  
- `datetime` → Manejo de fechas.  
- `spacy` → Tokenización, lematización y entidades.  
- `nltk` → Procesamiento de texto adicional.  
- `wordcloud` → Nube de palabras.  
- `matplotlib` → Visualización de gráficos.  
- `collections.Counter` → Conteo de frecuencias.  
- `re` → Expresiones regulares para limpieza.  

---

## 🔎 Desarrollo  

### 1. Extracción de datos  
- Se realizó un **scraping** en la sección **Política** del diario Infobae.  
- Se obtuvieron:  
  - **Títulos de noticias**  
  - **Primer párrafo o resumen**  
- Los datos se organizaron en un **DataFrame de Pandas** con columnas:  
  - `parrafo`  
  - `titulo`  
  - `cant_palabras` (conteo de palabras)  

---

### 2. Almacenamiento de noticias  
Las primeras **10 noticias** se almacenaron en un archivo de texto plano:  

Ultimas_noticias_de_Politica.txt

Cada registro incluye el **título** y el **párrafo** asociado.  

---

### 3. Procesamiento del texto  
- Aplicación de **tokenización y lematización** con `spaCy`.  
- Extracción de **entidades nombradas** (personas, organizaciones, lugares).  
- Construcción de un **corpus lematizado** para análisis textual.  

---

### 4. Visualización – WordCloud  
- Se eliminaron **stopwords** y caracteres no deseados.  
- Se calcularon las **frecuencias de palabras relevantes**.  
- Se generó una **nube de palabras** que refleja los conceptos predominantes en las noticias políticas.  

Ejemplo:  

<img width="979" height="493" alt="image" src="https://github.com/user-attachments/assets/7a63062d-fe6b-4cf4-87f5-a028d6673d50" />


---

## 📊 Resultados obtenidos  
- Extracción y almacenamiento de **10 noticias políticas recientes**.  
- Cálculo de la **cantidad de palabras por párrafo**.  
- Identificación de **términos clave y entidades** (ejemplo: *Javier Milei, Casa Rosada, DNU*).  
- Visualización de un **WordCloud** con las palabras más frecuentes.  

---

## 🚀 Conclusiones  
El proyecto permitió:  
✔️ Implementar un flujo completo de **captura, procesamiento y análisis de texto**.  
✔️ Aplicar técnicas de **Web Scraping, NLP y Visualización de Datos**.  
✔️ Detectar patrones en el discurso político reciente en medios digitales.  

---

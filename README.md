# 🧠 Kolb's Learning Styles Clustering

Este proyecto aplica técnicas de análisis estadístico y agrupamiento para explorar y visualizar estilos de aprendizaje según el modelo de Kolb a partir de datos académicos.

---

## 🎯 Objetivo

Agrupar estudiantes de acuerdo con sus puntajes GPA en distintas dimensiones del modelo de aprendizaje de Kolb, con el fin de:

- Analizar la distribución de estilos (Divergente, Convergente, Asimilador, Acomodador).
- Generar visualizaciones para facilitar la interpretación educativa.
- Explorar correlaciones entre estilos y rendimiento académico.

---

## 📂 Datos utilizados

- Archivo: `Data_Kolb_2.xlsx`
- Variables clave:
  - `GPA_CE` – Experiencia concreta
  - `GPA_LC` – Observación reflexiva
  - `GPA_RC` – Conceptualización abstracta
  - `GPA_CC` – Experimentación activa
  - `GPA_T` – Promedio general
  - `KOLB` – Estilo de aprendizaje original (etiquetado)

---

## ⚙️ Tecnologías y Librerías

- Python (Colab)
- Pandas, Numpy
- Scikit-learn (KMeans, escalado, codificación)
- Matplotlib, Seaborn (visualización)
- RobustScaler y StandardScaler (normalización)

---

## 🔬 Metodología

1. **Carga y limpieza de datos**
   - Eliminación de columnas no relevantes (`ID`)
   - Transformación de etiquetas `KOLB` con codificación `LabelEncoder` y `OneHotEncoder`.

2. **Escalado de variables**
   - Se aplica `StandardScaler` y `RobustScaler` para manejar la varianza y los outliers.

3. **Análisis de correlación**
   - Generación de matriz de correlación para interpretar las relaciones entre dimensiones y estilos.

4. **Clustering**
   - Se prueba el mejor número de clusters con el método del codo (*Elbow Method*).
   - Se aplica `KMeans` con 4 clusters.
   - Se interpretan las medias de cada grupo resultante.

5. **Visualización**
   - `Heatmaps` para correlaciones.
   - `Clustermap` de Seaborn para identificar patrones por grupo.

---

## 📈 Resultados esperados

- Agrupación efectiva de estudiantes según patrones similares de aprendizaje.
- Posibilidad de relacionar estilos de Kolb con el rendimiento académico general.
- Visualizaciones claras para apoyar decisiones pedagógicas.

---

## 🖼️ Ejemplo de salida

![Cluster Heatmap](img/kolb_clusters.png)

*Visualización promedio por grupo (cluster). Cada grupo representa un estilo dominante.*

---



## 📘 Referencias

- Kolb, D. A. (1984). *Experiential learning: Experience as the source of learning and development.*
- Modelo de estilos de aprendizaje de Kolb (Divergente, Asimilador, Convergente, Acomodador)

---

## 👨‍💻 Autor

**Jorge Ruiz Escorcia**  
📍 Barranquilla, Colombia  
📧 jorgeruizescorcia@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/jorge-ruiz-escorcia/)  
🔗 [GitHub](https://github.com/JorgeRuizEscorcia)

---

## 📄 Licencia

Este proyecto es de uso académico y educativo. Puedes reutilizar y modificar el código con fines investigativos o de enseñanza.

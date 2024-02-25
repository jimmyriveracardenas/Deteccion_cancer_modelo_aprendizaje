
# Proyecto de Detección de Cáncer de Mama
## Alumno: Jimmy Rivera
## Modelo y aprendizaje

Este proyecto tiene como objetivo desarrollar un modelo predictivo capaz de identificar la presencia de cáncer de mama con alta precisión, basándose en características extraídas de imágenes digitalizadas de biopsias de mama. Dada la importancia crítica de diagnosticar correctamente el cáncer de mama, se ha puesto especial énfasis en minimizar los falsos negativos, sin descuidar la necesidad de reducir también los falsos positivos.

## Acciones para el modelo

### Preprocesamiento de Datos
    Carga los datos, convierte los diagnósticos en variables binarias, y divide los datos en conjuntos de entrenamiento y prueba.
### Normalización
    Escala las características para tener una media de 0 y una varianza de 1.
### Entrenamiento y Evaluación de Modelos
    Entrena los modelos de Regresión Logística, Random Forest, y Gradient Boosting Classifier con el conjunto de entrenamiento balanceado y evalúa su rendimiento en el conjunto de prueba. Calcula y muestra la precisión, la tasa de error, la matriz de confusión y el reporte de clasificación para cada modelo.


## Justificación de los Modelos

### 1. Regresión Logística

- **Justificación:** La Regresión Logística es un modelo lineal simple que sirve como un excelente punto de partida debido a su interpretabilidad y eficiencia. A pesar de su simplicidad, puede ser muy efectiva en problemas de clasificación binaria cuando las variables predictoras tienen una relación lineal con el logit de la probabilidad de la clase objetivo.

### 2. Random Forest

- **Justificación:** Random Forest es un modelo basado en ensamblaje que utiliza múltiples árboles de decisión para mejorar la precisión y controlar el sobreajuste. Es particularmente útil para manejar conjuntos de datos de alta dimensionalidad y complejidad, como es común en el diagnóstico médico, donde múltiples características pueden influir en la clasificación.

### 3. Gradient Boosting Classifier

- **Justificación:** Gradient Boosting construye secuencialmente árboles de decisión, cada uno corrigiendo los errores del árbol anterior, lo cual lo hace potente para mejorar progresivamente el rendimiento en conjuntos de datos complejos. Este enfoque es valioso cuando se busca un modelo altamente preciso capaz de manejar las sutilezas de los datos de biopsias de mama.

## Evaluación de los Modelos

Cada modelo fue evaluado basándose en su precisión y tasa de error para abordar el desbalance de clases en el conjunto de datos. Los resultados obtenidos son los siguientes:

- **Regresión Logística:**
  - Tasa de Precisión: 97.37%
  - Tasa de Error: 2.63%
  
- **Random Forest:**
  - Tasa de Precisión: 96.49%
  - Tasa de Error: 3.51%
  
- **Gradient Boosting Classifier:**
  - Tasa de Precisión: 95.61%
  - Tasa de Error: 4.39%

### Conclusión

La Regresión Logística demostró ser el modelo más efectivo para este conjunto de datos, logrando la mayor precisión. Este resultado enfatiza la importancia de considerar no solo la complejidad del modelo sino también su adecuación a la naturaleza específica de los datos y el problema. La elección del modelo más adecuado debe basarse en una evaluación cuidadosa de su rendimiento, con especial atención a las métricas críticas para el contexto de aplicación, como la precisión y la tasa de error en el diagnóstico del cáncer de mama.

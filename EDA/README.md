# Análisis Exploratorio de Datos (EDA)

Este repositorio contiene el código y la documentación asociada con el Análisis Exploratorio de Datos (EDA) realizado en un conjunto de datos específico. El objetivo de este README es proporcionar una visión general del EDA realizado y los hallazgos clave.

## Preguntas Abordadas a través del EDA

### 1. Valores Faltantes y Patrones de Ausencia

- **¿Hay valores faltantes en el conjunto de datos? ¿Se pueden identificar patrones de ausencia?**
  
  Análisis de valores faltantes y patrones de ausencia en el conjunto de datos
Se identificaron valores faltantes en el conjunto de datos, específicamente en tres columnas de la tabla Downtime. Cada una de estas columnas presentaba 104.000 registros nulos, lo que representa una cantidad significativa de información faltante.
Se pudo identificar un patrón de ausencia: las tres columnas con valores faltantes no son relevantes para el análisis del área de ensamble, que es el enfoque principal del estudio. Debido a esto, se decidió eliminar estas columnas para evitar sesgos en el análisis y mejorar la precisión del modelo de predicción del uptime.
Es importante destacar que la eliminación de estas columnas no debería afectar significativamente la calidad del conjunto de datos, ya que las variables eliminadas no son esenciales para el análisis del área de ensamble.
Además del análisis de valores faltantes, también se realizó un análisis de frecuencia de valores en la columna Asset ID. Se encontró un top 10 de activos con gran frecuencia de información, los cuales serán utilizados para obtener un análisis de uptime más confiable. Se determinó que los activos relacionados con las líneas de ensamble son 8 equipos.
En resumen, se identificaron y eliminaron valores faltantes en tres columnas de la tabla Downtime que no eran relevantes para el análisis del área de ensamble. Se realizó un análisis de frecuencia de valores en la columna Asset ID y se identificaron los 8 equipos de las líneas de ensamble que serán utilizados para el análisis de uptime.
Estos análisis previos garantizan la calidad y confiabilidad del conjunto de datos que se utilizará para la construcción del modelo de predicción del uptime.

  ![Patrones de Ausencia](https://github.com/JulioQuintanaGarcia/ProyectoIntegradorE30/blob/main/images/DSta.png)

### 2. Estadísticas Resumidas del Conjunto de Datos

- **¿Cuáles son las estadísticas resumidas del conjunto de datos?**
  
  El DataFrame de downtime consta de 68,340 registros, todos relacionados con el AssetID 47. Las fechas de inicio y finalización de los periodos de inactividad oscilan desde el 2 de noviembre de 2021 hasta el 2 de mayo de 2024.
El tiempo medio de duración de los periodos de inactividad es de aproximadamente 279.58 segundos, con una desviación estándar de 8,766.96 segundos. La duración mínima registrada es de -32.04 segundos, lo que puede deberse a errores en los datos o registros incorrectos.
La fecha y hora de inicio y finalización de los periodos de inactividad tienen una distribución uniforme a lo largo de los días del mes y los meses del año, sin evidencia de patrones específicos.
Se puede observar que la variable categórica "Reason" no se incluye en este resumen ya que no tiene un resumen estadístico como las variables numéricas.

  ![Estadistica Descriptiva](https://github.com/JulioQuintanaGarcia/ProyectoIntegradorE30/blob/main/images/DSta.png)

### 3. Valores Atípicos

- **¿Hay valores atípicos en el conjunto de datos? Si es así, ¿se realizó una gráfica de cajas para visualizar dichos valores?**
  
  [Descripción de valores atípicos y visualización.]

  ![Valores Atípicos](ruta/a/imagen.png)

### 4. Cardinalidad de las Variables Categóricas

- **¿Cuál es la cardinalidad de las variables categóricas?**
  
  [Describir la cardinalidad de la variable categórica "Reason".]

### 5. Distribuciones Sesgadas y Transformaciones No Lineales

- **¿Existen distribuciones sesgadas en el conjunto de datos? ¿Es necesaria alguna transformación no lineal?**
  
  [Discusión sobre distribuciones sesgadas y transformaciones.]

### 6. Identificación de Tendencias Temporales

- **¿Se identifican tendencias temporales en el conjunto de datos?**
  
  [Descripción de tendencias temporales identificadas.]

### 7. Correlación entre Variables

- **¿Hay correlación entre las variables dependientes e independientes?**
  
  [Resultados de la correlación entre variables.]

### 8. Distribución de Datos en Función de Categorías

- **¿Cómo se distribuyen los datos en función de diferentes categorías?**
  
  [Descripción de la distribución de datos por categorías.]

### 9. Patrones o Agrupaciones (Clusters) en los Datos

- **¿Existen patrones o agrupaciones (clusters) en los datos con características similares?**
  
  [Discusión sobre patrones o clusters identificados.]

### 10. Normalización de Imágenes

- **¿Se deberían normalizar las imágenes para visualizarlas mejor?**
  
  [Recomendación sobre la normalización de imágenes.]

### 11. Desbalance en las Clases de la Variable Objetivo

- **¿Hay desbalance en las clases de la variable objetivo?**
  
  [Descripción de desbalance en las clases de la variable objetivo.]

## Contribuciones y Contacto

Si tienes alguna pregunta o sugerencia sobre el análisis realizado o el código asociado, no dudes en contactar al equipo a través de [correo electrónico](mailto:ejemplo@correo.com).

¡Gracias por tu interés en nuestro análisis exploratorio de datos!

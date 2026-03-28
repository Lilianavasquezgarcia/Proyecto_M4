El proyecto ABP 4 busca aplicar técnicas de análisis exploratorio de datos (EDA) y el modelado estadístico realizado sobre un conjunto de datos reales de flujos de CO2  (105 observaciones procesadas). El objetivo principal fue determinar el impacto de tres tratamientos experimentales (RC - Control, GT y UE) y diversas variables climáticas sobre el Flujo Total, con el fin de obtener hallazgos relevantes que permitan comprender el comportamiento de los flujos por tratamiento y sustentar decisiones estratégicas.

El proyecto se estructura en 6 partes que se detallan a continuación:

PARTE 1: Análisis exploratorio de datos. Se procede a agregar los datos con los que se va a trabajar, se renombra variables y se define su tipo. Se imputa los valores nulos y faltantes y se actualiza la base de datos ya limpia.
PARTE 2: Estadística descriptiva. Se calcula métricas descriptivas para los datos (Fig. 1) y se explora la estructura a través de gráficas como histogramas y boxplot. Se trata los valores outliers y se genera nuevos boxplots sin outliers (Ver anexos 1, 2 y 3).
 
Fig. 1: Estadística descriptiva

PARTE 3: Correlaciones. Se carga los datos limpios y se procede a generar correlaciones entre variables usando el método de Pearson, generando un heatmap con el valor de “r”. También se generan matrices de dispersión para identificar la distribución de los datos (Ver anexos 4 y 5).
PARTE 4: Regresiones lineales. Se genera modelos retrogresión usando statmodels. Además, se genera predicciones y se calcula la eficiencia del modelo a través de métricas (Fig. 2). Finalmente se desarrolla un gráfico para la visualización del modelo de regresión (Anexo 6).
 
Fig. 2: Métricas del modelo

PARTE 5: Análisis visual de datos. Se crean gráficos con el fin de visualizar múltiples variables y su comportamiento por cada tratamiento. Se crea un pairplot, violín plot, joinplot y facegrid con curvas y densidad de datos (Anexos del 7 al 10).

PARTE 6: Informe usando la librería MATPLOTLIB. Se crea un informe con elementos visuales que facilita la interpretación de los datos. (Anexo 11).


RESULTADOS

Los resultados obtenidos del análisis de los flujos de CO₂ muestran que el tratamiento UE y la temperatura ambiente ejercen un efecto real y significativo en el aumento del flujo total. Tanto los análisis visuales como el modelo de regresión confirman que, a medida que la temperatura ambiente aumenta, también lo hace el flujo, y que el tratamiento UE supera de manera consistente al control, mientras que el tratamiento GT no presenta incrementos estadísticamente significativos. Finalmente, se observó que el modelo final está respaldado por métricas robustas y ofrece estimaciones confiables que permiten identificar las variables que verdaderamente influyen en la respuesta del sistema.

INSIGHTS Y RECOMENDACIONES

Aplicar un preprocesamiento riguroso y utilizar datos depurados en los modelos estadísticos permite identificar de manera adecuada las variables que actúan como predictores realmente significativos del flujo de CO₂. La eliminación de outliers y la corrección de la multicolinealidad fueron pasos esenciales para garantizar un modelo estable y confiable, mientras que el EDA confirmó visualmente las tendencias detectadas. Se recomienda mantener procesos estrictos de limpieza, imputación y validación de datos en futuros análisis, así como priorizar la eficiencia del modelo incorporando únicamente aquellas variables con aporte estadístico comprobado, respaldadas por la información proveniente de la matriz de correlaciones. 

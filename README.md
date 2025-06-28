# Precificación Inmobiliaria

**Objetivo**: Estimar los precios de los inmuebles utilizando técnicas de regresión.

El objetivo principal de este proyecto es construir y evaluar modelos para predecir el precio de venta de propiedades, identificando los factores más influyentes en la precificación.

## Contenido del Notebook

El notebook `precificacion_inmobiliaria.ipynb` contiene los siguientes pasos:

1.  **Ajustando una recta**: Exploración inicial de los datos y ajuste de un modelo de regresión lineal simple utilizando el área del primer piso como única variable predictora.
    -   Lectura y exploración inicial de los datos (`precios_casas.csv`).
    -   Análisis de correlación entre variables.
    -   Visualización de la relación entre el área del primer piso y el precio de venta.
    -   Ajuste de un modelo de regresión lineal simple (OLS) utilizando `statsmodels`.

2.  **Explicando la recta**: Análisis y interpretación del primer modelo de regresión.
    -   Distribución de la variable objetivo (`precio_de_venta`).
    -   Separación de los datos en conjuntos de entrenamiento y prueba.
    -   Ajuste del modelo de regresión simple en el conjunto de entrenamiento.
    -   Análisis de los coeficientes del modelo.
    -   Evaluación de la explicabilidad del modelo (R²).
    -   Análisis de los residuos del modelo.

3.  **Añadiendo otras características**: Incorporación de múltiples variables predictoras al modelo.
    -   Análisis de la relación entre diferentes variables predictoras y el precio de venta utilizando `pairplot`.
    -   Construcción de modelos de regresión múltiple con diferentes combinaciones de variables.
    -   Comparación del desempeño (R²) de los diferentes modelos.

4.  **Precificando las casas**: Utilización del mejor modelo para predecir precios en datos de prueba y nuevos inmuebles.
    -   Evaluación del R² del modelo en el conjunto de prueba.
    -   Predicción del precio para un inmueble individual.
    -   Predicción del precio para un conjunto de nuevos inmuebles (`nuevas_casas.csv`).

5.  **Investigando el modelo**: Análisis de supuestos y problemas del modelo de regresión.
    -   Análisis de multicolinearidad utilizando el Factor de Inflación de Varianza (VIF).
    -   Análisis de los residuos para evaluar supuestos como la homocedasticidad.

## Requisitos

Para ejecutar este notebook, necesitas tener instaladas las siguientes bibliotecas de Python:

-   pandas
-   matplotlib
-   seaborn
-   plotly
-   scikit-learn
-   statsmodels

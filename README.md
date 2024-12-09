# Análisis de Preferencia de Espectadores y Factores de Éxito Comercial de Películas

## Descripción del Proyecto

Este proyecto tiene como objetivo analizar las preferencias de los espectadores y los factores que determinan el éxito comercial de las películas. Utilizando técnicas de Deep Learning, se desarrolló un modelo predictivo para identificar patrones no triviales en los datos y apoyar la toma de decisiones en la industria cinematográfica.

## Integrantes

- Carlos Andrés Pérez Guzmán (carlosperez1694@gmail.com)
- Adad Flores (adadft@gmail.com)
- Nadir Rodriguez (rodriguez1991mn@gmail.com)
- Ivan Castillo Fernandez (ivancastillofer@hotmail.com)

## Tabla de Contenido

1. [Introducción](#introducción)
2. [Importación de librerias necesarias](#importación-de-librerias-necesarias)
3. [Limpieza de Datos](#limpieza-de-datos)
4. [Preprocesamiento de Datos e Ingeniería de Características](#preprocesamiento-de-datos-e-ingeniería-de-características)
5. [Análisis Exploratorio de Datos](#análisis-exploratorio-de-datos)
6. [Preparación de Datos para el Modelo](#preparación-de-datos-para-el-modelo)
7. [Sistema de Recomendación](#sistema-de-recomendación)
8. [Conclusiones](#conclusiones)

## Introducción

En la industria cinematográfica, predecir qué películas resonarán con las audiencias y tendrán éxito comercial es un desafío constante. Este proyecto busca integrar y analizar múltiples fuentes de datos utilizando técnicas avanzadas de Deep Learning para predecir el éxito comercial de las películas y comprender mejor las preferencias de los espectadores.

## Configuración e Instalación

### Requisitos Previos

Este proyecto requiere que Anaconda esté instalado en la computadora. Para más detalles sobre la instalación, visite: [Anaconda Installation](https://docs.anaconda.com/anaconda/install/index.html)

### Cómo Ejecutar

1. Abra su aplicación Terminal favorita (Unix, Linux o MacOS), como Terminal, Comando, Consola, iTerm2, etc.
2. Clone el repositorio:

    ```sh
    git clone https://github.com/Grupo-A-Regression-and-Regularization/proyecto-final.git
    ```

3. Navegue al directorio del proyecto:

    ```sh
    cd proyecto-final
    ```

4. Cree y active el entorno virtual:

    ```sh
    conda create --name movie_analysis python=3.8
    conda activate movie_analysis
    ```

5. Instale las dependencias:

    ```sh
    pip install -r requirements.txt
    ```

6. Ejecute el Jupyter Notebook:

    ```sh
    jupyter notebook Proyecto_Final.ipynb
    ```

## Entendimiento de los Datos

El dataset utilizado contiene información sobre diversas películas, incluyendo su título, género, duración, críticas, likes en Facebook, número de usuarios que votaron, ingresos brutos, puntuación en IMDb, presupuesto y likes en Facebook de la película.

## Manipulación y Limpieza de Datos

1. **Lectura de datos:** Se lee el archivo CSV que contiene los metadatos de las películas.
2. **Selección de columnas relevantes:** Se conservan solo las columnas esenciales para el modelo de recomendación.
3. **Limpieza de datos:** Se eliminan las filas con valores perdidos en las columnas esenciales.

## Análisis de Datos

1. **Distribución de Películas por Género:** Se analiza la distribución de las películas basadas en su género.
2. **Ingresos por Género:** Se analiza la suma de ingresos por género de las películas.
3. **Distribución de Puntuación de IMDb:** Se analiza la distribución de las puntuaciones de IMDb.
4. **Mapa de Correlación entre las Variables Seleccionadas:** Se visualiza la matriz de correlación entre las variables numéricas.
5. **Presupuesto y Ganancias:** Se analiza la relación entre el presupuesto y las ganancias de las películas.
6. **Mejores Puntajes IMDb:** Se muestra el Top 30 de películas con mejores puntajes IMDb.

## Preparación de Datos y Modelado

1. **Preprocesamiento de Datos:** Se normalizan las columnas numéricas utilizando `StandardScaler`.
2. **Separación de Datos:** Se dividen los datos en conjuntos de entrenamiento y prueba.
3. **Construcción del Modelo:** Se construye un modelo de red neuronal utilizando Keras.

## Construcción del Modelo

Se construye y entrena un modelo de red neuronal para predecir los puntajes de IMDb de las películas. El modelo se evalúa utilizando métricas como el error absoluto medio (MAE) y la pérdida (loss).

## Conclusiones y Observaciones

El análisis realizado proporciona una visión detallada de los factores que influyen en el éxito comercial de las películas. Las técnicas de Deep Learning utilizadas permiten identificar patrones no triviales en los datos, mejorando la precisión y efectividad de los sistemas de recomendación y predicción en la industria cinematográfica.

---

Este README proporciona una visión general del proyecto y guía sobre cómo configurarlo y ejecutarlo. Para más detalles, consulte el Jupyter Notebook `Proyecto_Final.ipynb`.
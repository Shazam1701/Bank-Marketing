# Bank Marketing: Análisis exploratorio y regresión logística

## Descripción

El proyecto utiliza el conjunto de datos **Bank Marketing**, que contiene información de campañas de marketing directo de una institución bancaria portuguesa. El objetivo es explorar los datos, prepararlos y construir un modelo de clasificación que estime si un cliente se suscribió a un depósito a plazo fijo.

## Objetivos

- Explorar y visualizar las variables del conjunto de datos.
- Identificar y tratar valores desconocidos y categorías de baja frecuencia.
- Realizar limpieza e ingeniería de variables.
- Analizar relaciones entre variables y multicolinealidad.
- Aplicar análisis de componentes principales (PCA) para resumir variables socioeconómicas correlacionadas.
- Construir una tabla analítica de datos y entrenar un modelo de regresión logística.
- Evaluar el desempeño del modelo mediante métricas de clasificación y la curva ROC.

## Datos

El análisis utiliza `bank-additional-full.csv`, con 41,188 registros y 20 variables en la versión original.

Fuente: [UCI Machine Learning Repository — Bank Marketing](https://archive.ics.uci.edu/dataset/222/bank+marketing).

Descarga el archivo `bank-additional-full.csv` desde la fuente y colócalo en la misma carpeta que el notebook antes de ejecutarlo. El conjunto de datos tiene sus propias condiciones de uso; consulta la página de la fuente.

## Herramientas y técnicas

- Python
- pandas y NumPy
- Matplotlib y Seaborn
- scikit-learn
- Análisis exploratorio de datos (EDA)
- Limpieza y transformación de variables
- Imputación por moda de categorías desconocidas seleccionadas
- Análisis de correlación y PCA
- Regresión logística con ponderación de clases
- Evaluación mediante reporte de clasificación, matriz de confusión y ROC-AUC

## Resultado

En la ejecución documentada en el notebook, el modelo de regresión logística obtuvo un **ROC-AUC de 0.78**. Este valor indica capacidad para distinguir entre las dos clases mejor que una referencia aleatoria, aunque no implica por sí solo que el modelo esté listo para utilizarse en producción.

El notebook también documenta las decisiones de preparación de datos y las limitaciones encontradas durante el análisis.

## Cómo ejecutar el proyecto

1. Descarga o clona este repositorio.
2. Descarga `bank-additional-full.csv` desde la fuente indicada y guárdalo junto al notebook.
3. Abre el notebook en Jupyter Notebook, JupyterLab o Google Colab.
4. Ejecuta las celdas en orden.

### Dependencias principales

Instala las bibliotecas utilizadas con:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn cufflinks
```

El notebook puede requerir otras bibliotecas según las importaciones incluidas en él y el entorno utilizado.

## Dashboard

[Consultar el dashboard en Looker Studio](https://lookerstudio.google.com/reporting/a3f6496c-bfa7-49a3-bf8a-0cea92b42d06)

## Nota

Este proyecto tiene fines educativos y de portafolio. El resultado depende de las decisiones de preparación de datos, las variables incluidas y la partición utilizada. El ROC-AUC reportado corresponde a la ejecución documentada en el notebook.

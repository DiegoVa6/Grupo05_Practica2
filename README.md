# Grupo05_Practica2

Práctica 2 de Aprendizaje Automático: determinación de tipos de estrellas mediante técnicas de aprendizaje no supervisado.

## Descripción

El objetivo de esta práctica es agrupar estrellas a partir de sus características físicas y espectrales. Para ello se trabaja con un dataset de estrellas que incluye variables numéricas y categóricas, y se aplican diferentes técnicas de clustering.

El análisis incluye:

- Análisis exploratorio de datos.
- Limpieza y codificación ordinal de variables categóricas.
- Estandarización de variables.
- Reducción de dimensionalidad mediante PCA a 2 componentes.
- Comparación de K-Means, clustering jerárquico y DBSCAN.
- Selección de un pipeline recomendado.
- Caracterización de los clusters obtenidos.

## Estructura del proyecto

```text
Grupo05_Practica2/
│
├── data/
│   └── stars_data.csv
│
├── practica2_estrellas.ipynb
├── requirements.txt
├── README.md
└── .gitignore
````

## Dataset

El dataset utilizado se encuentra en:

```text
data/stars_data.csv
```

Contiene información sobre estrellas descritas mediante las siguientes variables:

* `Temperature`: temperatura superficial de la estrella.
* `L`: luminosidad relativa respecto al Sol.
* `R`: radio relativo respecto al Sol.
* `A_M`: magnitud absoluta.
* `Color`: color principal del espectro.
* `Spectral_Class`: clase espectral.

## Instalación

Se recomienda crear y activar un entorno virtual antes de instalar las dependencias.

En Windows PowerShell:

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

En Linux/macOS bash:
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Ejecución

Una vez instaladas las dependencias, abrir y ejecutar el notebook:

```text
practica2_estrellas.ipynb
```

En VS Code o Jupyter Notebook, seleccionar el kernel correspondiente al entorno virtual `venv` y ejecutar todas las celdas.

## Pipeline recomendado

Tras comparar los modelos, el pipeline recomendado es:

1. Limpieza de la variable `Color`.
2. Codificación ordinal de `Color` y `Spectral_Class`.
3. Estandarización de las variables.
4. Reducción de dimensionalidad mediante PCA a 2 componentes.
5. Aplicación de K-Means con `k = 6`.

## Dependencias principales

Las principales librerías utilizadas son:

* `numpy`
* `pandas`
* `matplotlib`
* `seaborn`
* `scikit-learn`
* `scipy`
* `hdbscan`
* `jupyter`

## Autores

Grupo 05, Diego Valladares Ortega & Juan Luis del Valle.

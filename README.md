# Análisis Estadístico y Tratamiento de Datos  
## Trabajo práctico

Este repositorio contiene varios cuadernos de Jupyter Notebook desarrollados como parte de un trabajo práctico de análisis de datos. En ellos se abordan tanto **distribuciones estadísticas y tests de análisis** como un **estudio aplicado de datos reales de viento** del aeropuerto de Gran Canaria.

El objetivo principal es mostrar el uso de herramientas estadísticas en Python, combinando **explicaciones teóricas**, **análisis exploratorio** y **representaciones gráficas**, de forma que los propios notebooks sirvan también como memoria del trabajo.

---

## Contenido del repositorio

### 1. `Aplicaciones_de_Distribuciones_y_Test_de_análisis_Santiago_Santana_Martínez.ipynb`

Este cuaderno está dedicado al estudio y aplicación de **distribuciones estadísticas** y **tests de análisis de datos** mediante ejemplos sencillos y didácticos.

Incluye:
- Ejercicios con distribuciones discretas: Bernoulli, Binomial y Poisson.
- Ejercicios con distribuciones continuas: Normal y Exponencial.
- Un ejemplo de correlación lineal y cálculo del coeficiente de Pearson.
- Aplicación de distintos tests estadísticos:
  - Q-Q plot  
  - Shapiro-Wilk  
  - Kolmogórov-Smirnov  
  - Bartlett  
  - Grubbs (detección de valores atípicos)  
  - Wilcoxon  

Cada apartado contiene un **enunciado**, una **explicación del método** y la **resolución en Python**, con el objetivo de ilustrar el uso práctico de cada técnica.

---

### 2. `Actividad_Tratamiento_de_datos_de_viento.ipynb`

Este cuaderno desarrolla un **estudio estadístico descriptivo de datos reales de viento** correspondientes al aeropuerto de Gran Canaria para el mes asignado.

El análisis incluye:
- Visualización inicial de los datos en bruto para identificar su estructura y patrones.
- Cálculo de estadísticos básicos: media, desviación estándar, valores máximo y mínimo.
- Representación gráfica de la velocidad del viento:
  - Día a día (media diaria).
  - Hora a hora para un día representativo.
- Histograma de las velocidades del viento.
- Ajuste de la velocidad del viento a una **distribución de Weibull**, obteniendo los parámetros `k` y `c`.
- Estudio de la dirección del viento:
  - Dirección predominante.
  - Histograma de direcciones.
  - Rosa de los vientos (diagrama polar).

Este notebook sigue una metodología de análisis exploratorio, priorizando la interpretación de los datos antes de aplicar modelos estadísticos.

---

## Creación del entorno de trabajo

Para garantizar la correcta ejecución de los notebooks, se recomienda utilizar un **entorno virtual conda**.  
La forma más sencilla de hacerlo es mediante **Anaconda**, que incluye Python, conda y Jupyter de forma integrada.

### Recomendación: instalar Anaconda

Se recomienda instalar **Anaconda** desde su página oficial:

https://www.anaconda.com/products/distribution

Anaconda facilita la gestión de entornos y dependencias.

---

### Dependencias principales

El entorno incluye, entre otras, las siguientes librerías:

- `numpy`
- `pandas`
- `scipy`
- `matplotlib`
- `seaborn`
- `statsmodels`
- `xlrd` (lectura de ficheros .xls)
- `windrose` (rosa de los vientos)

Estas librerías permiten realizar cálculos estadísticos, visualizaciones y el tratamiento de datos meteorológicos empleados en los notebooks.

### Creación del entorno conda

El repositorio incluye un archivo `environment.yaml` con todas las dependencias necesarias.

Para crear el entorno:

```bash
conda env create -f environment.yaml
```

Para activar el entorno en anaconda se puede usar el comando:

```bash
conda activate MID_trabajo_bloque_3
```

Para activarlo en el entorno de programación, suponiendo que se usa Visual Studio Code:
1. En la esquina superior derecha hay un botón que ponde `Select Kernel`, hacer clic en este botón.
2. Seleccionar la opción `Python Environments` en el desplegable que se acaba de abrir.
3. Buscar el nombre del entorno que se quiere activar y seleccionarlo.

---

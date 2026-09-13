# sprint7-final-project
# Proyecto ConnectaTel: Análisis de Datos
##  Objetivo del proyecto
El objetivo de este proyecto es realizar un análisis exploratorio de los datos de clientes de ConnectaTel para identificar problemas de calidad, analizar el comportamiento de los usuarios y encontrar patrones relacionados con la edad, los planes contratados y el nivel de uso de los servicios de llamadas y mensajes.
A partir de los resultados obtenidos se generan conclusiones y recomendaciones que pueden apoyar la toma de decisiones de la empresa.

##  Datasets utilizados

Para el análisis se utilizaron los siguientes datasets:
* **`users_latam.csv`**: contiene información de los usuarios, como identificador, edad, ciudad, plan, fecha de registro y fecha de cancelación.
* **`usage.csv`**: contiene información sobre el uso de los servicios, incluyendo llamadas y mensajes, duración de llamadas y longitud de mensajes.
* **`plans.csv`**: contiene las características de los planes ofrecidos por ConnectaTel, como precio mensual, cantidad de minutos, mensajes y datos incluidos.

## Etapas del análisis
El proyecto se desarrolló siguiendo las siguientes etapas:

1. **Exploración inicial**
   * Carga de los datasets.
   * Revisión de filas, columnas y tipos de datos.
   * Análisis de valores únicos y estadísticas descriptivas.
2. **Limpieza y preparación**
   * Identificación y tratamiento de valores faltantes.
   * Detección de valores inválidos y valores utilizados como indicadores de datos desconocidos.
   * Revisión y corrección de fechas inconsistentes.
   * Identificación de registros inconsistentes según el tipo de servicio.
   * Conversión y preparación de variables para el análisis.
3. **Análisis exploratorio**
   * Análisis de la distribución de edades.
   * Comparación de usuarios según el plan contratado.
   * Análisis del consumo de llamadas y mensajes.
   * Elaboración de histogramas y diagramas de caja.
4. **Agregación y segmentación**
   * Agrupación de los datos de uso por usuario.
   * Cálculo de cantidad de llamadas, mensajes y minutos utilizados.
   * Segmentación de clientes por edad.
   * Segmentación según nivel de uso: bajo, medio y alto.
5. **Análisis de valores atípicos**
   * Identificación de outliers mediante el rango intercuartílico (IQR).
   * Evaluación de si los valores atípicos corresponden a errores o a comportamientos reales de los usuarios.
6. **Conclusiones y recomendaciones**
   * Interpretación de los principales resultados.
   * Identificación de segmentos relevantes.
   * Propuesta de recomendaciones orientadas al comportamiento y consumo de los clientes.
## Cómo ejecutar el notebook
El proyecto puede ejecutarse en **Jupyter Notebook**.
Si se tiene Python y Jupyter instalado:
```bash
jupyter notebook
```
Luego abrir:
```text
S7 sprint7-final-project.ipynb
```
## Guía de reproducción
Para reproducir el análisis:

1. Descargar los tres datasets del proyecto.
2. Colocarlos en una carpeta `datasets/`.
3. Abrir el notebook en Google Colab o Jupyter Notebook.
4. Verificar que las rutas de los archivos CSV coincidan con la ubicación de los datasets.
5. Ejecutar las celdas en el orden establecido.
6. Revisar las transformaciones y resultados obtenidos.
7. Generar nuevamente las tablas y visualizaciones para comprobar los resultados del análisis.

### Estructura recomendada
```text
ConnectaTel/
│
├── datasets/
│   ├── users_latam.csv
│   ├── usage.csv
│   └── plans.csv
│
├── sprint7-final-project.ipynb
│
└── README.md
```
## Tecnologías utilizadas
* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook / Google Colab

## Resultado
El análisis permite conocer las principales características de los usuarios de ConnectaTel, identificar problemas de calidad en los datos y segmentar a los clientes según su edad y nivel de uso. Los resultados sirven como base para generar recomendaciones relacionadas con los planes y el comportamiento de consumo de los usuarios.

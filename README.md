# 🚖 Análisis de Datos de Taxis en Chicago - Zuber

📋 Descripción Breve
Proyecto de análisis de datos para Zuber, una nueva empresa de viajes compartidos que se lanza en Chicago. El objetivo es identificar patrones en el comportamiento de pasajeros, analizar la competencia y evaluar el impacto de factores externos como el clima en la frecuencia y duración de los viajes.

🛠️ Tecnologías Utilizadas
SQL
Extracción y manipulación de datos de bases de datos
Python 3.8+
Análisis de datos y estadísticas
Pandas
Manipulación y análisis de datasets
NumPy
Operaciones numéricas y estadísticas
Matplotlib
Visualización de datos
Seaborn
Gráficos estadísticos avanzados
SciPy
Pruebas de hipótesis estadísticas
Requests/BeautifulSoup
Web scraping de datos meteorológicos
Jupyter Notebook
Entorno de desarrollo interactivo
📊 Descripción del Proyecto
🎯 Objetivos Principales
Analizar patrones de uso de taxis en Chicago durante noviembre 2017
Identificar empresas competidoras y su participación en el mercado
Determinar barrios más populares como destinos de viajes
Evaluar el impacto del clima en la duración de viajes específicos
Proporcionar insights estratégicos para el lanzamiento de Zuber
🔍 Metodología
El proyecto combina análisis de bases de datos SQL con análisis exploratorio en Python, incluyendo web scraping de datos meteorológicos y pruebas de hipótesis estadísticas para validar hallazgos sobre el impacto climático en los viajes.

🗄️ Estructura de Datos
Base de Datos Principal (SQL)
Tabla neighborhoods - Información de barrios
- name - Nombre del barrio
- neighborhood_id - Código único del barrio

Tabla cabs - Información de vehículos
- cab_id - Código del vehículo
- vehicle_id - ID técnico del vehículo
- company_name - Empresa propietaria

Tabla trips - Datos de viajes
- trip_id - Código único del viaje
- start_ts/end_ts - Timestamps de inicio/fin
- duration_seconds - Duración en segundos
- distance_miles - Distancia en millas
- pickup_location_id/dropoff_location_id - Códigos de ubicaciones

Tabla weather_records - Datos meteorológicos
- record_id - Código del registro
- ts - Timestamp del registro
- temperature - Temperatura registrada
- description - Descripción de condiciones climáticas

Datasets Generados (CSV)
project_sql_result_01.csv
Viajes por empresa (15-16 nov 2017)
project_sql_result_04.csv
Promedio de viajes por barrio de destino
project_sql_result_07.csv
Viajes Loop-O'Hare con datos climáticos

⚙️ Funcionalidades Implementadas
### 🌐 Web Scraping
- Extracción de datos meteorológicos de Chicago (noviembre 2017)
- Procesamiento automático de condiciones climáticas
- Integración de datos externos con datasets principales

### 📊 Análisis SQL
- Consultas complejas para identificar top empresas de taxis
- Análisis de frecuencia de viajes por barrio de destino
- Extracción de viajes específicos Loop-Aeropuerto O'Hare
- Joins entre múltiples tablas para análisis integral

### 📈 Análisis Exploratorio (EDA)
- Visualización de participación de mercado por empresa
- Análisis de distribución de viajes por barrios populares
- Estudio de patrones temporales en viajes Loop-O'Hare
- Correlación entre condiciones climáticas y duración de viajes

### 🧪 Pruebas de Hipótesis
- **H0:** La duración promedio de viajes Loop-O'Hare es igual en días lluviosos vs no lluviosos
- **H1:** La duración promedio difiere según condiciones climáticas
- Aplicación de t-test para muestras independientes (α = 0.05)

## 🚀 Instalación y Uso

### Prerrequisitos

```bash
Python 3.8+
Jupyter Notebook
Acceso a base de datos SQL

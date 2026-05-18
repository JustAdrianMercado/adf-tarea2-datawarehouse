# adf-tarea2-datawarehouse
Descripción:

El Programa Ampliado de Inmunización (PAI) es el programa preventivo más importante del sistema de salud boliviano. Organizado desde 1979, su objetivo es reducir el riesgo de enfermar y morir por enfermedades inmunoprevenibles (tuberculosis, poliomielitis, sarampión, difteria, tétanos, tos ferina, hepatitis B, neumonías, diarreas por rotavirus, fiebre amarilla, entre otras) mediante la aplicación universal y gratuita de vacunas a toda la población boliviana.
El Ministerio de Salud y Deportes necesita consolidar todos estos registros en un Data Warehouse centralizado para monitorear coberturas de vacunación, detectar brechas en el esquema PAI, planificar campañas estacionales (como influenza pre-invierno) y asegurar la cadena de frío en todo el territorio nacional.
Objetivo:

Diseñar e implementar un pipeline ETL (Extracción, Transformación y Carga) en Azure Data Factory que consolide registros de vacunación de múltiples fuentes heterogéneas en un Data Warehouse con esquema estrella, resolviendo problemas reales de calidad de datos en el proceso.

Periodo de los Datos:

Enero 2024 a Junio 2025 (18 meses).

Catalogo de Datos:

Catalogo Departamentos:

 

Catalogo de vacunas PAI

 

Catalogo de establecimientos

 dgdf

Datos Vacunaciones Santa cruz, La Paz y Rural

 

Sugerencia de modelo de datwarehouse (Modelo Estrella)

 DIM_TIEMPO
DIM_ESTABLECIMIENTO
DIM_VACUNA
DIM_PACIENTE
HECHOS_VACUNACION
Stack Azure 
Grupo de Recurso
Storage Accounts - Datalake gen 2
Sql Database
Azure Datafactory
tota los servicios deben ser automatizados con terraform
 
 
Arquitectura
Bronze -> datos crudos
Silver -> limpieza e integracion de los datos
Gold -> creacion del datawarehouse etl & pipelines

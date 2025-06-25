# BDNR
Repositorio para Proyecto Final de Bases de Datos No Relacionales (Fing)

# Proyecto Final - Bases de Datos No Relacionales (BDNR)

Este repositorio contiene el proyecto final realizado para la materia **Bases de Datos No Relacionales**, correspondiente a la Maestría en Ciencia de Datos y Aprendizaje Automático. El trabajo se centra en la migración de un modelo de base de datos relacional hacia un modelo documental utilizando MongoDB, con el objetivo de mejorar la eficiencia de consultas, la escalabilidad del sistema y la flexibilidad estructural.

---

## Contenidos del repositorio

- `relational_database_data.zip`: Archivos JSON que representan las **tablas originales** del modelo relacional, utilizadas para cargar la base de datos inicial en MongoDB Atlas.
- `BDNR_2025_Tarea_Final_Auriello_Molina.ipynb`: Notebook principal del proyecto. Contiene las **transformaciones realizadas en Python** para migrar la base de datos relacional a una estructura documental en MongoDB.
- `Proyecto_Final_Consultas_SQL_para_comparacion.ipynb`: Notebook complementario que contiene las **consultas SQL comparativas** ejecutadas sobre una réplica del modelo relacional cargado en SQLite.
- `Auriello_Molina_Informe_Final_BDNR.pdf`: Informe final del trabajo, redactado en formato académico, que describe el contexto, decisiones de modelado, transformaciones, consultas y análisis de performance.
- `Plandetrabajo_BDNR2025_Auriello_Molina CHECKPOINT 2 (1).pdf`: Plan de trabajo inicial presentado en etapas tempranas del proyecto, incluyendo objetivos y diseño preliminar.

---

## Tecnologías utilizadas

- **MongoDB Atlas** (modelo documental)
- **Amazon Redshift** (modelo relacional original)
- **Python** con:
  - `pymongo`
  - `pandas`
  - `sqlite3`
- **Google Colab** como entorno de desarrollo
- **LaTeX** para la redacción del informe

---

## Estructura del proyecto

El proyecto se organiza en tres partes principales:

### 1. Migración de modelo relacional a documental
A partir de archivos JSON que representan tablas relacionales (`fact_vod_details`, `dim_client`, `dim_device`, etc.), se construyó una base documental en MongoDB. Se aplicaron patrones de modelado como:

- **Embedding** de dimensiones de baja cardinalidad
- **Subset pattern** para `users`
- **Extended reference pattern** para `clients`

### 2. Consultas comparativas
Se diseñaron y ejecutaron consultas representativas en:

- Redshift (entorno original)
- SQLite en Google Colab (entorno simulado)
- MongoDB Atlas (modelo documental)

Se midieron los tiempos de ejecución para comparar la performance entre modelos.

### 3. Documentación y análisis
El informe final documenta el proceso completo, decisiones de diseño, estructuras finales y resultados de las comparaciones, con capturas, esquemas y ejemplos de código.

---

## Autores

- **Joana Uriello**
- **Pablo Molina**

---

## Licencia

Este repositorio es de uso académico. Para más información, contactá a los autores.


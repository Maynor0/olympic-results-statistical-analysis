# Olympic Results Analysis

## Descripción
Este proyecto analiza una base de resultados olímpicos en formato parquet. El trabajo se divide en dos partes: limpieza y transformación de datos, y análisis exploratorio con visualizaciones.

## Objetivo
Explorar el comportamiento del medallero olímpico por país, deporte, atleta, categoría, tipo de juego y evolución temporal.

## Estructura del proyecto
- `notebooks/01_olympics_cleaning.ipynb`: limpieza, transformación de tipos, renombrado de columnas y normalización de texto.
- `notebooks/02_olympics_analysis.ipynb`: análisis exploratorio, tablas resumen y gráficos.
- `data/`: archivo fuente en formato parquet.
- `images/`: gráficos exportados en PNG.
- `output/`: tablas resumen exportadas en CSV.

## Dataset
La base contiene información de resultados olímpicos con variables como:
- Año
- Juegos
- Deporte
- Categoria
- Atleta
- ID_Atleta
- NOC
- Equipo
- Posicion
- Empatado
- Medalla

## Limpieza de datos
En la fase de limpieza se realizaron tareas como:
- Conversión de tipos de datos.
- Tratamiento de valores nulos.
- Limpieza de espacios en texto.
- Eliminación de tildes en algunas columnas.
- Renombrado de columnas al español.
- Normalización de los valores de Juegos a Verano e Invierno.

## Análisis realizado
Se desarrollaron análisis sobre:
- Países con más medallas.
- Deportes con más medallas.
- Evolución de medallas por año.
- Comparación entre Juegos de Verano e Invierno.
- Atletas con más apariciones en el medallero.
- Deportes con más empates.
- Conteo de medallas por tipo.
- Distribución de posiciones.
- Categorías con más medallas.
- Heatmap de medallas por país y año.

## Herramientas usadas
- Python
- pandas
- numpy
- matplotlib
- seaborn
- pyarrow
- Jupyter Notebook

## Principales hallazgos
- El medallero se concentra en un grupo reducido de países.
- Algunos deportes, como Athletics y Artistic Gymnastics, acumulan gran parte de las medallas.
- Los Juegos de Verano registran más medallas que los de Invierno.
- El análisis temporal permite detectar periodos de dominio por país.
- La distribución de posiciones muestra una fuerte concentración en los primeros puestos.

## Cómo ejecutar
1. Clonar este repositorio.
2. Instalar las dependencias:
   ```bash
   pip install -r requirements.txt
   ```
3. Abrir los notebooks en Jupyter.
4. Ejecutar primero `01_olympics_cleaning.ipynb`.
5. Ejecutar después `02_olympics_analysis.ipynb`.

## Autor
Proyecto realizado como práctica de análisis de datos con Python.
# Data

## Descripción
Esta carpeta contiene los archivos de datos utilizados en el proyecto de análisis de resultados olímpicos.

## Archivos
- `results.parquet`: archivo original con los resultados olímpicos.
- `data_new.parquet`: archivo transformado y limpiado para el análisis exploratorio, si se incluye en el repositorio.

## Formato
Los datos están almacenados en formato Parquet para facilitar una lectura eficiente con pandas.

## Variables principales
El dataset trabajado en el análisis incluye las siguientes columnas:
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

## Transformaciones realizadas
Durante la limpieza de datos se aplicaron las siguientes transformaciones:
- Conversión de tipos de datos en columnas numéricas.
- Tratamiento de valores nulos.
- Limpieza de espacios en variables de texto.
- Eliminación de tildes en algunas columnas.
- Renombrado de columnas al español.
- Estandarización de los valores de `Juegos` en Verano e Invierno.

## Uso en el proyecto
- `01_olympics_cleaning.ipynb` trabaja sobre el archivo original.
- `02_olympics_analysis.ipynb` utiliza la versión limpia para generar tablas y gráficos.

## Nota
Si algún archivo de datos no se incluye en GitHub por tamaño, debe indicarse aquí y explicarse cómo obtenerlo o generarlo a partir del notebook de limpieza.
# Análisis de resultados olímpicos

## Objetivo
Analizar una base de resultados olímpicos para explorar diferencias entre tipos de Juegos, países, deportes y evolución temporal, utilizando Python y SciPy para estadística descriptiva e inferencial.

## Dataset
Archivo principal: `results.parquet`

Columnas principales:
- `year` / `Año`
- `type` / `Juegos`
- `discipline` / `Deporte`
- `event` / `Categoria`
- `as` / `Atleta`
- `athlete_id` / `ID_Atleta`
- `noc` / `NOC`
- `team` / `Equipo`
- `place` / `Posicion`
- `tied` / `Empatado`
- `medal` / `Medalla`

## Proceso

1. Limpieza y preparación de datos:
   - Conversión de tipos.
   - Relleno de valores nulos.
   - Eliminación de espacios y tildes.
   - Renombrado de columnas al español.
   - Reemplazo de `Summer` por `Verano` y `Winter` por `Invierno`.

2. Análisis descriptivo:
   - `stats.describe()`.
   - Media, mediana, desviación estándar.
   - Cuartiles, IQR y valores atípicos.

3. Comparación entre tipos de Juegos:
   - Prueba U de Mann–Whitney.
   - Comparación de medias, medianas y dispersión entre Verano e Invierno.
   - Visualización con boxplot.

4. Medallero por país:
   - Conteo de medallas por NOC.
   - Análisis de concentración del medallero.
   - Comparación del país líder frente al resto.

5. Análisis por deporte:
   - Resumen descriptivo de posiciones por disciplina.
   - ANOVA de un factor para comparar deportes con tamaño muestral suficiente.

6. Evolución temporal:
   - Medallas por año para un país concreto.
   - Regresión lineal con `linregress`.

7. Asociación entre país y tipo de medalla:
   - Tabla de contingencia.
   - Prueba chi-cuadrado de independencia.

## Resultados destacados
- Los Juegos de Verano muestran mejores posiciones centrales que los de Invierno.
- Existe una fuerte concentración del medallero en pocos países.
- Las posiciones medias difieren significativamente entre deportes.
- No se observa una tendencia lineal clara en la evolución temporal de medallas para USA.
- Existe asociación entre `NOC` y `Medalla`.

## Tecnologías utilizadas
- `pandas`
- `numpy`
- `scipy`
- `matplotlib`
- `seaborn`

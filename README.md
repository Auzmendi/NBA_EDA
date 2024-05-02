# NBA_EDA


# Análisis Exploratorio de Datos (EDA) de Partidos de la NBA

## Introducción:

Este proyecto de análisis de datos explora un conjunto de datos que contiene información sobre partidos de la NBA desde la temporada 1946-47 hasta la temporada 2022-23. El objetivo del proyecto es comprender mejor los patrones y tendencias presentes en los datos, identificar posibles hipótesis y generar ideas para futuras investigaciones.

## Conjunto de datos:

El conjunto de datos utilizado en este análisis se encuentra en el archivo game_1.csv. Contiene las siguientes variables:


#### STATS GENERALES
* **season_id** : hay una cifra(2,3,etc) y seguido el año de inicio de la temporada.
* **team_id_home**, un id para idenatificar a los equipos. 
* **team_abbreviation_home**, abreviatura del nombre del equipo
* **team_name_home**, nombre del equipo
* **game_id**, identificador del partido al que referencian las estadisiticas de esta fila
* **game_date**, fecha de dicho partido
* **matchup_home**, muestra quienes son los equipos que juegan con sus abrreviaturas y vs en el medio
* **wl_home**,  -----no he encontrado nada------
* **min**, minutos jugados

### STATS POR EQUIPO
### EQUIPO LOCAL
#### TIROS DE CAMPO
* **fgm_home**, field goals made por el equipo local. canastas de 2 ptos HECHAS!
* **fga_home**, field goals attempted por el equipo local. canastas de 2 ptos INTENTADAS!
* **fg_pct_home**,   field goals percentage
* 
#### TIROS DE 3 PUNTOS
* **fg3m_home**, tiros de 3 convertidos
* **fg3a_home**, tiros de 3 intentados
* **fg3_pct_home**, porcentaje de acierto en tiros de 3
* 
#### TIROS LIBRES
* **ftm_home**, tiros libres convertidos
* **fta_home**,tiros libres intentados
* **ft_pct_home**, porcentaje de acierto en tiros libres

#### REBOTES / ASISTENCIAS / ROBOS / TAPONES / PERDIDAS / FALTAS / PUNTOS
* **oreb_home**, rebotes ofensivos
* **dreb_home**,rebotes defensivos
* **reb_home**,rebotes totales
* **ast_home**,asistencias
* **stl_home**,robos
* **blk_home**,tapones
* **tov_home**, pérdidas de balón
* **pf_home**, faltas
* **pts_home**, puntos
* **plus_minus_home**, valoración
* **video_available_home**, video disponible.

### EQUIPO VISITANTE
#### STATS GENERALES
* **team_id_away**, un id para idenatificar a los equipos.
* **team_abbreviation_away**,abreviatura del nombre del equipo
* **team_name_away**, nombre del equipo
* **matchup_away**,muestra quienes son los equipos que juegan con sus abrreviaturas y vs en el medio
* **wl_away**, -----no he encontrado nada------

#### TIROS DE CAMPO
* **fgm_away**, field goals made por el equipo local. canastas de 2 ptos HECHAS!
* **fga_away**, field goals attempted por el equipo local. canastas de 2 ptos INTENTADAS!
* **fg_pct_away**,   field goals percentage

#### TIROS DE 3 PUNTOS 
* **fg3m_away**, tiros de 3 convertidos
* **fg3a_away**, tiros de 3 intentados
* **fg3_pct_away**, porcentaje de acierto en tiros de 3

#### TIROS LIBRES
* **ftm_away**, tiros libres convertidos
* **fta_away**, tiros libres intentados
* **ft_pct_away**, porcentaje de acierto en tiros libres

#### REBOTES / ASISTENCIAS / ROBOS / TAPONES / PERDIDAS / FALTAS / PUNTOS
* **oreb_away**, rebotes ofencsivos
* **dreb_away**, rebotes defensivos
* **reb_away**, rebotes totales
* **ast_away**, asistencias
* **stl_away**, robos
* **blk_away**, tapones
* **tov_away**, pérdidas de balón
* **pf_away**, faltas
* **pts_away**, puntos
* **plus_minus_away**, valoración
* **video_available_away**, video disponible

## INDICADOR DE TIPO DE PARTIDO (PLAYOFF, TEMPORADA REGULAR, ALL STAR)
* **season_type** , indicador del tipo de partido. 3 opciones , 'Regular Season', 'Playoffs', 'All Star'


## Análisis Exploratorio de Datos (EDA):

El EDA se realizó utilizando el lenguaje de programación Python y las bibliotecas pandas, matplotlib y seaborn. Se llevaron a cabo las siguientes tareas:

* Limpieza de datos: Se eliminaron las filas con valores perdidos en las variables clave.
* Análisis descriptivo: Se calcularon medidas de resumen básicas para las variables numéricas y se analizaron las distribuciones de las variables mediante histogramas y diagramas de caja y bigotes.
* Análisis exploratorio de hipótesis: Se realizaron pruebas t de Student para comparar las medias de puntos anotados, rebotes, asistencias, robos, tapones y pérdidas entre equipos locales y visitantes. También se analizaron las tendencias en la puntuación y el número de triples a lo largo del tiempo.
* Identificación de patrones y tendencias: Se identificaron patrones interesantes en los datos, como la mayor probabilidad de victoria para los equipos locales y el aumento de la puntuación y el número de triples a lo largo del tiempo.
* Generación de ideas para futuras investigaciones: Se propusieron estudios futuros para profundizar en el análisis, como el estudio del impacto de jugadores individuales o el análisis de la influencia de factores externos como las lesiones o el calendario de partidos.
  
## Conclusiones:

El EDA realizado en este proyecto ha proporcionado información valiosa sobre los patrones y tendencias presentes en los datos de partidos de la NBA. Se han confirmado las hipótesis planteadas y se han identificado nuevos aspectos que podrían ser objeto de estudio en futuras investigaciones.

* **HIPÓTESIS 1:** El estilo de juego ha cambiado con el tiempo en la NBA, con un aumento de la puntuación y un mayor número de triples.

* **HIPÓTESIS 2:** Los equipos locales tienen una mayor probabilidad de ganar los partidos.

* **HIPÓTESIS 3:** Los equipos con mayor % de tiro de 3 puntos tienen una mayor probabilidad de ganar los partidos.

## Recomendaciones:

Se recomienda continuar con el análisis de datos de la NBA utilizando técnicas más avanzadas, como el modelado estadístico y el aprendizaje automático.
También se recomienda recopilar datos adicionales sobre jugadores, entrenadores y equipos para obtener una comprensión más completa del juego.

## Recursos:

https://pandas.pydata.org/
https://matplotlib.org/
https://stackoverflow.com/

## Próximos pasos:

* Implementar modelos estadísticos para predecir el resultado de los partidos.
* Aplicar técnicas de aprendizaje automático para identificar patrones complejos en los datos.
* Analizar el impacto de jugadores individuales en el rendimiento de los equipos.
* Estudiar la influencia de factores externos como las lesiones o el calendario de partidos.

<div align="center">

# taller_github_grupo_7

# $\color{blue}\text{KDD Cup 2009: Predicción de abandono y propensión de clientes}$ 


</div align="center">

## Este proyecto fue ejecutado por la científica de datos Claudia Perlich: su participación fue ganadora en el KDD Cup 2009 – Orange Challenge (tarea "Fast Challenge for CRM").


# Enfoque orientado a la toma de decisiones

El proyecto de la **KDD Cup 2009**, en el que participó Claudia Perlich, buscaba predecir diferentes comportamientos de los clientes de Orange.

Entre estos comportamientos se encontraban:

- **Churn:** probabilidad de que un cliente abandone la compañía.
- **Appetency:** probabilidad de que un cliente compre un nuevo producto o servicio.
- **Up-selling:** probabilidad de que un cliente adquiera productos o servicios adicionales.

Una de las características principales de este proyecto es su enfoque orientado a la toma de decisiones.

El objetivo no era solamente construir un modelo con buena capacidad predictiva, sino utilizar los datos de los clientes para obtener información útil sobre su comportamiento.

Gracias a estas predicciones, los resultados del modelo podían servir como apoyo para la toma de decisiones comerciales dentro de una empresa de telecomunicaciones.

De esta manera, el proyecto muestra cómo la ciencia de datos puede transformar grandes cantidades de información en conocimiento útil para comprender mejor a los clientes y apoyar decisiones empresariales.

## Selección pragmática de modelos (Ensemble Selection)

En lugar de apostar por un único algoritmo, el equipo de Claudia Perlich construyó una biblioteca de entre 500 y 1000 modelos para cada uno de los tres problemas (churn, appetency y up-selling). Entre ellos había regresión logística, Random Forest y árboles de decisión con boosting.

Luego aplicaron Ensemble Selection, donde se eligen varios modelos de la biblioteca y se combinan sus predicciones. La idea es que cada modelo detecta patrones distintos en los datos, y al combinarlos el resultado es más robusto y preciso que el de cualquier modelo individual. Esta tecnica llevo al equipo de Claudia a ganar la copa ese año. 

 La lección de esto es que probar muchas alternativas y combinar las mejores suele funcionar mejor que depender de un solo algoritmo.


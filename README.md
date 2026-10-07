<div align="center">

# taller_github_grupo_7

# $\color{blue}\text{KDD Cup 2009: Predicción de abandono y propensión de clientes}$ 


</div align="center">

## Este proyecto fue ejecutado por la científica de datos Claudia Perlich: su participación fue ganadora en el KDD Cup 2009 – Orange Challenge (tarea "Fast Challenge for CRM").

<h2 align="center">Integrantes del grupo 7</h2>

<div align="center">

| Nombre | Codigo |
|--------|---------|
| Juan Barbosa Aguilar | 202420510 |
| Jeronimo Gomez Sarmiento | 202420510 |
| Maria Fernanda leal rojas | 
| Andres Tovar Rodriguez | 202621740 |

</div>

# $\color{blue}\text{Problema inicial}$

**Contexto:** Orange, una de las principales empresas de telecomunicaciones de Francia, necesitaba manejar mejor la relación con sus clientes (CRM, *Customer Relationship Management*). Para personalizar esa relación, la empresa usa **puntajes (scores)**: valores que un modelo calcula para cada cliente y que indican qué tan probable es cierto comportamiento.

**Problema:** Con una base de datos de clientes muy grande, con variables numéricas y categóricas, ruidosas y con muchos datos faltantes, la empresa quería predecir tres comportamientos:

| Comportamiento | Qué se quería predecir |
|----------------|------------------------|
| $\color{brown}\text{Churn}$ | Si el cliente cambiaría de proveedor (abandono) |
| $\color{pink}\text{Appetency}$ | Si el cliente compraría un nuevo producto o servicio |
| $\color{green}\text{up-selling}$ | Si el cliente compraría mejoras o complementos que le ofrecen para hacer la venta más rentable |

**Objetivo:** Construir modelos que superaran al sistema interno desarrollado por Orange Labs, y hacerlo con rapidez. Parte de la competencia tenía límite de tiempo para evaluar la capacidad de entregar soluciones ágiles. El desempeño se midió con el **AUC** promedio de los tres modelos.

**Valor para el negocio:** Con estos puntajes, la empresa puede decidir a qué clientes dirigir campañas de retención (churn), de venta de nuevos productos (appetency) y de mejoras de servicio (up-selling), en lugar de contactar a todos por igual




# $\color{blue}\text{Enfoque orientado a la toma de decisiones}$

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


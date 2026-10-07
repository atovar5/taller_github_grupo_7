 <h1 align="center">Trabajo_asistido_intro_ciencia_datos_11am_taller_github_barbosa_gomez_leal_tovar</h1>

<h2 align="center">KDD Cup 2009: Predicción de abandono y propensión de clientes</h2>

<p align="center">Este proyecto fue ejecutado por la científica de datos Claudia Perlich: su participación fue ganadora en el KDD Cup 2009 – Orange Challenge (tarea "Fast Challenge for CRM").</p>

<h2 align="center">Integrantes del grupo 7</h2>

<div align="center">

| Nombre | Codigo |
|--------|---------|
| Juan Barbosa Aguilar | 202420510 |
| Jeronimo Gomez Sarmiento | 202420510 |
| Maria Fernanda leal rojas | 202616497 |
| Andres Tovar Rodriguez | 202621740 |

</div>

<h1 align="center">Problema inicial</h1>

**Contexto:** Orange, una de las principales empresas de telecomunicaciones de Francia, necesitaba manejar mejor la relación con sus clientes (CRM, *Customer Relationship Management*). Para personalizar esa relación, la empresa usa **puntajes (scores)**: valores que un modelo calcula para cada cliente y que indican qué tan probable es cierto comportamiento.

**Problema:** Con una base de datos de clientes muy grande, con variables numéricas y categóricas, ruidosas y con muchos datos faltantes, la empresa quería predecir tres comportamientos:

<div align="center">

| Comportamiento | ¿Qué se quería predecir? |
|----------------|--------------------------|
| **Churn** (Abandono) | Si el cliente cambiaría de proveedor |
| **Appetency** (Apetencia) | Si el cliente compraría un nuevo producto o servicio |
| **Up-selling** (Venta ascendente) | Si el cliente compraría mejoras o complementos que le ofrecen para hacer la venta más rentable |

</div>

**Objetivo:** Construir modelos que superaran al sistema interno desarrollado por Orange Labs, y hacerlo con rapidez. Parte de la competencia tenía límite de tiempo para evaluar la capacidad de entregar soluciones ágiles. El desempeño se midió con el **AUC** promedio de los tres modelos.

**Valor para el negocio:** Con estos puntajes, la empresa puede decidir a qué clientes dirigir campañas de retención (churn), de venta de nuevos productos (appetency) y de mejoras de servicio (up-selling), en lugar de contactar a todos por igual



<h1 align="center"><b>Enfoque orientado a la toma de decisiones</b></h1>

El proyecto de la **KDD Cup 2009**, en el que participó Claudia Perlich, buscaba predecir diferentes comportamientos de los clientes de Orange.

Entre estos comportamientos se encontraban:

- **Churn:** probabilidad de que un cliente abandone la compañía.
- **Appetency:** probabilidad de que un cliente compre un nuevo producto o servicio.
- **Up-selling:** probabilidad de que un cliente adquiera productos o servicios adicionales.

Una de las características principales de este proyecto es su enfoque orientado a la toma de decisiones.

El objetivo no era solamente construir un modelo con buena capacidad predictiva, sino utilizar los datos de los clientes para obtener información útil sobre su comportamiento.

Gracias a estas predicciones, los resultados del modelo podían servir como apoyo para la toma de decisiones comerciales dentro de una empresa de telecomunicaciones.

De esta manera, el proyecto muestra cómo la ciencia de datos puede transformar grandes cantidades de información en conocimiento útil para comprender mejor a los clientes y apoyar decisiones empresariales.

<h2 align="center"><b>Selección pragmática de modelos (Selección de conjuntos)</b></h2>

En lugar de apostar por un único algoritmo, el equipo de Claudia Perlich construyó una biblioteca de entre 500 y 1000 modelos para cada uno de los tres problemas (churn, appetency y up-selling). Entre ellos había regresión logística, Random Forest y árboles de decisión con boosting.

Luego aplicaron Ensemble Selection, donde se eligen varios modelos de la biblioteca y se combinan sus predicciones. La idea es que cada modelo detecta patrones distintos en los datos, y al combinarlos el resultado es más robusto y preciso que el de cualquier modelo individual. Esta tecnica llevo al equipo de Claudia a ganar la copa ese año. 

 La lección de esto es que probar muchas alternativas y combinar las mejores suele funcionar mejor que depender de un solo algoritmo. 

<h1 align="center"><b>Características Clave del Proyecto</b></h1>

1. Trabajo de Detective y Criterio Crítico con los Datos : El verdadero éxito de la investigación no estuvo en usar el algoritmo más avanzado, sino en entender los datos desde el primer día: en vez de meter a ciegas una base enorme, ruidosa y llena de huecos al modelo, actuó como detective revisando cada variable con lupa, corrigiendo fallas y evitando la filtración de información, demostrando así que la curiosidad y el sentido crítico pesan más que la simple fuerza de cómputo.

2.  Mantener las Cosas Simples y Útiles : En vez de complicarse la vida buscando la fórmula mágica o el algoritmo más raro, el equipo se fue por lo práctico. Apostaron por modelos conocidos, rápidos y confiables que no se colgaran al procesar miles de datos. Nos deja claro que, cuando el tiempo aprieta, una solución clara y bien ejecutada vale mucho más que una idea híper complicada que nadie puede mover.

3.  Pensar en el Negocio Antes que en la Computadora : o importante aquí no era sacar una nota perfecta en la métrica solo por presumirla, sino lograr algo que a la empresa le sirviera los lunes por la mañana. Cada resultado estaba pensado para que el equipo de ventas supiera a quién llamar, qué ofrecerle o a quién retener antes de que se cancelara el servicio. El foco siempre estuvo en resolver un problema real, no solo en correr código.

4.  Aprender a Trabajar Contra el Reloj : Como la competencia exigía entregas relámpago, no había espacio para quedarse pensando semanas. La estrategia fue probar rápido, ver qué servía, corregir lo que fallaba y desechar lo que estorbaba sin rodeos. Refleja muy bien cómo se siente la presión en el mundo laboral, donde hay que tomar decisiones ágiles y entregar resultados finos con el tiempo justo.

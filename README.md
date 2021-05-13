### TABLE OF CONTENTS

* DATASET TITLE
* AUTHORS AND AFFILIATIONS
* LANGUAGE
* SUMMARY/ABSTRACT
* KEYWORDS
* FILE ORGANIZATION
* DATASET DESCRIPTION 


### DATASET TITLE

Tráfico y Errores de un flow e-commerce genérico para
la introducción a Optimización de Tasa de Conversión en productos digitales

###  AUTHORS AND AFFILIATIONS

* Name: Luis Epifanio
* Organization/institution: Facultad de Matemática, Astronomía y Física de la Universidad Nacional de Córdoba
* Email: luis.epifanio[at]gmail.com

### LANGUAGE
Spanish

### SUMMARY/ABSTRACT

En su propósito, este dataset se desarrollo y adaptó para el dictado de la diplomatura de [DIPLOMATURA
ENCIENCIA DE DATOS, APRENDIZAJE AUTOMÁTICO
Y SUS APLICACIONES 2021](https://diplodatos.famaf.unc.edu.ar/) y persigue al menos dos objetivos principales:
1. Por una parte compartir y servir de introducción a la optimización de productos
digitales, planteando con una perspectiva simplificada ( ya que no incluye todas las variables de decisión de ) un proceso implementado en la industria.

2. Permite explorar e implementar muchos de los conceptos revisados en el dictado de la diplomatura en ciencia de datos por ej: análisis exploratorio,
curación, aprendizaje no supervisado,etc.. Como así también modelos predictivos
de series temporales, de aprendizaje automático y su combinación ( y quizás poder
construir modelos simples para detección de anomalías ). Por medio de dichos
modelos se intentará explicar el comportamiento de los usuarios y determinación
de KPI del producto.

En su dominio e intentando describir el comportamiento del usurio [el dataset de tráfico](traffic_AR_CL_UY.csv) intenta reflejar el tráfico entre las pantallas de un flujo de Compras / Checkout de un e-commerce generico ( muy inspirado en el de MercadoLibre )

![CheckOut Generic Diagram](./assets/images/checkout-flow.svg)

De manera más gráfica podemos asociarla a la siguiente experiencia de compra:

|   |   |   |   |   |
|:-:|---|---|---|---|
|  <img src="./assets/images/LOADING.jpeg" width="120" >  |  <img src="./assets/images/SHIPPING.jpeg" width="120" > | <img src="./assets/images/PAYMENTS.jpeg" width="120" >  |  <img src="./assets/images/REVIEW.jpeg" width="120" > |  <img src="./assets/images/CONGRATS.jpeg" width="120" > |

Por otra parte e intentando describir el comportamiento de la infraestructura
acompañamos [el dataset de eventos](events_AR_CL_UY.csv) que intente describir
los eventos/errores registrados durante la ejecución de los pasos de las experiencias 
anteriores

### KEYWORDS

To Be Definded

### FILE ORGANIZATION

El dataset consiste en 2 archivos:

1. [El dataset de tráfico](traffic_AR_CL_UY.csv) intenta reflejar el tráfico entre las pantallas de un flujo de Compras
2. [El dataset de eventos](events_AR_CL_UY.csv) que intente describir
los eventos/errores registrados durante la ejecución de los pasos del flow

### DATASET DESCRIPTION
1. [El dataset de tráfico](traffic_AR_CL_UY.csv) intenta reflejar el tráfico entre las pantallas de un flujo de Compras

| Nombre   |  Tipo  | Formato    | Descripción |
|----------|--------|------------|-------------|
| Fecha    |  Date | YYYY-MM-DD |  Los valores corresponde a los eventos registrados durante este día |
| flow     | String | direct-cart | Define si el flujo corresponde a compra directa o de carrito |
| Site     | String |   XXX       |             |
| Device   |        |             | Define el dispositivo donde se ejecuto el flujo de compra |
| Loading  | Entero |             | Cantidad de sesiones que vieron el paso de Loading  |
| Shipping |        |             | Cantidad de sesiones que vieron el paso de Shipping |
| Payments |        |             | Cantidad de sesiones que vieron el paso de Payments |
| Review   |        |             | Cantidad de sesiones que vieron el paso de Review   |
| Congrats |        |             | Cantidad de sesiones que vieron el paso de Congrats |




2. [El dataset de eventos](events_AR_CL_UY.csv) que intente describir
los eventos/errores registrados durante la ejecución de los pasos del flow

| Nombre   |  Tipo | Formato  | Descripción |
|----------|-------|----------|-------------|
| start    |       |          |             |
| end      |       |          |             |
| site     |       |          |             |
| event    |       |          |             |
| count    |       |          |             |
| cost     |       |          |             |





 
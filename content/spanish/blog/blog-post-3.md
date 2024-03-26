---
title: "CUBO OLAP "
date: 2024-03-24T11:07:10+06:00
author: [ "Jazmin Pineda" ]
image : "images/blog/blog-post-3.png"
bg_image: "images/feature-bg.jpg"
categories: ["Business Intelligence"]
tags: ["Base de Datos","Herramientas"]
description: "Herramienta superpoderosa en Business Intelligence."
draft: false
type: "post"
---

Imagen tomada curso LEVO especialización Dominio de Datos con Power BI.

</p>
En el siguiente artículo, deseo compartirles mi primera experiencia con una herramienta de Business Intelligence en OLAP. En mi travesía, me encontré con una escasez de documentación a nivel interno y una capacitación prácticamente inexistente, situaciones comunes para aquellos que incursionamos en este campo. 

<P>

Sin embargo, tras una exhaustiva investigación, descubrí un verdadero tesoro oculto que reside en las capacidades avanzadas que tiene el concepto CUBO OLAP y su relación con Excel. Permítanme contarles brevemente cómo me adentré en este tema.

</P>

Todo comenzó con un nuevo proyecto: debía implementar un Dashboard en una aplicación que operaba con **CUBOS OLAP (Procesamiento Analítico En Línea)**, una solución vital en el ámbito de **Business Intelligence**. 

Este sistema permite crear reportes personalizados, utilizando tablas dinámicas. Los requisitos que debia cumplir eran básicos como  incluír variaciones anuales según el período, cálculos de KPIs, añadir gráficos creando un ranking, tablas resumen y filtros interactivos. Por lo anterior, tenía la necesidad de comprender el funcionamiento interno de la herramienta.

### ¿Cómo enfrenté este desafío?

Comencé abordando los conceptos básicos y esenciales, seguido de la creación de mi propio CUBO y métricas en Excel, permitiéndome experimentar y familiarizarme a usar expresiones MDX.  Una vez adquirida esta base, me dediqué a trabajar en la aplicación. (Para ver algunos resultados puedes chequear en mis proyectos).

A continuación, comparto los conceptos principales que considero fundamentales para aquellos que se encuentren ante la misma situación, y en otro artículo exploraré las capacidades que ofrece Excel en este sentido.

#### ¿Qué es un Almacén de Datos?


Un almacén de datos, o almacén de datos empresarial (EDW), es un sistema centralizado que recopila datos de diversas fuentes en un solo lugar 
¿Cual es su propósito? Facilitar el análisis de datos, la minería de datos y la inteligencia artificial. 
Esto permite a una organización ejecutar análisis potentes en grandes volúmenes de datos históricos, que una base de datos estándar o normal no puede.


<br/>

<div class="d-flex justify-content-center"> 
<image class="p-11"  src="/images/portfolio/work4.4.jpg"/>
</div>

</p>

#### ¿Qué es OLAP?

OLAP en ingles **(Online Analytical Processing)** o **Procesamiento Analítico en Línea**, es una tecnología diseñada para realizar análisis multidimensionales a alta velocidad en grandes volúmenes de datos en un almacén de datos. A diferencia del Procesamiento Transaccional en Línea (OLTP), que se centra en transacciones en tiempo real, OLAP está orientado hacia el análisis y la generación de informes. 


### ¿Qué es un esquema multidimensional?
Las bases de datos multidimensionales (MBD) están optimizadas para trabajar en un ambiente de Data Warehouse, se organizan los datos en una estructura de múltiples dimensiones, donde cada una de ella representa un aspecto diferente de los datos, como el tiempo, la ubicación o el producto. Esto significa que las bases de datos multidimensionales se conforman a partir de diversas bases de datos relacionales.


#### Principales Usos de OLAP

1. **Minería de Datos y Inteligencia Empresarial:** OLAP es una herramienta  para extraer conocimientos de grandes conjuntos de datos de diferentes fuentes de información. Facilita la identificación de tendencias, patrones y oportunidades ocultas que pueden impulsar el crecimiento y la eficiencia empresarial.
    
2. **Cálculos Analíticos Complejos:** Desde análisis de tendencias hasta simulaciones nos ayuda a responder la pregunta ¿qué pasaría si...?.
    
3. **Reportes Empresariales:** Ya sea para informes de ventas, marketing, análisis financiero o planificación de presupuestos, OLAP proporciona las herramientas necesarias para generar informes detallados y perspicaces que respalden la toma de decisiones estratégicas.


#### Esquemas de Almacenamiento en OLAP

Existe dos esquemas que tambien se usa Power BI, estos son: Esquema de Estrella y Copo de Nieve. 

<br/>

<div class="d-flex justify-content-center"> 
<image class="p-11"  src="/images/blog/blog-post-3.1.png"/>
</div>

</p>

El **Esquema de Estrella** se caracteriza por una tabla de hechos conectada a varias tablas de dimensiones desnormalizadas, lo que garantiza consultas rápidas. 
<p>

Para profundizar te dejo este link que lo explica detalladamente como lo usa Power BI. [Esquema Estrella en Power BI](https://learn.microsoft.com/es-es/power-bi/guidance/star-schema) 
 
 Por otro lado, el **Esquema de Copo de Nieve** presenta tablas de dimensiones normalizadas, lo que reduce la redundancia de datos pero puede afectar el rendimiento de las consultas.



#### ¿Qué son las Dimensiones en OLAP?

En OLAP, las dimensiones son elementos clave que permiten filtrar, agrupar y etiquetar datos. Similar a las clases en un sistema de gestión, las dimensiones en OLAP contienen una lista de atributos que se asignan a propiedades específicas en una clase. Por ejemplo, una dimensión puede permitir filtrar ventas por tipo de sucursal y agruparlas por región o punto de venta.


#### Relación Cubo OLAP y Excel

El concepto de OLAP se remonta a la década de 1970, cuando el Dr. E.F. Codd, un científico de IBM, que ideó la base de datos relacional. 
A medida que las bases de datos relacionales ganaron popularidad en las décadas siguientes, surgió la necesidad de una solución para generar informes eficientes a partir de estos datos. Es aquí donde entra en juego el cubo OLAP, una innovación que precalcula totales y subtotales necesarios para informes, permitiendo consultas rápidas y eficientes.

¿Cual fue su beneficio? Fue diseñada para tener acceso rápido y eficiente a datos históricos y transaccionales para realizar cálculos analíticos complejos, crear escenarios predictivos y crear informes empresariales. Facilitando la toma de decisiones al proporcionar una visión profunda y contextualizada de los datos. 

Por esta razón, te recomiendo aprovechar al máximo las **funciones CUBO**, ya que consultan rápidamente al modelo de datos mediante expresiones en **MDX (MultiDimensional eXpression)**.

## "Esta fue la verdadera "MAGIA" que me ayudo a comprender cómo usar las expresiones en MDX y poder encarar este desafio."

<p>
Adicionalmente, descubrí que no solo agilizan las consultas en nuestros informes, sino que también posibilitan la creación de plantillas que se actualizan automáticamente con la información más reciente, de manera similar a una tabla dinámica, lo cual marca una diferencia significativa en la eficiencia y flexibilidad al realizar una implementación.

#### Otras Referencias

Para los Data Enginier y Cientificos de Datos que se interesa más por la infraestructura y procesamiento de los datos, recomiendo este super artículo bien explicado, es mucho más técnico, las credenciales se las destaco a mi amigo Alejandro Loredo quien me dio luces para entender cómo funciona el Data Warehouse o llamado tambien un Sistema de Soporte de Decisiones (DSS). ([haz click aqui](https://www.linkedin.com/pulse/data-warehouse-series-3-dimensional-modeling-olap-cube-loredo-x48lf/?trackingId=TjOm1EEtpJwajk2rBGMtOg%3D%3D)) 

Para los que quieren aprender más, te dejo estos videos en español:  

[Cubos OLAP y sus operaciones](https://www.youtube.com/watch?v=0MM7zesKh74)

[OLAP en Excel](https://www.youtube.com/watch?v=pVbaSHlo1RA)

[!Funciones de cubo BIEN EXPLICADAS!](https://www.youtube.com/watch?v=uXEPLun9QQI)

[Documentación de Microsoft](https://learn.microsoft.com/es-es/system-center/scsm/olap-cubes-overview?view=sc-sm-2022)


Espero que sea de gran utilidad y recuerdá:

### "No estudio por saber más, sino por ignorar menos."
Sor Juana Inés de la Cruz


Abrazos!


###
---
title: "Macro de Actualización masiva escrita en VBA."
description: "¡Un desafío superado!"
draft: false
image : "images/portfolio/work3.1.jpg"
bg_image: "images/feature-bg.jpg"
category: [ "Automatización" ]
information:
  - label : "Titulo"
    info : "Macro VBA"
  - label : "Lo que hice"
    info : "Implementación Macro en Excel"
  - label : "Herramientas utilizadas"
    info : "Excel | VBA "
  - label : "Completado"
    info : "1 Marzo 2024"
  - label : "Skills"
    info : "Programación | Resolución de Problemas"
  # - label : "Ver Video"
  #   info : "https://youtu.be/TAr9FoDpJj0"
---

## Desafio

Se requiere realizar una actualización masiva desde un archivo Excel principal, donde contiene la tablas maestras, medidas y modelos de datos, el cual se transfieren los datos a diferentes archivos de excel secundarios que filtran la información con una variable y están distribuidos en distintas rutas o subcarpetas. 
Cada subcarpeta visible solo esta visible para las personas responsables. 
La actualización del  proceso manual dura aproximadamente 50 minutos y el desafio es disminuir el proceso de actualización. 

A continuación muestro la estructura de los directorios.

<br/>
<div class="d-flex justify-content-center"> 
<image class="p-10"  src="/images/portfolio/work3.2.png"/>

</div>

  
<br/><br/>

<br/>

## Descripción 
### Pre- Condiciones:
* El archivo principal debe estar identificado al inicio con la serie de año y período, seguido del nombre fijo.
* Los archivos secundarios de Excel se encuentran en diferentes subcarpetas con el nombre del usuario y comparten la misma serie mencionada anteriormente.
* La macro se implementa en un Excel "externo", el cual no interviene en la actualización principal de los datos del modelo del Excel principal.
* Los archivos de Excel secundarios existirán para cada período.

### Solución:
La macro escrita en VBA recorre las subcarpetas de una carpeta principal (ObjetoCarpeta.SubFolders) y realiza acciones (buscar la carpeta, la serie, abrir, actualizar la información, guardar y cerrar) para cada archivo de Excel de las subcarpetas (ObjetoCarpeta2.Files).


Se crea una función donde se definen las variables principales:
*	Serie: Guarda la respuesta que escribe el usuario que contiene el año y mes en formato "YYMM".
*	ArchAct: Contiene el nombre del archivo final.
*	CarpetaPrincipal As String: Almacena la ruta de la carpeta principal donde se encuentran las subcarpetas.
*	CarpetaSecundaria As String: Almacena la ruta de la carpeta secundaria que contiene varios archivos de Excel con distintos períodos.

<br/>
La ejecución comienza tomando la entrada del usuario. 
Luego, se solicita al usuario a través de InputBox que ingrese la Serie YYMM. 
Se establece una condición donde si la serie está vacía, se termina la ejecución; en caso contrario, la ejecución continúa.
Después, se asigna la ruta donde se encuentra el directorio principal, comenzando así a recorrer las subcarpetas y posteriormente los archivos dentro de cada subcarpeta. 
<br/><br/>
Si encuentra el archivo que tiene la serie, realiza la actualización, guarda la información y una vez recorridas todas las carpetas, finaliza con un mensaje de que ha concluido con éxito.

Para consulta el código lo puedes encontrar aquí el siguiete link: <a href="https://github.com/JazminPineda/cookbook/blob/main/vba/macro_actualizac_tableros.vba">vba/macro_actualizac_tableros.vba </a>

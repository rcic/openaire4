.. _dc.description:

Descripción (MA)
================

``dc.description``

Definición y alcance del campo
------------------------------
Información general o específica del recurso utilizada para la descripción textual. En la descripción se puede incluir resumen, tabla de contenido, representación gráfica

Cuando un recurso consta de varios recursos o anexos en URL, no se debe utilizar este campo para enumerar estos recursos.  

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio si es aplicable (MA)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R)

Campo con esquema de metadatos
------------------------------
dc.description 

Traducción al español
---------------------
Descripción 

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar la descripción del recurso:

- **dc.description:** Descripción general del recurso.

- **dc.description.abstract:** Describe el alcance de los contenidos, puede ser un sumario, un resumen, una reseña, una anotación o una frase que describe el recurso. Si la información es tomada textualmente del recurso, se ingresa de la siguiente forma. 

Ej: En la presente edición, producto del trabajo colectivo del programa, han sido sometidos a la metodología de validación científica TRAMIL, 399 usos significativos de partes de 130 especies reportadas en 11.004 encuestas etnofarmacológicas, llevadas a cabo en 64 comunidades incluyendo la mayor parte de los países de la cuenca del Caribe. De los usos sometidos a validación, 393 han sido clasificados en la categoría REC y 6 en TOX. Además, se han realizado 529 ensayos de laboratorio: fitoquímicos (49), de actividad biológica (213) y evaluación de toxicidad (267). Más del 90% de estos ensayos se han realizado en laboratorios universitarios de los países participantes de la cuenca del Caribe. (Apartes del texto)


Valores permitidos (Vocabularios Controlados)
---------------------------------------------
Description

Relaciones con otros campos
---------------------------

Restricciones
-------------

Ejemplos
--------

.. code-block:: xml
   :linenos:

   <dc.description abstract>
      Aislamiento y purificación de compuestos; Actividad antileishmanial a partir de Cordia dentada Poir; Heliotropium indicum; etc.
   </dc.description abstract>

   <dc.description abstract xml:lang="en-US">
     En la presente edición, producto del trabajo colectivo del programa, han sido sometidos a la metodología de validación científica TRAMIL, 399 usos significativos de partes de 130 especies reportadas en 11.004 encuestas etnofarmacológicas, llevadas a cabo en 64 comunidades incluyendo la mayor parte de los países de la cuenca del Caribe. De los usos sometidos a validación, 393 han sido clasificados en la categoría REC y 6 en TOX. Además, se han realizado 529 ensayos de laboratorio: fitoquímicos (49), de actividad biológica (213) y evaluación de toxicidad (267). Más del 90% de estos ensayos se han realizado en laboratorios universitarios de los países participantes de la cuenca del Caribe.
   </dc.description abstract>

.. _DRIVER Guidelines v2 element description: https://wiki.surfnet.nl/display/DRIVERguidelines/Description

Atributos de Campo
------------------
xml:lang → se utiliza este atributo para indicar el idioma de la descripción.

Especificadores de campo
------------------------

- dc.description.abstract

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear los siguientes campos en Dspace:

- dc.description 
- dc.description.abstract

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

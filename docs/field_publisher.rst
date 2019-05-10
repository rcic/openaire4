.. _dc.publisher:

Editor (MA)
===========

``dc.publisher``

Definición y alcance del campo
------------------------------
Entidad responsable de hacer que el recurso esté disponible. Los editores pueden ser personas, organizaciones o servicios. 

No confundir con colaborador (MA) y creador (M). En la mayoría de los casos el colaborador y el editor no son los mismos. 

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio cuando sea aplicable (MA)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible ( R)

Campo con esquema de metadatos
------------------------------
dc.publisher

Traducción al español
---------------------
Editor

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar el editor:

- **dc.publisher:** Nombre del editor, distribuidor, etc. Ej: Metabiblioteca. Si hay más de dos editores se registra en un nuevo campo.

Valores permitidos (Vocabularios Controlados)
---------------------------------------------
No aplica

Relaciones con otros campos
---------------------------

Restricciones
-------------


Ejemplos
--------

.. code-block:: xml
   :linenos:

   <dc.publisher>
     Universidad Nacional de Colombia. Departamento de Investigaciones.
   </dc.publisher>
   <dc.publisher>John Campos. (US)</dc.publisher>

.. _DRIVER Guidelines v2 element publisher: https://wiki.surfnet.nl/display/DRIVERguidelines/Publisher

Atributos de campo
------------------
No aplica

Especificadores de campo
------------------------

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear en Dspace los siguientes campos:

- dc.publisher

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------
OpenAIRE 3: dc.publisher
.. _dci:identifier:

Identificador de recursos (M)
=============================

``datacite:identifier``

Definición y alcance del campo
------------------------------
Es la cadena única para identificar el recurso. Los sistemas de identificación de recursos más comunes son:

- URI
- URL
- DOI
- PURL
- HANDLE

El uso de este campo es para ingresar un acceso directo al recurso digital.

No confundir con Identificador alternativo (R), Identificador relacionado (R), Ubicación del archivo (MA) y Fuente (R).

Niveles de requerimientos (M/MA/R/O)
-------------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
No repetible (NR)

Campo con esquema de metadatos
------------------------------
datacite:identifier

Traducción al español
---------------------
Identificador de recursos

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
---------------------------------------------
Identifier type

Relaciones con otros campos
---------------------------

Restricciones
-------------


Ejemplos
--------

.. code-block:: xml
   :linenos:

   <datacite:identifier identifierType="Handle">http://hdl.handle.net/1234/5628</datacite:identifier>

Atributos de campo 
------------------
Valores controlados  permitidos:

- ARCA
- DOI
- Encargarse de
- PUNTILLA
- URL
- URNA

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

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

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

También hace referencia el número de identificación del proyecto ante los entes financiadores. 

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

Revise la forma adecuada para ingresar el identificador del recurso:

- **datacite:identifier:** Ingrese alguno de los siguientes identificadores normalizados:
		- URI
		- URL
		- DOI
		- PURL
		- HANDLE

- **datacite:identifier-projectid:** Se debe ingresar el número de identificación del proyecto establecido por la institución. Ej: 1101-586-35778.


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

   <datacite:identifier-projectid>3454-102-001-86</<datacite:identifier-projectid>

Atributos de campo 
------------------
Valores controlados  permitidos:

- ARCA
- DOI
- Encargarse de
- PUNTILLA
- URL
- URNA
- PROJECT

Especificadores de campo
------------------------

- datacite:identifier-projectid

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

- datacite:identifier
- datacite:identifier-projectid

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear los siguientes campos en Dspace:

- datacite:identifier
- datacite:identifier-projectid

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

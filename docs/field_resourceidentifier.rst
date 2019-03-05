.. _dci:identifier:

Identificador de recursos (M)
=============================

``datacite:identifier``

Nombre del campo
----------------

Campo normalizado:
~~~~~~~~~~~~~~~~~~
identifier

Campo con esquema de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
datacite:identifier

Traducción al español:
~~~~~~~~~~~~~~~~~~~~~~
Identificador de recursos

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de Ocurrencia (R/NR - Cantidad Veces)
---------------------------------------------
No repetible (NR)

Definición y Alcance del campo
------------------------------
Es la cadena única para identificar el recurso. Los sistemas de identificación de recursos más comunes son: 
URI
URL
DOI
PURL
HANDLE

El uso de este campo es para ingresar un acceso directo al recurso digital.

Forma de Descripción Normalizada (RDA/RCAAA/..)
-----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Identifier type

Relaciones con otros campos
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Restricciones
~~~~~~~~~~~~~

Ejemplos
~~~~~~~~

.. code-block:: xml
   :linenos:

   <datacite:identifier identifierType="Handle">http://hdl.handle.net/1234/5628</datacite:identifier>

Atributos de Campo
------------------

Valores controlados  permitidos:
- ARCA
- DOI
- Encargarse de
- PUNTILLA
- URL
- URNA


Especificadores de Campo
------------------------

Niveles de Aplicación - Productos de Colciencias
------------------------------------------------
Se aplica a todos los productos de Colciencias.

Observaciones del Campo
-----------------------
No confundir con Identificador alternativo (R ), Identificador relacionado (R ), Ubicación del archivo (MA) y Fuente (R ).

Adaptado de
~~~~~~~~~~~

Relaciones con otros modelos de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Niveles Semánticos
~~~~~~~~~~~~~~~~~~

Recomendación de Campos de aplicación en DSPACE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LAREFERENCIA, OPENAIRE2, OPENAIRE3)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Otras Observaciones
~~~~~~~~~~~~~~~~~~~

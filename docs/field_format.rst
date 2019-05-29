.. _dc.format:

Format (Formato) (R)
====================

``dc.format``


Definición y alcance del campo
------------------------------
Hace referencia a la manifestación física o digital del recurso, se puede incluir el medio del recurso. El formato es una guía para el usuario que le permite determinar el software o hardware necesario para operar el recurso. 

No confundir con el tipo de recurso (M) y el identificador del recurso (M).

Niveles de persistencia (M/MA/R/O)
-----------------------------------
Recomendado (R)

Niveles de ocurrencia (R / NR)
------------------------------
No repetible (NR)

Esquema de metadatos
--------------------
dc:format

Traducción al español
---------------------
Formato

Forma de Descripción Normalizada (RDA / RCAA2/ ISBD)
----------------------------------------------------
RDA (Recursos: descripción y acceso)

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Relaciones con otros campos
---------------------------

Restricciones
-------------

Ejemplos y ayudas
------------------

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc.format>video/quicktime</dc.format>
   <dc.format>application/pdf</dc.format>
   <dc.format>application/xml</dc.format>
   <dc.format>application/xhtml+xml</dc.format>
   <dc.format>application/html</dc.format>
   <dc.format>application/vnd.oasis.opendocument.text</dc.format>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

**Esquema xoai**

.. code-block:: xml
   :linenos:

**Esquema xoai**

.. code-block:: xml
   :linenos:


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

- dc:format
- dc:format.mimetype


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

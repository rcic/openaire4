.. _dci:datePublication:

Fecha de publicación (M)
========================

``datacite:date``

Definición y alcance del campo
-------------------------------
Fecha asociada a la creación del recurso. 

La mejor práctica es codificar el valor de la fecha con el perfil que define ISO 8601 [W3CDTF] con formato YYYY-MM-DD

Campo con esquema de metadatos
------------------------------
datacite:date

Traducción al español
---------------------
Fecha de publicación 

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R)

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
---------------------------------------------
Data type

Relaciones con otros campos
---------------------------

Restricciones
-------------

Ejemplos
--------

.. code-block:: xml
   :linenos:

   <datacite:date dateType="Issued">2010-12-25</datacite:date>

.. _DRIVER Guidelines v2 element date: https://wiki.surfnet.nl/display/DRIVERguidelines/Date
.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

Atributos de campo
------------------
Data type

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
OpenAIRE 3: dc.date 
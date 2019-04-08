.. _dci:dateEmbargo:

Fecha de Periodo de Embargo (MA)
================================

``datacite:date``

Definición y alcance del campo
------------------------------
Fecha asociada a la disponibilidad del recurso. 

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio cuando sea aplicable (MA)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
No repetible (NR)

Campo con esquema de metadatos
------------------------------
datacite:date

Traducción al español
---------------------
Fecha de periodo de embargo

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
---------------------------------------------
date type 

Relaciones con otros campos
---------------------------
Fecha de finalización de embargo 

Restricciones
-------------

Ejemplos
--------

.. code-block:: xml
   :linenos:

   <datacite:dates>
     <datacite:date dateType="Accepted">2017-11-01</datacite:date>
     <datacite:date dateType="Available">2017-12-01</datacite:date>
   </datacite:dates>


Atributos de campo
------------------
data type

Especificadores de campo
------------------------

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Revistas, artículos, documentos de trabajo.

Relaciones con otros modelos de metadatos
-----------------------------------------
dc.date

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
------------------------------------------------

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------
OpenAIRE 3: dc.date

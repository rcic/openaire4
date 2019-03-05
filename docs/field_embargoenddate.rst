.. _dci:dateEmbargo:

Fecha de Periodo de Embargo (MA)
================================

``datacite:date``

Nombre del campo
----------------

Campo normalizado
~~~~~~~~~~~~~~~~~
date

Campo con esquema de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
datacite:date

Traducción al español:
~~~~~~~~~~~~~~~~~~~~~~
Fecha de periodo de embargo

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio cuando sea aplicable (MA)

Niveles de Ocurrencia (R/NR - Cantidad Veces)
---------------------------------------------
No repetible (NR)

Definición y Alcance del campo
------------------------------
Fecha asociada a la disponibilidad del recurso. 

Forma de Descripción Normalizada (RDA/RCAA2)
---------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
date type

Relaciones con otros campos
~~~~~~~~~~~~~~~~~~~~~~~~~~~
Fecha de finalización de embargo

Restricciones
~~~~~~~~~~~~~

Ejemplos
~~~~~~~~

.. code-block:: xml
   :linenos:

   <datacite:dates>
     <datacite:date dateType="Accepted">2017-11-01</datacite:date>
     <datacite:date dateType="Available">2017-12-01</datacite:date>
   </datacite:dates>


Atributos de Campo
------------------
data type

Especificadores de Campo
------------------------


Niveles de Aplicación - Productos de Colciencias
------------------------------------------------
Revistas, artículos, documentos de trabajo.

Observaciones del Campo
-----------------------

Adaptado de..
~~~~~~~~~~~~~

Relaciones con otros modelos de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Niveles Semánticos
~~~~~~~~~~~~~~~~~~

Recomendación de Campos de aplicación en DSPACE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LAREFERENCIA, OPENAIRE2, OPENAIRE3)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
OpenAIRE 3: dc:date

Otras Observaciones
~~~~~~~~~~~~~~~~~~~

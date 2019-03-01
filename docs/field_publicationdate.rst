.. _dci:datePublication:

Fecha de publicación (M)
========================

``datacite:date``

Nombre del campo
----------------

Campo normalizado:
~~~~~~~~~~~~~~~~~~
date

Campo con esquema de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
datacite:date

Traducción al español:
~~~~~~~~~~~~~~~~~~~~~~
Fecha de publicación

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de Ocurrencia (R/NR - Cantidad Veces)
---------------------------------------------
Repetible (R)

Definición y Alcance del campo
------------------------------
Fecha asociada a la creación del recurso. 

Forma de Descripción Normalizada (RDA/RCAA2/)
-----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Data type

Relaciones con otros campos
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Restricciones
~~~~~~~~~~~~~

Ejemplos
~~~~~~~~

.. code-block:: xml
   :linenos:

   <datacite:date dateType="Issued">2000-12-25</datacite:date>

.. _DRIVER Guidelines v2 element date: https://wiki.surfnet.nl/display/DRIVERguidelines/Date
.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

Atributos de Campo
------------------
Data type

Especificadores de Campo
------------------------

Niveles de Aplicación - Productos de Colciencias
------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Observaciones del Campo
-----------------------
La mejor práctica es codificar el valor de la fecha con el perfil que define ISO 8601 [W3CDTF] con formato YYYY-MM-DD

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


.. _DRIVER Guidelines v2 element date: https://wiki.surfnet.nl/display/DRIVERguidelines/Date
.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
.. _dc:format:

Formato (R)
===========

``dc:format``

Nombre del campo
----------------

Campo normalizado:
~~~~~~~~~~~~~~~~~~
format

Campo con esquema de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
dc:format

Traducción al español:
~~~~~~~~~~~~~~~~~~~~~~
Formato

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Recomendado (R)

Niveles de Ocurrencia (R/NR - Cantidad Veces)
---------------------------------------------
No repetible (NR)

Definición y Alcance del campo
------------------------------
Hace referencia a la manifestación física o digital del recurso, se puede incluir el medio del recurso. El formato es una guía para el usuario que le permite determinar el software o hardware necesario para operar el recurso. 

Forma de Descripción Normalizada (RDA/RCAA2)
-----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Format

Relaciones con otros campos
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Restricciones
~~~~~~~~~~~~~

Ejemplos
~~~~~~~~

.. code-block:: xml
   :linenos:

   <dc:format>video/quicktime</dc:format>
   <dc:format>application/pdf</dc:format>
   <dc:format>application/xml</dc:format>
   <dc:format>application/xhtml+xml</dc:format>
   <dc:format>application/html</dc:format>
   <dc:format>application/vnd.oasis.opendocument.text</dc:format>

.. _DRIVER Guidelines v2 element format: https://wiki.surfnet.nl/display/DRIVERguidelines/Format


Atributos de Campo
------------------
De acuerdo con las mejores prácticas, se pueden seleccionar los tipos de medio de la siguiente lista: http://www.iana.org/assignments/media-types/media-types.xhtml

Especificadores de Campo
------------------------

Niveles de Aplicación - Productos de Colciencias
------------------------------------------------
Se aplica a todos los productos de Colciencias.

Observaciones del Campo
-----------------------
No confundir con el tipo de recurso (M) y el identificador del recurso (M).

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

.. _DRIVER Guidelines v2 element format: https://wiki.surfnet.nl/display/DRIVERguidelines/Format
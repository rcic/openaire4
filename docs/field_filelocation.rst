.. _aire:file:

Ubicación del archivo (MA)
==========================

``oaire:file``

Nombre del campo
----------------

Campo normalizado:
~~~~~~~~~~~~~~~~~~
file

Campo con esquema de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
oaire:file

Traducción al español:
~~~~~~~~~~~~~~~~~~~~~~
Ubicación del archivo

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio si es aplicable (MA)

Niveles de Ocurrencia (R/NR - Cantidad Veces)
---------------------------------------------
No repetible (NR)

Definición y Alcance del campo
------------------------------
Hace referencia a la ubicación de un archivo que está asociado al recurso. 

Forma de Descripción Normalizada (RDA/RCAA2)
--------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
oaire:file

Relaciones con otros campos
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Restricciones
~~~~~~~~~~~~~

Ejemplos
~~~~~~~~

.. code-block:: xml
   :linenos:

   <oaire:file accessRightsURI="http://purl.org/coar/access_right/c_abf2" mimeType="application/pdf" objectType="fulltext">http://link-to-the-fulltext.org</oaire:file>

.. _COAR Access Right Vocabulary: http://vocabularies.coar-repositories.org/documentation/access_rights/

Atributos de Campo
------------------
Use los términos del vocabulario controlado:

+------------------------------------------+---------------------+
| ConceptURI                               | Etiqueta            |
+==========================================+=====================+
| http://purl.org/coar/access_right/c_abf2 | open access         |
+------------------------------------------+---------------------+
| http://purl.org/coar/access_right/c_f1cf | embargoed access    |
+------------------------------------------+---------------------+
| http://purl.org/coar/access_right/c_16ec | restricted access   |
+------------------------------------------+---------------------+
| http://purl.org/coar/access_right/c_14cb | metadata only access|
+------------------------------------------+---------------------+

Especifique el el formato del archivo, se recomienda seleccionar los tributos de tipo de medio: http://www.iana.org/assignments/media-types 

Para el tipo de objeto, seleccione los siguientes atributos de la lista controlada:

- fulltext
- dataset
- software
- other

Especificadores de Campo
------------------------

Niveles de Aplicación - Productos de Colciencias
------------------------------------------------
Se aplica a todos los productos de Colciencias. 

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

Otras Observaciones
~~~~~~~~~~~~~~~~~~~

.. _COAR Access Right Vocabulary: http://vocabularies.coar-repositories.org/documentation/access_rights/
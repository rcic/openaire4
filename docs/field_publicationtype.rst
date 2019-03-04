.. _aire:resourceType:

Tipo de recurso (M) 
===================

``oaire:resourceType``

Nombre del campo
----------------

Campo normalizado:
~~~~~~~~~~~~~~~~~~
resource type

Campo con esquema de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
oaire:resourcetype

Traducción al español:
~~~~~~~~~~~~~~~~~~~~~~
Tipo de recurso

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de Ocurrencia (R/NR - Cantidad Veces)
---------------------------------------------
No repetible (NR)

Definición y Alcance del campo
------------------------------
Hace referencia al tipo de producción científica o contenido intelectual en el que se manifiesta el recurso. Y es utilizado por el usuario para identificar el recurso que está buscando. Ejemplo: Libro, artículo, revista, etc. 

Forma de Descripción Normalizada (RDA/RCAA2)
-----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Ver vocabularios
http://vocabularies.coar-repositories.org/documentation/resource_types/

Relaciones con otros campos
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Restricciones
~~~~~~~~~~~~~

Ejemplos
~~~~~~~~

.. code-block:: xml
   :linenos:

   <oaire:resourceType resourceTypeGeneral="literature" uri="http://purl.org/coar/resource_type/c_6501">journal article</oaire:resourceType>

.. _COAR Resource Type Vocabulary: http://vocabularies.coar-repositories.org/documentation/resource_types/


Atributos de Campo
------------------

+-----------------------------------------------+-------------------------+
| ConceptURI		                              | Etiqueta		           |
+===============================================+=========================+
| http://purl.org/coar/resource_type/c_1162     | annotation              |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_6501     | journal article         |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_545b     | letter to the editor    |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_b239     | editorial               |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_2df8fbb1 | research article        |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_dcae04bc | review article          |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_beb9     | data paper              |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_3e5a     | contribution to journal |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_ba08     | book review             |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_3248     | book part               |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_2f33     | book                    |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_86bc     | bibliography            |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_816b     | preprint                |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_8042     | working paper           |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_71bd     | technical documentation |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18gh     | technical report        |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18ws     | research report         |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18hj     | report to funding agency|
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18op     | project deliverable     |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_186u     | policy report           |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18wq     | other type of report    |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18wz     | memorandum              |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18ww     | internal report         |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_efa0     | review                  |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_baaf     | research proposal       |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_ba1f     | report part             |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_93fc     | report                  |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_15cd     | patent                  |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18co     | conference poster not   |
|						                              | in proceedings          |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18cp     | conference paper not    |
|                                               | in proceedings          |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_6670     | conference poster       |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_5794     | conference paper        |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_c94f     | conference object       |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_f744     | conference proceedings  |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_7a1f     | bachelor thesis         |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_bdcc     | master thesis           |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_db06     | doctoral thesis         |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_46ec     | thesis                  |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_0857     | letter                  |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_8544     | lecture                 |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18cf     | text                    |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18cw     | musical notation        |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18cd     | musical composition     |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18cc     | sound                   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_12ce     | video                   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_8a7e     | moving image            |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_ecc8     | still image             |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_c513     | image                   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_12cd     | map                     |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_12cc     | cartographic material   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_5ce6     | software                |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_ddb1     | dataset                 | 
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_e9a0     | interactive resource    |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_7ad9     | website                 |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_393c     | workflow                |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_1843     | other                   |
+-----------------------------------------------+-------------------------+

Especificadores de Campo
------------------------

Niveles de Aplicación - Productos de Colciencias
------------------------------------------------
Se aplica a todos los productos de Colciencias.

Observaciones del Campo
-----------------------
No confundir con el campo Formato (R ), porque hace referencia al tipo de medio en el que está el recurso. 

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

.. _COAR Resource Type Vocabulary: http://vocabularies.coar-repositories.org/documentation/resource_types/
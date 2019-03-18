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
| ConceptURI                                    | Etiqueta                |
+===============================================+=========================+
| http://purl.org/coar/resource_type/c_1162     | Anotación               |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_6501     | Artículo de revista     |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_545b     | Carta al editor         |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_b239     | Editorial               |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_2df8fbb1 | Artículo de             |
|                                               | investigación           |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_dcae04bc | Artículo de revisión    |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_beb9     | Papel de datos          |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_3e5a     | Contribución a la       |
|                                               | revista                 |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_ba08     | Reseña de libro         |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_3248     | Parte de libro          |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_2f33     | Libro                   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_86bc     | Bibliografía            |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_816b     | Preimpresión            |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_8042     | Documento de trabajo    |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_71bd     | Documentación técnica   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18gh     | Reporte técnico         |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18ws     | Informe de investigación|
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18hj     | Informe agencia de      |
|                                               | financiamiento          |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18op     | Entregable de proyecto  |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_186u     | Informe de política     |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18wq     | Otro tipo de informe    |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18wz     | Memorando               |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18ww     | Informe interno         |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_efa0     | Revisión                |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_baaf     | Propuesta de            |
|                                               | investigación           |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_ba1f     | Parte del informe       |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_93fc     | Informe                 |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_15cd     | Patente                 |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18co     | Documento de conferencia|
|                                               | en proceso              |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18cp     | Documento de conferencia|
|                                               | en no proceso           |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_6670     | Póster de la conferencia|
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_5794     | Documento de sesión     |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_c94f     | Objeto de conferencia   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_f744     | Actas de conferencia    |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_7a1f     | Tesis de licenciatura   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_bdcc     | Tesis de maestría       |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_db06     | Tesis doctoral          |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_46ec     | Tesis                   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_0857     | Carta                   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_8544     | Conferencia             |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18cf     | Texto                   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18cw     | Notación musical        |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18cd     | Composición musical     |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_18cc     | Sonido                  |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_12ce     | Video                   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_8a7e     | Imagen en movimiento    |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_ecc8     | Imagen fija             |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_c513     | Imagen                  |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_12cd     | Mapa                    |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_12cc     | Material cartográfico   |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_5ce6     | Software                |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_ddb1     | Conjunto de datos       |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_e9a0     | Recurso interactivo     |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_7ad9     | Sitio web               |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_393c     | Flujo de trabajo        |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/resource_type/c_1843     | Otro                    |
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
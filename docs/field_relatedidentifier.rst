.. _dci:relatedIdentifier:

Identificador relacionado (R)
=============================

``datacite:relatedIdentifier``

Nombre del campo
----------------

Campo normalizado:
~~~~~~~~~~~~~~~~~~
relatedIdentifier

Campo con esquema de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
datacite: relatedIdentifier

Traducción al español:
~~~~~~~~~~~~~~~~~~~~~~
Identificador Relacionado

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Recomendado (R)

Niveles de Ocurrencia (R/NR - Cantidad Veces)
---------------------------------------------
Repetible (R)

Definición y Alcance del campo
------------------------------

Forma de Descripción Normalizada (RDA/RCAA2)
-----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
relatedIdentifier type
relation type
resourcetype general

Relaciones con otros campos
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Restricciones
~~~~~~~~~~~~~

Ejemplos
~~~~~~~~
ark: Clave de recursos de archivo
arxiv: identificador arXiv.org
bibcode: Códigos bibliográficos del Sistema de Datos Astrofísicos; bibcodes se pueden resolver a través de http://adsabs.harvard.edu/abs/bibcode
doi: Identificador de Objeto Digital
isgn: Número de muestra internacional de Geo; un código alfanumérico de 9 dígitos que identifica de forma exclusiva muestras de nuestro entorno natural y características de muestreo relacionadas.
isbn: Número Internacional Estandarizado para Libros 
issn: Número de serie estándar internacional; un número único de 8 dígitos que se utiliza para identificar una publicación periódica impresa o electrónica.
pmid: ID de PubMed
purl: Localizador de recursos uniforme y persistente
url: Localizador uniforme de recursos 
urn: Nombre del recurso uniforme
wos: Número de acceso a la Web of Science

.. code-block:: xml
   :linenos:

   <datacite:relatedIdentifiers>
      <datacite:relatedIdentifier relatedIdentifierType="URL" relationType="HasPart">http://someUrl</datacite:relatedIdentifier>
   </datacite:relatedIdentifiers>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

Atributos de Campo
------------------
alternateIdentifier type

Especificadores de Campo
------------------------

Niveles de Aplicación - Productos de Colciencias
------------------------------------------------
Aplica para libros, revistas, artículos, documentos de trabajo, proyectos de investigación, norma técnica, proyecto de ley.

Observaciones del Campo
-----------------------

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
OpenAIRE 3: dc:relation

Otras Observaciones
~~~~~~~~~~~~~~~~~~~

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
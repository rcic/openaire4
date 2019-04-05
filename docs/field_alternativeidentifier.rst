.. _dci:alternativeIdentifier:

Identificador alternativo (R)
=============================

``datacite:alternateIdentifier``

Definición y alcance del campo
------------------------------
Es un código local, nacional o internacional que se le otorga al recurso, puede ser una cadena alfanumérica para identificar su ubicación o puede ser un código normalizado según el tipo de recurso. 

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Recomendado (R)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R)

Campo con esquema de metadatos
------------------------------
datacite:alternateIdentifier

Traducción al español
---------------------
Identificador Alternativo

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
---------------------------------------------
alternateIdentifier

Relaciones con otros campos
---------------------------

Restricciones
-------------

Ejemplos
--------
- **ark:** Clave de recursos de archivo
- **arxiv:** identificador arXiv.org
- **doi:** Identificador de Objeto Digital
- **isbn:** Número Internacional Estandarizado para Libros 
- **pissn:** Número de serie estándar internacional (versión impresa)
- **eissn:** Número de serie estándar internacional (versión electrónica)
- **pmid:** ID de PubMed
- **purl:** Localizador de recursos uniforme y persistente
- **urn:** Nombre del recurso uniforme
- **wos:** Número de acceso a la Web of Science

.. code-block:: xml
   :linenos:

   <datacite:alternateIdentifiers>
      <datacite:alternateIdentifier alternateIdentifierType="URL">http://someUrl</datacite:alternateIdentifier>
   </datacite:alternateIdentifiers>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

Atributos de Campo
------------------
alternateIdentifier type

Especificadores de campo
------------------------

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Aplica para libros, revistas, artículos, documentos de trabajo, proyectos de investigación, norma técnica, proyecto de ley.

Relaciones con otros modelos de metadatos
-----------------------------------------
dc.identifier

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------
OpenAIRE 3: dc:relation

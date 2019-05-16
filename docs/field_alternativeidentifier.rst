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

Revise la forma adecuada para ingresar el identificador alternativo con su debida puntuación:

- **datacite:alternateIdentifier-doi:** Hace referencia al identificador del objeto digital. Ej: http://dx.doi.org/10.1145/1067268.1067287

- **datacite:alternateIdentifier-isbn:** Número Internacional Estandarizado para Libros. Se recomienda diligenciar el isbn sin guiones. Ej: 97857821345

- **datacite:alternateIdentifier-pisbn:** Número de serie estándar internacional (versión impresa). Se recomienda diligenciar el pisbn sin guiones. Ej: 101350768

- **datacite:alternateIdentifier-eissn:** Número de serie estándar internacional (versión electrónica). Ej. 4567-7789

- **datacite:alternateIdentifier-pmid:** ID de PubMed. Ej: 235749

- **datacite:alternateIdentifier-purl:** Localizador de recursos uniforme y persistente. Ej: http://purl.oclc.org/OCLC/

- **datacite:alternateIdentifier-urn:** Nombre del recurso uniforme. Son unas cadenas de texto que se usan para nombrar recursos en Internet para su identificación. Ej: urn:isbn:0451450523

- **datacite:alternateIdentifier-wos:** Número de acceso a la Web of Science. Ej:  WOS:000465252900002

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

- datacite:alternateIdentifier
- datacite:alternateIdentifier-doi
- datacite:alternateIdentifier-isbn
- datacite:alternateIdentifier-pisbn
- datacite:alternateIdentifier-eissn
- datacite:alternateIdentifier-pmid
- datacite:alternateIdentifier-purl
- datacite:alternateIdentifier-urn
- datacite:alternateIdentifier-wos

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

Se recomienda crear en Dspace los siguientes campos:

- datacite:alternateIdentifier
- datacite:alternateIdentifier-doi
- datacite:alternateIdentifier-isbn
- datacite:alternateIdentifier-pisbn
- datacite:alternateIdentifier-eissn
- datacite:alternateIdentifier-pmid
- datacite:alternateIdentifier-purl
- datacite:alternateIdentifier-urn
- datacite:alternateIdentifier-wos

Si necesita crear otro tipo de identificadores, siga la misma estructura utilizada anteriormente. 


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------
OpenAIRE 3: dc:relation

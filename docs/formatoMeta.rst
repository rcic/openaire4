.. _formatoMeta:

Formato de metadatos
====================

Aunque el modelo de metadatos utilizado de manera predominante hasta el momento ha sido Dublin Core  (modelo de metadatos ha sido desarrollado por la DCMI - Dublin Core Metadata Initiative) en su versión básica (15 Campos), este conjunto de directrices ha tomado en cuenta los siguientes formatos de metadatos con el fin de promover arquitecturas más abiertas que involucren nuevos alcances de campos, nuevas y distintas tipologías documentales que presenten vocabularios especializados para la descripción estandarizada de los recursos bibliográficos:

+-------------------------------------------------------------+------------------------------------------+--------------------------------------------------------------------------+
| Modelo de Metadatos                                         | Codificación REDCOL (espacios de Nombre) | URL Esquema Definición                                                   |
+=============================================================+==========================================+==========================================================================+
| Simple DC XML Schema                                        | dc                                       | http://purl.org/dc/elements/1.1/                                         |
+-------------------------------------------------------------+------------------------------------------+--------------------------------------------------------------------------+
| DCMI Metadata Terms Schema                                  | dcterms                                  | http://purl.org/dc/terms/                                                |
+-------------------------------------------------------------+------------------------------------------+--------------------------------------------------------------------------+
| Learning Object Metadata Schema definition (LOM)            | lom                                      | http://standards.ieee.org/reading/ieee/downloads/LOM/lomv1.0/xsd/lom.xsd |
+-------------------------------------------------------------+------------------------------------------+--------------------------------------------------------------------------+
| Electronic Theses and Dissertation Metadata Schema (ETD-MS) | thesis                                   | http://www.ndltd.org/standards/metadata/etd-ms-v1.1.html                 |
+-------------------------------------------------------------+------------------------------------------+--------------------------------------------------------------------------+
| DataCite Metadata Schema                                    | datacite                                 | https://schema.datacite.org/meta/kernel-4.1/metadata.xsd                 |
+-------------------------------------------------------------+------------------------------------------+--------------------------------------------------------------------------+
| OpenAire Specification Schema                               | oaire                                    | http://namespace.openaire.eu/schema/oaire/                               |
+-------------------------------------------------------------+------------------------------------------+--------------------------------------------------------------------------+


La Red Colombiana de Información Científica espera que los metadatos utilizados los distintos sistemas de información que se adhieran a la iniciativa y se codifiquen siguiendo el formato de metadatos definido en el **“Perfil de la aplicación REDCOL”** que se presenta en este documento.

Para interoperabilidad en sistemas DSPACE, se recomienda crear este conjunto de esquemas de metadatos con sus correspondientes campos:

.. image:: _static/41formatoMet.jpg
   :scale: 80%


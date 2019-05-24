.. _dc.source:

Source (Fuente) (R) 
===================

``dc.source``

Definición y alcance del campo
------------------------------
Hace referencia a un recurso derivado del recurso presente. El recurso fuente puede derivarse en su totalidad o en partes. Lo que se recomienda es hacer referencia al recurso por medio de un identificador.  También está relacionado con las bibliográficas que contiene el recurso. 

Se recomienda utilizar el resultado de los recursos digitalizados de un recurso original físico, de lo contrario, debe utilizarse un campo: dci:relatedIdentifier.

No confundir con Identificador de recursos (M)

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Recomendado (R)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R)

Campo con esquema de metadatos
------------------------------

- dc.source
- dc.source.bibliographicCitation

Traducción al español
---------------------

- Fuente
- Cita Bibliográfica

Forma de Descripción Normalizada (RDA / RCAA2)
-----------------------------------------------
RDA (Recursos: descripción y acceso)

Se recomienda utilizar los siguientes estilos de citación:

- **APA (American Psychological Association):**  Este estilo ya cuenta con seis ediciones y explica cómo se deben presentar artículos científicos: márgenes, fuente, tamaño de letra, uso de color, gráficas, tablas, y citación y referenciación. 

- **ICONTEC:** Estas normas fueron definidas por el comité técnico del Instituto Colombiano de Normas Técnicas y Certificación, el cual es un organismo multinacional de carácter privado, dedicado a la gestión de la calidad en Colombia, Chile, Ecuador, El Salvador, Guatemala, Honduras y Perú.

- **IEEE (Institute of Electrical and Electronics Engineers):** Este estilo de citación es definido por la asociación científica internacional de técnicos e ingenieros dedicados a la estandarización y desarrollo, es el más utilizado en áreas de ingeniería para todo tipo de documentos. 

- **MLA (Modern Language Association):** Es un estilo y formato de citación bibliográfica para revistas, libros y otro tipo de textos académicos. Es utilizado principalmente en áreas de humanidades y artes,​ sobre todo en filosofía, crítica literaria, literatura comparada y en campos interdisciplinarios, como los estudios culturales.

- **VANCOUVER:** Este estilo de citación válidas para todo tipo de documentos específico para las áreas de Ciencias de la Salud.

Valores permitidos (Vocabularios Controlados)
---------------------------------------------

* dc.source
* dc.source.bibliographicCitation

Relaciones con otros campos
---------------------------

Restricciones
-------------

Ejemplos
--------

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc.source>Cuadernos de ecología volumen 4 (2001)</dc.source>

   <dc.source.bibliographicCitation>CEPAL. (2017). Panorama fiscal de américa latina. La movilización de recursos para el financiamiento del desarrollo sostenible </dc.source.bibliographicCitation>

.. _DRIVER Guidelines v2 element source: https://wiki.surfnet.nl/display/DRIVERguidelines/Source

**Esquema DataCite**

.. code-block:: xml
   :linenos:

**Esquema xoai**

.. code-block:: xml
   :linenos:

**Esquema xoai**

.. code-block:: xml
   :linenos:

Atributos de campo 
------------------

Especificadores de campo
------------------------

- dc.source.bibliographicCitation

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear los siguientes campos en Dspace:

- dc.source
- dc.source.bibliographicCitation

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

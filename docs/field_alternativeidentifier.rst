.. _dci:alternativeIdentifier:

Identificador alternativo (R)
=============================

``datacite:alternateIdentifier``

Definición y alcance del campo
------------------------------
Es un código local, nacional o internacional que se le otorga al recurso, puede ser una cadena alfanumérica para identificar su ubicación o puede ser un código normalizado según el tipo de recurso. 

Niveles de persistencia (M/MA/R/O)
------------------------------------
Recomendado (R)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R): **1-n veces**
Repita este campo para colocar  cada uno de los identificadores alternativos necesarios en **orden prioritario.**

Esquema de metadatos
--------------------
datacite:alternateIdentifier
**Nota:** Este campo se ha adaptado del esquema de metadatos DATACITE MetadataKernel versión 4.1 (http://doi.org/10.5438/0014), el cual es utilizado ampliamente para la gestión de documentos y datos. 

Traducción al español
---------------------
Identificador alternativo, código alternativo

Forma de Descripción Normalizada (RDA / RCAA2 / ISBD)
-----------------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar el identificador alternativo con su debida puntuación:

- Para el ingreso de ISBN no incluya guiones (-).
- Para el caso del PURL, coloque la URL completa.


Propiedades, atributos y especificadores de campo
-------------------------------------------------

**Propiedad del Identificador Alternativo (alternateIdentifier) (R, 0-1):** Esta propiedad permite especificar el valor del identificador alternativo que se le ha otorgado al recurso.

	**Atributo: Tipo de identificador alternativo (AlternateIdentifier) (M) (O, 0-1):** Este atributo permite especificar el tipo de identificador alternativo que se le ha otorgado al recurso. Se debe tener en cuenta los siguientes tipos de identificadores y su codificación normalizada según el vocabulario controlado propuesto:

.. tabularcolumns:: |\Y{0.15}|\Y{0.7}|\Y{0.15}|

+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| Vocabulario Normalizado | Descripción del Atributo                                                                                                                                                                                                                                                        | Dominio de Vocabulario |
+=========================+=================================================================================================================================================================================================================================================================================+========================+
| ARK                     | Clave de recursos de archivo                                                                                                                                                                                                                                                    | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| arXiv                   | Identificador de https://arxiv.org/                                                                                                                                                                                                                                             | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| bibcode                 | Códigos bibliográficos del Sistema de Datos Astrofísicos; bibcodes se pueden resolver a través de http://adsabs.harvard.edu/abs/bibcode                                                                                                                                         | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| DOI                     | Identificador de Objeto Digital. Código alfanumérico que sirva para identificar de forma única un documento digital.                                                                                                                                                            | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| EAN13                   | Número de artículo europeo, ahora renombrado como Número de artículo internacional, pero que conserva el acrónimo original, es un estándar de código de barras de 13 dígitos que es un superconjunto del sistema del Código de producto universal (UPC) original de 12 dígitos. | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| EISSN                   | Número internacional normalizado de publicaciones seriadas (versión electrónica), permite identificar de manera única una colección seriada evitando posibles errores en la transcripción del título o información bibliográfica.                                               | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| Handle                  | Es un identificador persistente, es decir, un sistema de especificación para nombres e identificación de servicios.                                                                                                                                                             | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| IGSN                    | Número de muestra internacional Geo; un código alfanumérico de 9 dígitos que identifica de forma exclusiva muestras de nuestro entorno natural y funciones de muestreo relacionadas.                                                                                            | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| ISBN                    | Número internacional normalizado de libros, es un identificador único para libros, prevista para su uso comercial.                                                                                                                                                              | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| ISSN                    | Número internacional normalizado de publicaciones seriadas, permite identificar de manera única una colección seriada evitando posibles errores en la transcripción del título o información bibliográfica.                                                                     | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| ISTC                    | Código internacional normalizado de obras textuales, es un identificador único para obras textuales siempre y cuando exista una intención de producir dicha obra en forma de una o más manifestaciones.                                                                         | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| ISSN-L                  | Es un número específico que reúne los diferentes soportes en los que se edita una publicación seriada.                                                                                                                                                                          | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| LSID                    | Es el identificador único de las ciencias naturales, considerándose una especificación en curso del Nombre del Recurso Uniforme (URN) y permite identificar los recursos en diferentes almacenes de datos biológicamente significativos.                                        | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| PISSN                   | Número internacional normalizado de publicaciones seriadas, permite identificar de manera única una colección seriada evitando posibles errores en la transcripción del título o información bibliográfica. (versión impresa)                                                   | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| PMID                    | ID de PubMed. Número único asignado a cada cita de artículo de revistas biomédicas y de las ciencias naturales.                                                                                                                                                                 | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| PURL                    | Localizador de recursos uniforme y persistente, se utiliza para referenciar un determinado recurso que cambia de dirección a lo largo del tiempo desde una misma dirección.                                                                                                     | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| UPC                     | Código de producto universal, es un código de barras utilizado para rastrear artículos comerciales. Su forma más común, la UPC-A, consta de 12 dígitos numéricos.                                                                                                               | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| URL                     | Localizador Uniforme de Recursos, es la dirección específica que se le asigna a cada uno de los recursos disponibles en la red con el fin de localizarlos e identificarlos fácilmente.                                                                                          | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| URN                     | Nombre del recurso uniforme, permite identificar recursos en la web pero no indica exactamente dónde se encuentra el recurso.                                                                                                                                                   | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| WOS                     | Número de acceso a la Web of Science, es una identificación asociada a cada registro del producto, formado por el número de acceso del productor y un número secuencial.                                                                                                        | datacite               |
+-------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+



Relaciones con otros campos
---------------------------
No debe confundirse el Identificador Alternativo **(datacite:alternateIdentifier)** del recurso el identificador relacionado **(datacite:relatedIdentifier)** del mismo.

Restricciones
-------------
No Aplica

Ejemplos y ayudas
-----------------

Ayudas
++++++

- **Identificador Alternativo:** Identificador del recurso, puede ser una cadena alfanumérica que sea única dentro de su dominio o emisión. También pueden utilizarse identificadores locales.

	- Ej: (ISBN): 9788490299029. La edición universitaria en el contexto de la ciencia abierta. 
	- Ej: (PISSN): 0121-7550 (impreso). Revista Nómadas. 
	- Ej: (PURL): http://purl.oclc.org/OCLC/
	- Ej: (WOS): 000465252900002


Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <datacite:alternateIdentifiers>
      <datacite:alternateIdentifier alternateIdentifierType="URL">http://someUrl</datacite:alternateIdentifier>
   </datacite:alternateIdentifiers>

**Esquema xoai**

.. code-block:: xml
   :linenos:

**Esquema xoai**

.. code-block:: xml
   :linenos:


Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Aplica para libros, revistas, artículos, documentos de trabajo, proyectos de investigación, norma técnica, proyecto de ley.

Relaciones con otros modelos de metadatos
-----------------------------------------
El campo Identificador Alternativo (datacite:alternateIdentifier) es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+-------------------------------------------------------------------+
| Esquema de Metadatos | Campo Relacionado                                                 |
+======================+===================================================================+
| dc                   | * dc.identifier.doi                                               |
|                      | * dc.identifier.local                                             |
|                      | * dc.identifier.isbn                                              |
|                      | * dc.identifier.issn                                              |
|                      | * dc.identifier.uri                                               |
|                      | * dc.identifier.url                                               |
|                      | * dc.identifier.other                                             |
+----------------------+-------------------------------------------------------------------+
| marcxml              | field: 050, 052, 055, 061, 071, 072, 080, 082, 084, 086, 088, 090 |
+----------------------+-------------------------------------------------------------------+


Niveles semánticos
------------------

- Este campo contempla la utilización de distintos números internacionales estandarizados para la identificación de un recurso.

- Cada registro presente en estos números internacionales estandarizados un Identificación persistente.

Adicionalmente dichos sistemas proveen una URI única que debe ser enlazada y utilizada en el campo de metadatos asociado.


Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

+----------------------------------------+-----------------------+------------+----------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Cualificar | Nota de alcance      |
+========================================+=======================+============+======================+
| Identificador Alternativo              | identifier            | * doi      | funderIdentifiertype |
|                                        |                       | * local    |                      |
|                                        |                       | * isbn     |                      |
|                                        |                       | * issn     |                      |
|                                        |                       | * uri      |                      |
|                                        |                       | * url      |                      |
|                                        |                       | * other    |                      |
+----------------------------------------+-----------------------+------------+----------------------+


Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------
Se recomienda específicamente crear los nuevos atributos/especificadores del campo de identificador alternativo según la codificación propuesta.
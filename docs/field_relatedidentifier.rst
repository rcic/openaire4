.. _dci:relatedIdentifier:

Related Identifier (Identificador relacionado) (R)
==================================================

``datacite:relatedIdentifier``

Definición y alcance del campo
------------------------------
Este campo contiene uno o varios identificadores de recursos relacionados con el recursos que se está describiendo. Este campo no contiene el Identificador primario del recurso, ni identificadores alternativos del mismo.

Este campo de identificador es utilizado conjuntamente con una propiedad de relación adjunta según corresponda. El uso de este campo es opcional pero recomendada.

Niveles de persistencia (M/MA/R/O)
------------------------------------
Recomendado (R)

Niveles de ocurrencia (R / NR )
-------------------------------
Repetible (R) **0-n veces.**

..

Repita este campo para colocar cada uno de los identificadores relacionados necesarios.

Esquema de metadatos
--------------------
datacite:relatedIdentifier

- **Nota:** Este campo se ha adaptado del esquema de metadatos DATACITE MetadataKernel versión 4.1 (http://doi.org/10.5438/0014), el cual es utilizado ampliamente para la gestión de documentos y datos.

Traducción al español
---------------------
Identificador relacionado 

Forma de Descripción Normalizada (RDA / RCAA2 / ISBD)
-----------------------------------------------------
RDA (Recursos: descripción y acceso)

..

Revise la forma adecuada para ingresar el identificador relacionado con su debida puntuación según el esquema de identificación utilizado.


Propiedades, atributos y especificadores de campo
-------------------------------------------------
 
Propiedad del Identificador Relacionado (relatedIdentifier) (R, 0-n): 
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Esta propiedad permite especificar el valor del identificador relacionado que se le ha otorgado al recurso.

	- **Atributo:** Tipo de identificador relacionado (relatedIdentifierType)  (M, 1 si la propiedad RelatedIdentifier es utilizada): Este atributo permite especificar el tipo de identificador relacionado al recurso. Se debe tener en cuenta los siguientes tipos de identificadores y su codificación normalizada según el vocabulario controlado propuesto: 

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

	- **tributo: Tipo de Relación (relationshipType) (M) (O, 0-1):** Este atributo permite describir la relación del recurso que se está registrando (A) y el recurso relacionado (B). Es obligatorio si se utiliza la propiedad relatedIdentifier. Revise los siguientes valores de la lista controlada:
	
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Vocabulario                 | Traducción                    | Descripción                                                                                                         |                                           |
	+=============================+===============================+=====================================================================================================================+===========================================+
	| Is Cited By                 | Es citado por                 | (indica que B incluye A en una cita)                                                                                |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Cites                       | Cita                          | (indica que A incluye B en una cita)                                                                                |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Supplement To            | Es suplemento a               | (indica que A es un suplemento de B)                                                                                |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Supplemented By          | Es complementado por          | (indica que B es un suplemento a A)                                                                                 |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Continued By             | Es continuado por             | (indica que A es continuado por el trabajo B)                                                                       |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Continues                   | Continúa                      | (indica que A es una continuación del trabajo B)                                                                    |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Described By             | Se describe por               | (indica que A está descrito por B)                                                                                  |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Describes                   | Describe                      | (indica que A describe a B)                                                                                         |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Has Metadata                | Tiene metadatos               | (indica que el recurso A tiene metadatos adicionales B)                                                             |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Metadata For             | Es metadatos para             | (indica metadatos adicionales A para un recurso B)                                                                  |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Has Version                 | Tiene version                 | (indica que A tiene una versión B)                                                                                  |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Version Of               | Es la versión de              | (indica que A es una versión de B)                                                                                  |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is New Version Of           | Es la nueva versión de        | (indica que A es una nueva edición de B, donde la nueva edición se ha modificado o actualizado)                     |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Previous                 | Version Of                    | Es la version anterior de                                                                                           | (indica que A es una edición previa de B) |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Part Of                  | Es parte de                   | (indica que A es una parte de B; puede usarse para elementos de una serie)                                          |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Has Part                    | Tiene parte                   | (indica que A incluye la parte B)                                                                                   |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Referenced By            | Es referenciado por           | (indica que A se usa como fuente de información por B)                                                              |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| References                  | Referencias                   | (Indica que B se usa como fuente de información para A)                                                             |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Documented By            | Es documentado por            | (indica que B es documentación sobre / explicando A)                                                                |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Documents                   | Documentos                    | (indica que A es documentación sobre / explicando B)                                                                |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is CompiledBy               | Es compilado por              | (indica que B se usa para compilar o crear A)                                                                       |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Compiles                    | Compila                       | (indica que B es el resultado de un evento de compilación o creación usando A)                                      |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Variant Form Of          | Es la forma variante de       | (indica que A es una variante o forma diferente de B, por ejemplo, forma calculada o calibrada o empaque diferente) |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Original Form Of         | Es la forma original de       | (indica que A es la forma original de B)                                                                            |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Identical To             | Es identico a                 | (indica que A es idéntico a B, para usar cuando es necesario registrar dos instancias separadas del mismo recurso)  |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Reviewed By              | Es revisado por               | (indica que A es revisado por B)                                                                                    |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Reviews                     | Opiniones                     | (indica que A es una revisión de B)                                                                                 |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Derived From             | Se deriva de                  | (indica que B es una fuente en la que se basa A)                                                                    |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Source Of Is Required By | Es fuente de es requerida por | (indica que A es una fuente en la que B se basa)                                                                    |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Is Required By              | Es requerido por              | (indica que A requiere B)                                                                                           |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+
	| Requires                    | Requiere                      | (indica que A requiere B)                                                                                           |                                           |
	+-----------------------------+-------------------------------+---------------------------------------------------------------------------------------------------------------------+-------------------------------------------+


Relaciones con otros campos
---------------------------
No debe confundirse el Identificador relacionado (datacite:relatedIdentifier) del recurso el identificador alternativo (datacite:alternativeIdentifier) del mismo.

Restricciones
-------------
No aplica


Ejemplos y ayuda
----------------

Ayudas
++++++

- **Identificador Relacionado:** Identificador del recurso, puede ser una cadena alfanumérica que sea única dentro de su dominio o emisión. También pueden utilizarse identificadores locales.

	- Ej: (ISBN): 9788420471839. Cien años de soledad 

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <datacite:relatedIdentifiers>
      <datacite:relatedIdentifier relatedIdentifierType="URL" relationType="HasPart">http://someUrl</datacite:relatedIdentifier>
   </datacite:relatedIdentifiers>

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
El campo Identificador Relacionado (datacite:relatedIdentifier) es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+-------------------------------------------------------------------+
| Esquema de Metadatos | Campo Relacionado                                                 |
+======================+===================================================================+
| dc                   | * dc.identifier.local                                             |
|                      | * dc.identifier.doi                                               |
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
- Cada registro presente en estos números internacionales estandarizados tiene un identificador persistente.

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

+----------------------------------------+-----------------------+------------+-----------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Cualificar | Nota de alcance       |
+========================================+=======================+============+=======================+
| Identificador Relacionado              | dc.identifier         | local      | relatedIdentifierType |
+----------------------------------------+-----------------------+------------+-----------------------+
| DOI                                    | dc.identifier         | doi        |                       |
+----------------------------------------+-----------------------+------------+-----------------------+
| ISBN                                   | dc.identifier         | isbn       |                       |
+----------------------------------------+-----------------------+------------+-----------------------+
| ISSN                                   | dc.identifier         | issn       |                       |
+----------------------------------------+-----------------------+------------+-----------------------+
| HANDLE                                 | dc.identifier         | handle     |                       |
+----------------------------------------+-----------------------+------------+-----------------------+
| URI                                    | dc.identifier         | uri        |                       |
+----------------------------------------+-----------------------+------------+-----------------------+
| URL                                    | dc.identifier         | url        |                       |
+----------------------------------------+-----------------------+------------+-----------------------+
| OTHER                                  | dc.identifier         | other      |                       |
+----------------------------------------+-----------------------+------------+-----------------------+

Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------
Se recomienda específicamente crear los nuevos atributos/especificadores del campo de identificador alternativo según la codificación propuesta.
.. _aire:resourceType:

Resource Type (Tipo de recurso) (M)  
===================================

``oaire:resourceType``

Definición y alcance del campo
------------------------------

Este campo tiene varios usos dependiendo del contexto general de aplicación, los distintos usos se enumeran a continuación:

	- **Tipología Documental Normalizada COAR (M,1):** Hace referencia al tipo de publicación basándose en un vocabulario controlado normalizado, el cual es utilizado por el usuario (una máquina) para identificar la categoría asociada al recurso que está mostrando.

	- **Tipología Documental Normalizada MinCiencias (MA,1):** Hace referencia al tipo de recurso de investigación reconocido y avalado por MinCiencias basándose en un vocabulario controlado normalizado, el cual es utilizado por el usuario (una máquina) para identificar la categoría asociada al recurso que está mostrando.

	- **Tipología Documental Local (R,1):** Hace referencia al tipo de producción científica o contenido intelectual en el que se manifiesta el recurso, el cual es utilizado por el usuario (una persona) para identificar la categoría asociada al recurso que está mostrando.  Ejemplo: Libro, artículo, revista, etc. 

	- **Tipología asociada a la Naturaleza del Contenido del Recurso (O,1):** Hace referencia al tipo de contenido interno sobre el cual está construido el recurso de información (Naturaleza del contenido) basándose en un vocabulario controlado normalizado.

Niveles de persistencia (M/MA/R/O)
------------------------------------

	- Tipología Documental Normalizada COAR: Obligatorio (M,1)
	- Tipología Documental Normalizada MinCiencias: Obligatorio si es aplicable (MA,1)
	- Tipología Documental Local: Recomendado (R,1)
	- Tipología del Contenido del Recurso: Opcional (O,1)


Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R) según los distintos contextos de aplicación de la tipología documental asociada.

Esquema de metadatos
------------------------------
oaire:resourcetype 

Traducción al español
---------------------
Tipo de recurso / Tipología Documental / Tipología del Contenido

Forma de Descripción Normalizada (RDA / RCAA2/ ISBD)
----------------------------------------------------
RDA (Recursos: descripción y acceso)

	Revise la forma adecuada para seleccionar el tipo de recurso:

		- **Tipología Documental Local:** Texto libre. Sin embargo se recomienda utilizar un vocabulario controlado de tipologías documentales. Esta directriz sugiere un vocabulario asociado a este campo. 
		- **Tipología Documental Normalizada COAR:** Se debe seleccionar el tipo de recurso que debe estar debidamente relacionado con una uri definido con el vocabulario controlado de COAR.
		- **Tipología Documental Normalizada RedCol:** Se debe seleccionar el tipo de recurso que debe estar debidamente relacionado con una uri definido con el vocabulario controlado de REDCOL.
		- **Tipología del Contenido del Recurso:** Se debe seleccionar el tipo de contenido del recurso según vocabulario controlado provisto **(resourceTypeGeneral).**

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad Tipo de Recurso (resourceType) (M/MA/O/R, 1-n):
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Utilice la etiqueta del término de tipo de recurso como valor. Utilice el **valor del atributo asociado a la tipología documental que es** utilizado por el **usuario (una persona)** para identificar la categoría que está describiendo. Se puede utilizar la etiqueta en cualquier idioma indicado en el vocabulario.

	- **Atributo: Tipo de Contenido General (resourceTypeGeneral) (MA, 1):** Este atributo permite especificar el tipo de contenido asociado a la tipología documental descrita del recurso de información. Se debe tener en cuenta los siguientes tipos de contenido y su codificación normalizada según el vocabulario controlado propuesto:
	  
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| Vocabulario Normalizado | Descripción del Atributo                                                                                                                                                                                                         | Dominio de Vocabulario |
	+=========================+==================================================================================================================================================================================================================================+========================+
	| Audiovisual             | Contenido Audiovisual/Multimedia. Una serie de representaciones visuales que imparten una impresión de movimiento cuando se muestran en sucesión. Puede o no incluir sonido. En el Vocabulario DC se representa como MovingImage | MovingImage            |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| Collection              | Contenido Colección. Una agregación de recursos, que puede abarcar colecciones de un tipo de recurso así como de tipos mixtos. Una colección se describe como un grupo; Sus partes también se pueden describir por separado.     | Collection             |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| DataPaper               | Contenido Publicación de datos. Una publicación especializada con la intención de identificar y describir datos específicos, conjuntos de datos o recopilaciones de datos para facilitar el descubrimiento.                      | Text                   |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| Dataset                 | Contenido Conjunto de datos. Datos codificados en una estructura definida.                                                                                                                                                       | Dataset                |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| Event                   | Contenido Acontecimiento. Una ocurrencia no persistente, basada en el tiempo.                                                                                                                                                    | Event                  |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| Image                   | Contenido Imagen. Una representación visual que no sea texto. En el vocabulario DC se representa como Image, StillImage                                                                                                          | Image, StillImage      |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| InteractiveResource     | Contenido Recurso interactivo. Un recurso que requiere la interacción del usuario para ser comprendido, ejecutado o experimentado.                                                                                               | InteractiveResource    |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| Model                   | Contenido Modelo. Un modelo abstracto, conceptual, gráfico, matemático o de visualización que representa objetos empíricos, fenómenos o procesos físicos.                                                                        | N/A                    |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| PhysicalObject          | Contenido Objeto físico. Un objeto o sustancia inanimada, tridimensional.                                                                                                                                                        | PhysicalObject         |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| Service                 | Contenido Servicio. Un sistema organizado de aparatos, aparatos, personal, etc., para suministrar algunas funciones requeridas por los usuarios finales.                                                                         | Service                |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| Software                | Contenido Software. Un programa informático en código fuente (texto) o en forma compilada. Utilice este tipo de contenido para todos los componentes de software relacionados.                                                   | Software               |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| Sound                   | Contenido Sonido. Un recurso destinado principalmente a ser escuchado.                                                                                                                                                           | Sound                  |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| Text                    | Contenido Texto. Un recurso formado principalmente por palabras para la lectura.                                                                                                                                                 | Text                   |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| Workflow                | Contenido Flujo de Trabajo. Una serie estructurada de pasos que se pueden ejecutar para producir un resultado final, que permite a los usuarios especificar y ejecutar su trabajo de una manera más reproducible.                | N/A                    |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
	| Other                   | Contenido Otros. Contenido que no se puede describir en los anteriores elementos.                                                                                                                                                | N/A                    |
	+-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+


	- **Atributo: Contexto de la Tipología (resourceTypeContext) (R, 1):** Este atributo permite especificar el contexto de uso de la tipología según los distintos usos y aplicaciones. En el evento que este atributo no sea declarado, se entenderá que la tipología suministrada se describe según vocabulario COAR. Se debe tener en cuenta los siguientes contextos y su codificación normalizada según el vocabulario controlado propuesto:
	
	+-------------------------+-------------------------------------------------------------------+------------------------+
	| Vocabulario Normalizado | Descripción del Atributo                                          | Dominio de Vocabulario |
	+=========================+===================================================================+========================+
	| coar                    | Tipología documental descrita según vocabulario COAR              | redcol                 |
	+-------------------------+-------------------------------------------------------------------+------------------------+
	| redcol                  | Tipología documental descrita según vocabulario REDCOL            | redcol                 |
	+-------------------------+-------------------------------------------------------------------+------------------------+
	| local                   | Tipología documental descrita según vocabulario LOCAL             | redcol                 |
	+-------------------------+-------------------------------------------------------------------+------------------------+
	| other                   | Otra categoría de de tipologías documentales asociadas al recurso | redcol                 |
	+-------------------------+-------------------------------------------------------------------+------------------------+

	- **Atributo: Identificador Uniforme del Recurso (uri) (M, 1):** Este atributo permite especificar un identificador semántico basado en un vocabulario controlado (ontología) para describir de manera unívoca una tipología documental.
	
		- **Tipología Documental Normalizada COAR:** Se debe seleccionar el tipo de recurso que debe estar debidamente relacionado con una uri definida con el vocabulario controlado de COAR:
		
**Vocabulario normalizado de Tipos Documentales OPENAIRE-COAR**

 	    `versión 3.1 <http://vocabularies.coar-repositories.org/documentation/resource_types/>`_. | 2022-09-29 - http://vocabularies.coar-repositories.org/documentation/resource_types

     	    `Versión SKOS-XL  RDF <https://github.com/coar-repositories/vocabularies/tree/master/resource_types>`_.  https://github.com/coar-repositories/vocabularies/tree/master/resource_type



- **Tipología Documental Normalizada RedCol:** Se debe seleccionar el tipo de recurso que debe estar debidamente relacionado con una uri definida con el vocabulario controlado de REDCOL:


	**Productos resultados de actividades de generación de nuevo conocimiento** http://purl.org/co-repo/resource_type/COL_GNC    

	**Productos resultado de actividades de desarrollo tecnológico e innovación** http://purl.org/co-repo/resource_type/COL_DTI

	**Productos resultado de actividades de Apropiación Social del Conocimiento y Divulgación Pública de la Ciencia**  http://purl.org/co-repo/resource_type/COL_ASCDP

	**Productos de actividades relacionadas con la Formación de Recurso Humano para CTeI** http://purl.org/co-repo/resource_type/COL_FRH

	**Productos resultado de la creación o investigación+creación. Provenientes de la Creación en Artes, Arquitectura y Diseño** http://purl.org/co-repo/resource_type/COL_IC


Relaciones con otros campos
---------------------------

- No confundir con el campo Formato (R), porque hace referencia al tipo de medio en el que está el recurso. 

Restricciones
-------------

Ninguna


Ejemplos y ayudas
-----------------

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:type>Trabajo de grado - Pregrado</dc:type>
   <dc:type>Text</dc:type>
   <dc:type>http://purl.org/coar/resource_type/c_7a1f</dc:type>
   <dc:type> http://purl.org/redcol/resource_type/TP</dc:type>


**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <oaire:resourceType resourceTypeGeneral="Text" resourceTypeContext="coar" uri="http://purl.org/coar/resource_type/c_6501">journal article</oaire:resourceType>

**Esquema xaoi**

.. code-block:: xml
   :linenos:

   <element name="type">
   <element name="spa">
     <field name="value">http://purl.org/coar/resource_type/c_7a1f</field>
   </element>
	</element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="type"  qualifier="coar" lang="spa">http://purl.org/coar/resource_type/c_7a1f</dim:field>


Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
**REDCOL** ha desarrollado un vocabulario controlado acorde con los productos de investigación reconocidos y avalados por MinCiencias y que se ciñe a los modelos semánticos provistos por **DATACITE y OPENAIRE.**  

Para describir estos tipos documentales asociados a los productos resultados de investigación reconocidos por MinCiencias, los sistemas de información deben utilizar estos nuevos elementos para describir tipologías documentales propuestas para **REDCOL.**

En el caso que no haya equivalencia en los **vocabularios de los productos documentales de REDCOL** con el **Vocabulario normalizado de Tipos Documentales OPENAIRE-COAR,**  se debe utilizar  en  **COAR** el valor “other - http://purl.org/coar/resource_type/c_1843”  y posteriomente seleccionar el tipo documental específico del vocabulario **REDCOL.**

Para el caso de artículos de revistas científicas, se ha hecho una alineación con las recomendaciones de categorías propuestas y utilizadas por **Publindex** con el fin de describir de manera adecuada las distintas categorías de artículos de revistas.

.. tabularcolumns:: |\Y{0.2}|\Y{0.3}|\Y{0.3}|\Y{0.2}|

+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Publindex                                             | RedCol                                           | OpenAire4                                                                     |
+=======================================================+==================================================+===============================================================================+
| Artículo de investigación científica y tecnológica    |  http://purl.org/redcol/resource\_type/ART       | Artículo de investigación (http://purl.org/coar/resource\_type/c\_2df8fbb1)   |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Artículo de reflexión                                 |  http://purl.org/redcol/resource\_type/ARTREF    | Artículo de revista (http://purl.org/coar/resource\_type/c\_6501)             |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Artículo de revisión                                  |  http://purl.org/redcol/resource\_type/ARTREV    | Artículo de revisión (http://purl.org/coar/resource\_type/c\_dcae04bc)        |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Artículo corto                                        |  http://purl.org/redcol/resource\_type/ARTCORT   | Artículo de diario  (http://purl.org/coar/resource_type/c\_998f )             |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Reporte/Estudio de caso                               |  http://purl.org/redcol/resource\_type/ARTCASO   |                                                                               |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Revisión de tema                                      |  http://purl.org/redcol/resource\_type/ARTREVT   | Revisión de tema (http://purl.org/coar/resource_type/c\_efa0)                 |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Cartas al editor                                      |  http://purl.org/redcol/resource\_type/ARTCAE    | Carta al editor (http://purl.org/coar/resource\_type/c\_545b)                 |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Editorial                                             |  http://purl.org/redcol/resource\_type/ARTEDIT   | Editorial (http://purl.org/coar/resource\_type/c\_b239)                       |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Traducción                                            |  http://purl.org/redcol/resource\_type/ARTTRAD   |                                                                               |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Documento de reflexión no derivado de investigación   |  http://purl.org/redcol/resource\_type/ARTDIV    | Contribución a la revista (Artículo de Divulgación)                           |
|  (Artículo de Divulgación)                            |                                                  | (http://purl.org/coar/resource_type/c\_3e5a)                                  |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Reseña bibliográfica                                  |  http://purl.org/redcol/resource\_type/ARTREB    | Reseña de libro (http://purl.org/coar/resource\_type/c\_ba08)                 |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Fe de erratas                                         |  http://purl.org/redcol/resource\_type/ARTFDE    | Corrigendum (http://purl.org/coar/resource_type/c\_7acd)                      |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Artículo de Sotfware                                  |  http://purl.org/redcol/resource\_type/ARTSOFT   | Artículo de Software (http://purl.org/coar/resource_type/c\_7bab)             |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Artículo de Datos                                     |  http://purl.org/redcol/resource\_type/ARTDATA   | Artículo de Datos (http://purl.org/coar/resource\_type/c\_beb9)               |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+
| Otros                                                 |  http://purl.org/redcol/resource\_type/ARTOTR    | Otro (http://purl.org/coar/resource_type/c\_1843)                             |
+-------------------------------------------------------+--------------------------------------------------+-------------------------------------------------------------------------------+




Relaciones con otros modelos de metadatos
-----------------------------------------
El campo **Tipo de recurso (oaire:resourcetype)** es utilizado por los siguientes esquemas:

+----------------------+-----------------------+
| Esquema de Metadatos | Campo Relacionado     |
+======================+=======================+
| marcxml              | 008 Posición 24       |
+----------------------+-----------------------+
| dc                   | dc.type               |
+----------------------+-----------------------+
| dcterms              | dcterms.type          |
+----------------------+-----------------------+
| datacite             | datacite.resourcetype |
+----------------------+-----------------------+



Niveles semánticos
------------------

Los campos de los atributos de los vocabularios controlados están construidos en skos por la confederación de repositorio de acceso abierto COAR. (https://www.coar-repositories.org/activities/repository-interoperability/coar-vocabularies/)

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:


+---------------------------------------------------+-----------------------+--------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Vocabulario controlado OpenAire/RedCol            | Campo Elemento DSPACE | Calificadores      | Nota de alcance                                                                                                                                                                                                   |
+===================================================+=======================+====================+===================================================================================================================================================================================================================+
| Tipología Documental Normalizada COAR             | dc.type               | coar               | Incluir la URI                                                                                                                                                                                                    |
+---------------------------------------------------+-----------------------+--------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Tipología Documental Normalizada Drive/OpenAireV3 | dc.type               | driver             | Campo Obsoleto, utilizar únicamente con fines de compatibilidad con versiones anteriores                                                                                                                          |
+---------------------------------------------------+-----------------------+--------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Tipología Documental Normalizada RedCol           | dc.type               | *redcol            | Incluir la URI NOTA: Se presenta equivalencia semántica para los campos dc.type.redcol y dc.type.minciencias                                                                                                      |
|                                                   |                       | *minciencias       |                                                                                                                                                                                                                   |
+---------------------------------------------------+-----------------------+--------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Tipología Documental Normalizada Local            | dc.type               | local              | Incluir el Texto para Usuarios. NOTA: Se presenta equivalencia semántica para los campos dc.type y dc.type.local. Para este campo se recomienda utilizar el vocabulario propuesto para tipología documental local |
+---------------------------------------------------+-----------------------+--------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Tipología del Contenido del Recurso               | dc.type               | content            | Utilizar vocabulario controlado                                                                                                                                                                                   |
| Tipo de Contenido General (resourceTypeGeneral)   |                       |                    |                                                                                                                                                                                                                   |
+---------------------------------------------------+-----------------------+--------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

**NOTAS:**

- DSPACE utiliza el campo “dc.type” para hacer visibles/ocultos el despliegue  de algunos campos en función de este primer campo.



Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

- Las versiones anteriores de las Directrices de OpenAIRE y Driver utilizaban el vocabulario info: eu-repo para los tipos de publicación. 
- Por compatibilidad con este vocabulario controlado anterior, si los registros actualmente utilizados contienen dichos vocabularios, se recomienda mantenerlos y agregar los nuevos campos con los nuevos vocabularios propuestos (COAR, REDCOL, etc..). 
- Los valores de tipologías que se manejaban en este vocabulario **INFO:EU-REPO** (ahora obsoleto) son:
  
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Tipología                     | Driver/OpenaireV3                               | OpenAireV4                                    |
+===============================+=================================================+===============================================+
| Artículo científico           | info:eu-repo/semantics/article                  | Artículo de revista (Concepto genérico)       |
|                               |                                                 | http://purl.org/coar/resource_type/c_6501     |
|                               |                                                 |                                               |
|                               |                                                 | Artículo de Revista - Resultado de            |
|                               |                                                 | Investigación                                 |
|                               |                                                 | http://purl.org/coar/resource_type/c_2df8fbb1 |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Trabajo de Grado - Pregrado   | info:eu-repo/semantics/bachelorThesis           | http://purl.org/coar/resource_type/c_7a1f     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Trabajo de Grado - Máster     | info:eu-repo/semantics/masterThesis             | http://purl.org/coar/resource_type/c_bdcc     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Tesis de Doctorado            | info:eu-repo/semantics/doctoralThesis           | http://purl.org/coar/resource_type/c_db06     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Libro                         | info:eu-repo/semantics/book                     | http://purl.org/coar/resource_type/c_2f33     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Capítulo de Libro             | info:eu-repo/semantics/bookPart                 | http://purl.org/coar/resource_type/c_3248     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Revisión, Crítica, Comentario | info:eu-repo/semantics/review                   | http://purl.org/coar/resource_type/c_efa0     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Contribución a congreso       | info:eu-repo/semantics/conferenceObject         | http://purl.org/coar/resource_type/c_c94f     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Ponencia                      | info:eu-repo/semantics/lecture                  | http://purl.org/coar/resource_type/c_8544     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Documento de Trabajo          | info:eu-repo/semantics/workingPaper             | http://purl.org/coar/resource_type/c_8042     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Pre-Publicación               | info:eu-repo/semantics/preprint                 | http://purl.org/coar/resource_type/c_816b     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Reporte                       | info:eu-repo/semantics/report                   | http://purl.org/coar/resource_type/c_93fc     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Glosa (Nota de Texto)         | info:eu-repo/semantics/annotation               | http://purl.org/coar/resource_type/c_1162     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Contribución a Revista        | info:eu-repo/semantics/contributionToPeriodical | http://purl.org/coar/resource_type/c_3e5a     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Patente                       | info:eu-repo/semantics/patent                   | http://purl.org/coar/resource_type/c_15cd     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+
| Otros                         | info:eu-repo/semantics/other                    | http://purl.org/coar/resource_type/c_1843     |
+-------------------------------+-------------------------------------------------+-----------------------------------------------+


- Este conjunto de directrices está utilizando el elemento resourceType del esquema de metadatos DataCite MetadataKernel v4.2. [#]_
- A dicho esquema se le adicionaron dos atributos para refinar el contenido del campo:
	- El atributo **uri** para el concepto de tipo de recurso URI a este perfil de aplicación
	- El atributo **resourceTypeContext** para determinar el contexto de aplicación de la tipología documental descrita.

.. [#] https://schema.datacite.org/meta/kernel-4.2/doc/DataCite-MetadataKernel_v4.2.pdf


		
		

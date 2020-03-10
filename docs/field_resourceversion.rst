.. _aire:version:

Resource Version (Versión del recurso) (R)
==========================================

``oaire:version``

Definición y alcance del campo
------------------------------

Dependiendo del tipo de recurso, este campo se utiliza para describir los siguientes elementos:

	- La versión de un conjunto de datos o software (Nombre Clave ó Número).
	- El estado del proceso editorial del recurso basándose en un vocabulario controlado normalizado.
 

Niveles de persistencia (M/MA/R/O)
------------------------------------
Recomendado (R)

Niveles de ocurrencia (R / NR)
------------------------------------------------
Repetible (R): 0-n

Esquema de metadatos
------------------------------
oaire:version

Traducción al español
---------------------
(Estado, Nombre Clave ó Número) de la Versión de publicación del recurso 

Forma de Descripción Normalizada (RDA / RCAA2 /ISBD)
----------------------------------------------------
RDA (Recursos: descripción y acceso)

	- Cuando se trate de la versión del estado de publicación, revise la forma adecuada para ingresar la versión del recurso según el vocabulario propuesto.
	- Cuando se describa la versión (Nombre Clave ó Número) Revise la forma adecuada para ingresar la versión del recurso.


Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad Principal Versión (version) (R, 0-n):
+++++++++++++++++++++++++++++++++++++++++++++++

Utilice un número de versión o la etiqueta del término de vocabulario como valor.

	- **Atributo: URI (uri) (MA, 1):** Este atributo permite especificar la URI que identifica la versión del estado de publicación. Se debe tener en cuenta los siguientes tipos de URI y su codificación normalizada según el vocabulario controlado propuesto (http://vocabularies.coar-repositories.org/documentation/version_types/):

+----------------------------------------------------+----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| ConceptURI                                         | Etiqueta | Comentario                                                                                                                                                        |
+====================================================+==========+===================================================================================================================================================================+
| http://purl.org/coar/version/c_b1a7d7d4d402bcce    | AO       | Versión original del autor, Borrador, Manuscrito                                                                                                                  |
+----------------------------------------------------+----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| http://purl.org/coar/version/c_71e4c1898caa6e32    | SMUR     | Versión sometida a revisión, Versión no evaluada por pares, versión enviada a revisión, versión enviada a revisión por pares, versión enviada al editor, preprint |
+----------------------------------------------------+----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| http://purl.org/coar/version/c_ab4af688f83e57aa    | AM       | Versión final del autor, Versión aceptada para publicar, postprint, manuscrito aceptado                                                                           |
+----------------------------------------------------+----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| http://purl.org/coar/version/c_fa2ee174bc00049f    | P        | Prueba de Galera, manuscrito editado, manuscrito aceptado                                                                                                         |
+----------------------------------------------------+----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| http://purl.org/coar/version/c_970fb48d4fbd8a85    | VoR      | Versión publicada, Versión de registro, versión final del editor                                                                                                  |
+----------------------------------------------------+----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| http://purl.org/coar/version/c_e19f295774971610    | CVoR     | Versión corregida, versión publicada corregida                                                                                                                    |
+----------------------------------------------------+----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| http://purl.org/coar/version/c_dc82b40f9837b551    | EVoR     | Versión mejorada, versión ampliada                                                                                                                                |
+----------------------------------------------------+----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| http://purl.org/coar/version/c_be7fb7dd8ff6fe43    | NA       | Versión desconocida, versión No aplicable (o desconocido)                                                                                                         |
+----------------------------------------------------+----------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Relaciones con otros campos
---------------------------

- No confundir el campo de versión del recurso **(oaire:version)** con el campo identificador relacionado **(datacite:relatedIdentifier)** en especial con los atributos: IsVersionOf, HasVersion, IsPreviousVersionOf, IsNewVersionOf
- No confundir el campo versión del recurso **(oaire:version)** con el campo descripción del recurso **(dc:description)**
- El campo de versión del recurso **(oaire:version),** está relacionado directamente con la fecha asociada al estado de publicación del recurso **(datacite:date),** en específico con el atributo dateType
- No confundir la versión del recurso de información **(oaire:version)** con la edición de publicación del mismo **(dc.description.edition)**

Restricciones
-------------
Ninguna

Ejemplos y ayudas
-----------------

Ayudas
++++++

	- **Versión del Recurso:** DSPACE 6.3
	- **Versión del estado de Publicación (Borrador):** http://purl.org/coar/version/c_b1a7d7d4d402bcce

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:type>http://purl.org/coar/version/c_970fb48d4focketsa85</dc:type>
   <dc:type>info:eu-repo/semantics/draft</dc:type>
	
	
**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <oaire:version>1.0.3</oaire:version>
   <oaire:version uri="http://purl.org/coar/version/c_be7fb7dd8ff6fe43">AM</oaire:version>

**Esquema xoai**

.. code-block:: xml
   :linenos:
   
   <element name="dc">
		<element name="type">
			<element name="version">
				<element name="spa">
					<field name="value">info:eu-repo/semantics/draft</field>
				</element>
			</element>
		</element>
   </element>
   <element name="oaire">
		<element name="version">
			<element name="spa">
				<field name="value">http://purl.org/coar/version/c_970fb48d4focketsa85</field>
			</element>
		</element>
	</element>
 

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="type" qualifier="version" lang="spa">info:eu-repo/semantics/publishedVersion</dim:field>
   <dim:field mdschema="oaire" element="version" qualifier="" lang="spa">http://purl.org/coar/version/c_970fb48d4focketsa85</dim:field>

Niveles de aplicación para  productos de investigación de MinCiencias
---------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias.

Relaciones con otros modelos de metadatos
-----------------------------------------
El campo **Versión de recurso (oaire:version)** es utilizado por los siguientes esquemas:

+----------------------+-----------------------+
| Esquema de Metadatos | Campo Relacionado     |
+======================+=======================+
| marcxml              | 250$a (Edición)       |
+----------------------+-----------------------+
| dc                   | dc.type               |
+----------------------+-----------------------+
| dcterms              | dcterms.type          |
+----------------------+-----------------------+
| datacite             | datacite.resourcetype |
+----------------------+-----------------------+

Niveles semánticos
------------------

	- Este campo contempla la utilización de distintos calificadores de la versión del estado de publicación como atributos estandarizados según un vocabulario específico COAR que maneja elementos semánticos.

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

+----------------------------------------+-----------------------+---------------+------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores | Nota de alcance        |
+========================================+=======================+===============+========================+
| Versión (Clave ó Número)               | dc.description        | version       |                        |
+----------------------------------------+-----------------------+---------------+------------------------+
| Estado de Publicación(Driver/OpenAire3)| dc.type               | version       |                        |
+----------------------------------------+-----------------------+---------------+------------------------+
| Estado de Publicación(OpenAire4)       | oaire.version         |               | equivalencia semántica |
|                                        |                       |               | dc.type.coarversion    |
+----------------------------------------+-----------------------+---------------+------------------------+

Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

	- Las versiones anteriores de las Directrices de OpenAIRE y Driver utilizaban el vocabulario info: eu-repo para los tipos de publicación. Se recomienda actualizar los valores del vocabulario anterior al nuevo vocabulario. Los valores anteriores de este vocabulario (obsoleto) son:

+---------------------------------------------------------+-----------------------------------------+----------------------------------------------------+
| Estado de Publicación                                   | Driver/OpenaireV3                       | OpenAireV4                                         |
+=========================================================+=========================================+====================================================+
| Versión original del autor, Borrador, Manuscrito        | info:eu-repo/semantics/draft            | http://purl.org/coar/version/c_b1a7d7d4d402bcce    |
+---------------------------------------------------------+-----------------------------------------+----------------------------------------------------+
| Versión sometida a revisión                             | info:eu-repo/semantics/submittedVersion | http://purl.org/coar/version/c_71e4c1898caa6e32    |
+---------------------------------------------------------+-----------------------------------------+----------------------------------------------------+
| Versión final del autor, Versión aceptada para publicar | info:eu-repo/semantics/acceptedVersion  | http://purl.org/coar/version/c_ab4af688f83e57aa    |
+---------------------------------------------------------+-----------------------------------------+----------------------------------------------------+
| Prueba de Galera                                        |                                         | http://purl.org/coar/version/c_fa2ee174bc00049f    |
+---------------------------------------------------------+-----------------------------------------+----------------------------------------------------+
| Versión publicada                                       | info:eu-repo/semantics/publishedVersion | http://purl.org/coar/version/c_970fb48d4fbd8a85    |
+---------------------------------------------------------+-----------------------------------------+----------------------------------------------------+
| Versión corregida                                       |                                         | http://purl.org/coar/version/c_e19f295774971610    |
+---------------------------------------------------------+-----------------------------------------+----------------------------------------------------+
| Versión mejorada, versión ampliada                      | info:eu-repo/semantics/updatedVersion   | http://purl.org/coar/version/c_dc82b40f9837b551    |
+---------------------------------------------------------+-----------------------------------------+----------------------------------------------------+
| Versión desconocida                                     |                                         | http://purl.org/coar/version/c_be7fb7dd8ff6fe43    |
+---------------------------------------------------------+-----------------------------------------+----------------------------------------------------+

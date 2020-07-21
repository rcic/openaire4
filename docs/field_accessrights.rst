.. _dci:accessrights:

Access Rights (Derechos de acceso) (M)
======================================

``datacite:rights``

Definición y alcance del campo
------------------------------
Se describen las condiciones de acceso al recurso según su contenido. Información sobre el tipo de acceso o derecho que va a tener el recurso. Si los metadatos describen más de un recurso, por ejemplo, texto completo y material complementario, se debe proporcionar el derecho de acceso del recurso principal.

Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR)
-------------------------------
No repetible (NR): 1 **vez**

Esquema de metadatos
------------------------------
datacite:rights

Nota: Este campo se ha adaptado del esquema de metadatos DATACITE MetadataKernel versión 4.2 (http://doi.org/10.5438/0014), el cual es utilizado ampliamente para la gestión de documentos y datos.

Traducción al español
---------------------
Derechos de acceso

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
**RDA (Recursos: descripción y acceso):** Revise la forma adecuada para ingresar la información de título con su debida puntuación:

	- **datacite:rights:** Se debe de seleccionar las condiciones de acceso que se le van a dar al recurso definidas previamente en los atributos del campo con la definición previa del vocabulario controlado de COAR. Ej: uri: http://vocabularies.coar-repositories.org/access_right/c_abf2.html → Acceso Abierto

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad Derechos de Acceso (AccessRights) (M, 1):
+++++++++++++++++++++++++++++++++++++++++++++++++++

Usa la etiqueta del término de vocabulario como valor del campo.

	- **Atributos URI (M,1):** Use la dirección URI relacionada según vocabulario de derechos de acceso (Access Rights) desarrollado por **COAR** el cual es presentado a continuación:

+------------------------------------------+-------------------------+
| URI                                      | Etiqueta                |
+==========================================+=========================+
| http://purl.org/coar/access_right/c_abf2 | Acceso abierto          |
+------------------------------------------+-------------------------+
| http://purl.org/coar/access_right/c_f1cf | Acceso embargado        |
+------------------------------------------+-------------------------+
| http://purl.org/coar/access_right/c_16ec | Acceso restringido      |
+------------------------------------------+-------------------------+
| http://purl.org/coar/access_right/c_14cb | Acceso a solo metadatos |
+------------------------------------------+-------------------------+

Relaciones con otros campos
---------------------------

	- No confundir el campo de derechos de acceso **(datacite:rights)** con el campo que indica la condición de la licencia **(oaire:licenseCondition)**
	- No confundir el campo de derechos de acceso **(datacite:rights)** con notas de acceso (dc.description)

Restricciones
-------------
No aplica 


Ejemplos y ayudas
-----------------

Ayudas
++++++

	- **Derechos de acceso:** Coloque el término del vocabulario COAR. Ej: http://purl.org/coar/access_right/c_abf2

Ejemplo en XML  (Interoperabilidad OAI-PMH) 
+++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:rights>http://purl.org/coar/access_right/c_16ec</dc:rights>
   <dc:rights>info:eu-repo/semantics/closedAccess</dc:rights>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <datacite:rights rightsURI="http://purl.org/coar/access_right/c_abf2">open access</datacite:rights>

**Esquema xoai**

.. code-block:: xml
   :linenos:
   <element name="dc">   
	<element name="rights">
     <element name="accessrights">
          <element name="spa">
             <field name="value">info:eu-repo/semantics/embargoedAccess</field>
         </element>
     </element>
	</element>
   </element>   
   <element name="oaire">
     <element name="accessrights">
          <element name="spa">
             <field name="value">http://purl.org/coar/access_right/c_f1cf</field>
         </element>
     </element>
   </element>   

**Esquema dim**

.. code-block:: xml
   :linenos:

    <dim:field mdschema="dc" element="rights" qualifier="accessrights" lang="spa">http://purl.org/coar/access_right/c_f1cf</dim:field>

Atributos de Campo
------------------
Use el siguiente vocabulario de acceso COAR: http://vocabularies.coar-repositories.org/documentation/access_rights/

+-----------------------------------------------+-------------------------+
| ConceptURI                                    | Etiqueta                |
+===============================================+=========================+
| http://purl.org/coar/access_right/c_abf2      | Acceso abierto          |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/access_right/c_f1cf      | Acceso embargado        |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/access_right/c_16ec      | Acceso restringido      |
+-----------------------------------------------+-------------------------+
| http://purl.org/coar/access_right/c_14cb      | Acceso a solo metadatos |
+-----------------------------------------------+-------------------------+

Especificadores de campo
------------------------

Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------
El campo **Derechos de Acceso** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

======================  =======================
Esquema de Metadatos    Campo Relacionado      
======================  =======================
dc                      * dc.rights.access
                        * dc.rights       
dcterms                 dcterms.rights.access  
lom                     lom.rights.access      
marcxml                 field:506              
======================  =======================


Niveles semánticos
------------------

- Este campo contempla la utilización de distintos calificadores de los derechos de acceso como atributos estandarizados según un vocabulario específico COAR que maneja elementos semánticos: (http://vocabularies.coar-repositories.org/documentation/access_rights/)

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

+------------------------+-----------------------+---------------+----------------------------+
| Vocabulario controlado | Campo elemento DSPACE | Calificadores | Nota de alcance            |
+========================+=======================+===============+============================+
| Driver / OpenAire 3    | dc.rights             | accessrights  | Derechos de acceso         |
+------------------------+-----------------------+---------------+----------------------------+
| OpenAire4              | dc.rights             | coar          | Equivalencia semántica con:|
|                        |                       |               |                            |
|                        |                       |               | - **oaire.accessrights**   |
|                        |                       |               | - **datacite.rights**      |
|                        |                       |               |                            |
+------------------------+-----------------------+---------------+----------------------------+

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

	- En las distintas directrices que han existido, siempre ha sido obligatorio el uso del campo derechos de acceso.
	- Se recomienda específicamente crear los nuevos atributos/especificadores de campo de título según la codificación propuesta.
	- En la siguiente tabla puede revisar los términos del vocabulario de eu-repo-Access-Terms de OpenAIRE V3 y su equivalencia en OpenAIRE V4. 

+------------------------------------------+-----------------------------------------+--------------------+
| OpenAIRE V4                              | OpenAIRE V3                             | Etiqueta           |
+==========================================+=========================================+====================+
| http://purl.org/coar/access_right/c_14cb | info:eu-repo/semantics/closedAccess     | Acceso cerrado     |
+------------------------------------------+-----------------------------------------+--------------------+
| http://purl.org/coar/access_right/c_f1cf | info:eu-repo/semantics/embargoedAccess  | Acceso embargado   |
+------------------------------------------+-----------------------------------------+--------------------+
| http://purl.org/coar/access_right/c_16ec | info:eu-repo/semantics/restrictedAccess | Acceso restringido |
+------------------------------------------+-----------------------------------------+--------------------+
| http://purl.org/coar/access_right/c_abf2 | info:eu-repo/semantics/openAccess       | Acceso abierto     |
+------------------------------------------+-----------------------------------------+--------------------+

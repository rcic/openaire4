.. _dci:contributor:

Contributor (Colaborador) (MA)
==============================

``datacite:contributor``

Definición y alcance del campo
------------------------------
Es la entrada secundaria. El campo “Colaborador” define las entidades responsables de contribuir a la creación, desarrollo, gestión y publicación del contenido del recurso.  Esta entidad puede ser una persona, una organización o un servicio (máquina).


Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio si es aplicable ó si está definido explícitamente en el recurso de información (MA)

Niveles de ocurrencia (R / NR)
-------------------------------

Repetible (R): **0-n veces**.
Repita este campo para describir todas las entidades responsables de la creación del recurso en **orden prioritario** ó de presentación

Esquema de metadatos
------------------------------
datacite:contributor
**Nota:** Este campo se ha adaptado del esquema de metadatos DATACITE MetadataKernel versión 4.1 (http://doi.org/10.5438/0014), el cual es utilizado ampliamente para la gestión de documentos y datos.

Traducción al español
---------------------
Colaborador

Forma de Descripción Normalizada (RDA / RCAA2 / ISBD)
-----------------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar el nombre del colaborador con su debida puntuación:

- Para nombres personales utilizar el formato invertido de tal forma que la sintaxis sea: “Apellido” + “, “ + “Nombre”. De manera complementaria, los nombres personales se pueden codificar utilizando los siguientes formatos:
 
		- APA (American Psychological Association)
		- MLA (Modern Language Association of America)
		- Vancouver 
		- Chicago

- Para nombre de autores corporativos, donde exista una jerarquía institucional clara, enumerar las partes de la jerarquía de mayor a menor y separarlas con puntos seguidos de un espacio. Si no queda clara la existencia de una jerarquía, o si se desconoce cuál es la parte más grande y más pequeña del cuerpo, facilitar el nombre tal como aparece en la copia electrónica.

- Para el caso que la colaboración se haya realizado a través de un servicio, se debe describir el nombre del servicio, la versión del servicio, la URL del servicio, el método utilizado y demás elementos que se consideren importantes.

- Registrar el nombre de cada colaborador en instancias separadas. Para el caso de los trabajos de grado y tesis de maestría/doctorado, se debe registrar en la primera instancia al director (a).


Propiedades, atributos y especificadores de campo
-------------------------------------------------

Clase Principal Colaboradores(contributors) (MA, 0-n):
++++++++++++++++++++++++++++++++++++++++++++++++++++++
Entidad que agrupa todos los colaboradores del recurso.

Propiedad: Colaborador (contributor) (MA, 0-n):
+++++++++++++++++++++++++++++++++++++++++++++++++++
Entidad que identifica cada uno de los colaboradores del recurso.

- **Atributo: Tipo de Colaboración (contributorType) (M, 1):** Este atributo, define el rol del colaborador durante el ciclo de vida del mismo. Este campo es obligatorio cuando se define la propiedad “contributor”. Se debe tener en cuenta los siguientes tipos de colaboradores y su codificación normalizada según el vocabulario controlado propuesto:

+-------------------------+----------------------------------------------------------+------------------------+
| Vocabulario Normalizado | Descripción del Atributo                                 | Dominio de Vocabulario |
+=========================+==========================================================+========================+
| Advisor                 | Director de trabajo de grado tesis de maestría/doctorado | redcol                 |
+-------------------------+----------------------------------------------------------+------------------------+
| AudiovisualDesigner     | Diseñador Audiovisual                                    | redcol                 |
+-------------------------+----------------------------------------------------------+------------------------+
| AudiovisualDirector     | Director Audiovisual                                     | redcol                 |
+-------------------------+----------------------------------------------------------+------------------------+
| ContactPerson           | Persona de contacto                                      | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| ContentProvider         | Proveedor de Contenidos                                  | redcol/lom             |
+-------------------------+----------------------------------------------------------+------------------------+
| DataCollector           | Recolector de datos                                      | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| DataCurator             | Curador de datos                                         | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| DataManager             | Administrador de datos                                   | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| Distributor             | Distribuidor                                             | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| Editor / Compilator     | Editor - Compilador                                      | datacite/redcol/lom    |
+-------------------------+----------------------------------------------------------+------------------------+
| EducationalValidator    |                                                          | redcol                 |
+-------------------------+----------------------------------------------------------+------------------------+
| ExecutiveProducer       | Productor Ejecutivo                                      | redcol                 |
+-------------------------+----------------------------------------------------------+------------------------+
| HostingInstitution      | Institución anfitriona                                   | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| Financer                | Financista                                               | redcol                 |
+-------------------------+----------------------------------------------------------+------------------------+
| GraphicalDesigner       | Diseñador Gráfico                                        | redcol/lom             |
+-------------------------+----------------------------------------------------------+------------------------+
| Illustrator             | Ilustrador                                               | redcol                 |
+-------------------------+----------------------------------------------------------+------------------------+
| Initiator               | Iniciador                                                | redcol/lom             |
+-------------------------+----------------------------------------------------------+------------------------+
| InstructionalDesigner   | Diseñador Instruccional                                  | redcol/lom             |
+-------------------------+----------------------------------------------------------+------------------------+
| Photographer            | Fotografo                                                | redcol                 |
+-------------------------+----------------------------------------------------------+------------------------+
| Producer                | Productor                                                | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| ProjectLeader           | Lider de Proyecto                                        | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| ProjectManager          | Jefe de Proyecto                                         | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| ProjectMember           | Miembro de Proyecto                                      | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| Referee                 | Par Evaluador                                            | redcol                 |
+-------------------------+----------------------------------------------------------+------------------------+
| RegistrationAgency      | Agencia de registro                                      | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| RegistrationAuthority   | Autoridad de registro                                    | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| RelatedPerson           | Persona Relacionada                                      | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| Researcher              | Investigador                                             | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| ResearchGroup           | Grupo de investigación                                   | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| RightsHolder            | Titular de derechos                                      | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| ScriptWriter            | Guionista                                                | redcol/lom             |
+-------------------------+----------------------------------------------------------+------------------------+
| SoftwareDeveloper       | Desarrollador - Programador - Integrador de software -   | redcol                 |
+-------------------------+----------------------------------------------------------+------------------------+
| Sponsor                 | Patrocinador                                             | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| SubjectMatterExpert     | experto en la materia                                    | redcol/lom             |
+-------------------------+----------------------------------------------------------+------------------------+
| Supervisor              | Supervisor                                               | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| TechnicalImplementer    | Implementador técnico                                    | redcol/lom             |
+-------------------------+----------------------------------------------------------+------------------------+
| TechnicalValidator      | Validador Técnico                                        | redcol/lom             |
+-------------------------+----------------------------------------------------------+------------------------+
| Terminator              | Terminador / Corrector de Pruebas                        | redcol/lom             |
+-------------------------+----------------------------------------------------------+------------------------+
| Translator              | Traductor                                                | redcol                 |
+-------------------------+----------------------------------------------------------+------------------------+
| Validator               | Validador                                                | redcol/lom             |
+-------------------------+----------------------------------------------------------+------------------------+
| WebDeveloper            | Desarrollador Web                                        | redcol                 |
+-------------------------+----------------------------------------------------------+------------------------+
| WorkPackageLeader       | Líder de paquete de trabajo                              | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+
| Other                   | Otros                                                    | datacite               |
+-------------------------+----------------------------------------------------------+------------------------+

	Notas: La definición de cada uno de los tipos de colaboración se basa principalmente en los siguientes esquema de metadatos:

	- DATACITE (https://schema.datacite.org/meta/kernel-4.1/doc/DataCite-MetadataKernel_v4.1.pdf) 
	- LOM (http://tvdi.det.uvigo.es/proyectos/t-learning/SCORM_ontology/LOM_Contributor.html)

- **Sub-Propiedad: Nombre Completo del Colaborador (contributorName) (M, 1):** Esta propiedad incluye el texto asociado al colaborador del recurso que debe ser descrito en cualquiera de los formas de descripción propuestas para el campo authorName.

	- **Atributo: Tipo de Colaborador (nameType) (O, 0-1):** Este atributo permite especificar el tipo de colaborador que se describe en el campo de metadatos. Se debe tener en cuenta los siguientes tipos de colaboradores y su codificación normalizada según el vocabulario controlado propuesto:

..

	+-------------------------+----------------------------+------------------------+
	| Vocabulario Normalizado | Descripción del Atributo   | Dominio de Vocabulario |
	+=========================+============================+========================+
	| Organizational          | Colaboración Corporativo   | datacite               |
	+-------------------------+----------------------------+------------------------+
	| Personal                | Colaboración Personal      | datacite               |
	+-------------------------+----------------------------+------------------------+
	| Event                   | Colaboración Conferencia - | redcol                 |
	|                         | Evento                     |                        |
	+-------------------------+----------------------------+------------------------+
	| Service                 | Servicio                   | redcol                 |
	+-------------------------+----------------------------+------------------------+

..

	- **Sub-Propiedad: Nombres (givenName) (O, 0-1):** Esta propiedad de uso opcional, incluye el texto asociado exclusivamente a los nombres (primer y segundo nombres) del colaborador cuando este se trate de una persona.

	- **Sub-Propiedad: Apellidos (familyName) (O, 0-1):** Esta propiedad de uso opcional, incluye el texto asociado exclusivamente a los apellidos (primer y segundo apellidos) del colaborador cuando este se trate de una persona. 

	- **Sub-Propiedad: Afiliación institucional (affiliation) (O, 0-n):** Esta propiedad de uso opcional, incluye el texto asociado a las distintas afiliación institucionales a las que pertenece el colaborador. 

	- **Sub-Propiedad: Identificador de Nombre (nameIdentifier) (O, 0-n):** Esta propiedad de uso opcional, incluye el texto asociado que permite identificar de manera unívoca un colaborador como persona natural o corporativa a partir del uso de diversos esquemas de identificación. El formato de texto asociado depende de cada esquema de identificación utilizado. Se debe tener en cuenta los siguientes tipos de identificadores existentes y su codificación normalizada en los atributos de esta propiedad (nameIdentifierScheme),  según el vocabulario controlado propuesto (Uso Opcional):


+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+
| Vocabulario Normalizado (nameIdentifierScheme) | Descripción del Elemento                                                | Esquema de Dominio del Vocabulario (schemeURI)    |
+================================================+=========================================================================+===================================================+
| EMAIL                                          | Dirección principal de correo electrónico                               | https://schema.org/email                          |
+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+
| ORCID                                          | Open Researcher and Contributor ID                                      | https://orcid.org                                 |
+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+
| ISNI                                           | International Standard Name Identifier (ISO 27729)                      | http://www.isni.org/                              |
+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+
| PUBLONS                                        | Clarivate Analytics Publons ID                                          | https://publons.com                               |
+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+
| RESEARCHID                                     | Web of Science ResearcherID                                             | https://www.researcherid.com                      |
+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+
| SCOPUS                                         | Author ID SCOPUS                                                        | https://www.scopus.com/freelookup/form/author.uri |
+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+
| IRALISID                                       | IRA-LIS                                                                 | https://www.iralis.org/                           |
+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+
| VIAF                                           | Virtual International Authority File                                    | https://viaf.org/                                 |
+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+
| LCNAF                                          | Library of Congress authority ID                                        | http://id.loc.gov/authorities/names.html          |
+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+
| OCLC                                           | OCLC FAST Authority File                                                | http://experimental.worldcat.org/fast/            |
+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+
| WIKIDATA                                       | Wikidata databse                                                        | https://www.wikidata.org                          |
+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+
| OTHERS                                         | Incluye: Facebook, Twitter, Mendeley, LinkedIn, BNE, BNC, ResearchGate. |                                                   |
+------------------------------------------------+-------------------------------------------------------------------------+---------------------------------------------------+

..

	- **Atributo Nombre del esquema del identificador (nameIdentifierScheme) (M, 1, si es utilizada la propiedad nameIdentifier):** Este atributo permite especificar el nombre del esquema identificador utilizado para describir al colaborador en el campo de metadatos. Se debe tener en cuenta el vocabulario controlado propuesto en la propiedad nameIdentifier.

	- **Atributo URI del esquema del identificador (schemeURI) (M, 1, si es utilizada la propiedad nameIdentifier):** Este atributo permite especificar la URI del nombre del esquema identificador utilizado para describir al colaborador en el campo de metadatos. Se debe tener en cuenta el vocabulario controlado propuesto en la propiedad **nameIdentifier**

Relaciones con otros campos
---------------------------

	- No debe confundirse al **colaborador (dc.contributor)** del recurso  con el autor del recurso **(dc.creator) incluidas sus especificadores de campo.**
	- No debe confundirse al **colaborador (dc.contributor)** del recurso  con la entidad responsable de la **publicación (dc.publisher)** del mismo.
	- Cuando se trate de describir a una entidad que patrocina el desarrollo de un recurso de información  de debe utilizar el campo **dc.contributor.sponsor** y no los campos **dc.description.sponsorship** ó  **dc.description.funder.**
	- Cuando se describe al director de un trabajo de grado ó tesis de maestría ó doctorado se debe utilizar dc.contributor.advisor.
	- Para identificar la institución que certifica el grado de un trabajo de grado ó tesis de maestría / doctorado debe utilizarse **thesis.degree.grantor.**


Restricciones
-------------
Ninguna 
 

Ejemplos y ayudas
-----------------

Ayudas
++++++

- Colaborador Editor/Compilador de la obra):
- Colaborador Traductor:

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:contributor>Vivas Barrera, Tania Giovanna, editora</dc:contributor>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   	<datacite:contributors>
        <datacite:contributor>
          <datacite:contributorName>Evans, R. J.</datacite:contributorName>
        <datacite:contributor>
        <datacite:contributor>
          <datacite:contributorName>International Human Genome Sequencing Consortium</datacite:contributorName>
        </datacite:contributor>
	</datacite:contributors>


**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="contributor" qualifier="editor" lang="spa">Vivas Barrera, Tania Giovanna, editora</dim:field>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   	<element name="dc">
	<element name="contributor">
	<element name="editor">
	<element name="spa">
	<field name="value">Vivas Barrera, Tania Giovanna</field>
	</element>
	</element>
	</element>

.. code-block:: xml
   :linenos:

    <element name="dc">
      <element name="contributor">
         <element name="author">
            <element name="none">
               <field name="value">Gasparini, Blaž</field>
               <field name="authority">a863d05d988bdb56375ccf483f6c2ef3</field>
               <field name="confidence">600</field>
               <field name="orcid-id" />
            </element>
         </element>
         <element name="supervisor">
            <element name="none">
               <field name="value">Lohmann, Ulrike</field>
               <field name="authority">895d98a3537122db33165a6db6c0af61</field>
               <field name="confidence">600</field>
               <field name="orcid-id" />
               <field name="value">Peter, Thomas</field>
               <field name="authority">53688288a3c9335eefa0ddc6b1b85b0c</field>
               <field name="confidence">600</field>
               <field name="orcid-id" />
               <field name="value">Leisner, Thomas</field>
               <field name="authority">728336b61c3952148ab1b65bdc2a9202</field>
               <field name="confidence">600</field>
               <field name="orcid-id" />
            </element>
         </element>

..


Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

El campo **Colaborador (datacite:contributor)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+------------------------------------+
| Esquema de Metadatos | Campo Relacionado                  |
+======================+====================================+
| dc                   | * dc.contributor                   |
|                      | * dc.contributor.advisor           |
|                      | * dc.contributor.editor, etc.      |
+----------------------+------------------------------------+
| dcterms              | * dcterms.contributor              |
|                      | * dcterms.contributor.advisor      |
|                      | * dcterms.contributor.editor, etc. |
+----------------------+------------------------------------+
| lom                  | lom.lifecycle.contribute           |
+----------------------+------------------------------------+
| marcxml              | field:700,710,711                  |
+----------------------+------------------------------------+


Niveles semánticos
------------------

- Para la gestión normalizada de roles de usuario, se está tomando como base las siguientes ontologías:

	- LOM Ontologiy (http://tvdi.det.uvigo.es/proyectos/t-learning/SCORM_ontology/index.html):
	- Datacite Ontology (https://sparontologies.github.io/datacite/current/datacite.html)
	- FOAF Ontology (http://xmlns.com/foaf/spec/)
	- CERIF Ontology (https://www.eurocris.org/ontologies/semcerif/)

- Este campo contempla la utilización de distintos **sistemas de gestión de autoridades de nombre** que normalizan semánticamente los colaboradores.

- Cada registro presente en estos **sistemas de gestión de autoridades de nombre provee una Identificación persistente.**

- **Adicionalmente dichos sistemas proveen una URI única que debe ser enlazada y utilizada en el campo de metadatos asociado.**

- **En su mayoría, los sistemas de gestión de autoridades de nombre** contemplan la exportación de registros en representaciones semánticas MADS/SKOS a través de formatos MARCXML, RDF, XML, N3, Turtle, JSON.

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

..

+----------------------------------------+-----------------------+-----------------------+-----------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Cualificar            | Nota de alcance |
+========================================+=======================+=======================+=================+
| Advisor                                | dc.contributor        | advisor               |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| AudiovisualDesigner                    | dc.contributor        | audiovisualdesigner   |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| AudiovisualDirector                    | dc.contributor        | audiovisualdirector   |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| ContactPerson                          | dc.contributor        | contactperson         |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| ContentProvider                        | dc.contributor        | contentprovider       |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| DataCollector                          | dc.contributor        | datacollector         |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| DataCurator                            | dc.contributor        | datacurator           |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| DataManager                            | dc.contributor        | datamanager           |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Distributor                            | dc.contributor        | distributor           |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Editor / Compilator                    | dc.contributor        | editor                |Incluye          |
|                                        |                       |                       |Compilador       |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| EducationalValidator                   | dc.contributor        | educationalvalidator  |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| ExecutiveProducer                      | dc.contributor        | executiveproducer     |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| HostingInstitution                     | dc.contributor        | hostinginstitution    |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Financer                               | dc.contributor        | financer              |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| GraphicalDesigner                      | dc.contributor        | graphicaldesigner     |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Illustrator                            | dc.contributor        | illustrator           |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Initiator                              | dc.contributor        | initiator             |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| InstructionalDesigner                  | dc.contributor        | instructionaldesigner |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Photographer                           | dc.contributor        | photographer          |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Producer                               | dc.contributor        | producer              |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| ProjectLeader                          | dc.contributor        | projectleader         |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| ProjectManager                         | dc.contributor        | projectmanager        |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| ProjectMember                          | dc.contributor        | projectmember         |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Referee                                | dc.contributor        | referee               |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| RegistrationAgency                     | dc.contributor        | registrationagency    |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| RegistrationAuthority                  | dc.contributor        | registrationauthority |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| RelatedPerson                          | dc.contributor        | relatedperson         |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Researcher                             | dc.contributor        | researcher            |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| ResearchGroup                          | dc.contributor        | researchgroup         |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| RightsHolder                           | dc.contributor        | rightsholder          |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| ScriptWriter                           | dc.contributor        | scriptwriter          |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| SoftwareDeveloper                      | dc.contributor        | softwaredeveloper     |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Sponsor                                | dc.contributor        | sponsor               |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| SubjectMatterExpert                    | dc.contributor        | subjectmatterexpert   |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Supervisor                             | dc.contributor        | supervisor            |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| TechnicalImplementer                   | dc.contributor        | technicalimplementer  |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| TechnicalValidator                     | dc.contributor        | technicalvalidator    |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Terminator                             | dc.contributor        | terminator            |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Translator                             | dc.contributor        | translator            |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Validator                              | dc.contributor        | validator             |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| WebDeveloper                           | dc.contributor        | webdeveloper          |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| WorkPackageLeader                      | dc.contributor        | workpackageleader     |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+
| Other                                  | dc.contributor        | other                 |                 |
+----------------------------------------+-----------------------+-----------------------+-----------------+

..

**Notas:**

	- Con el fin de tener un alcance normalizado de las distintas propiedades y atributos (correos, afiliaciones, identificadores, etc..) asociadas a los autores, se recomienda utilizar la configuración de control de autoridades provista por DSPACE ó en su defecto incorporar características de sistema CRIS en DSPACE, en específico activar la entidad CONTRIBUTOR.


Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

	- En las distintas directrices que han existido, siempre ha sido obligatorio el uso del campo colaborador aunque no se hace explícito contemplar las diferencias de los distintos tipos y características de los autores.
	- En el sistema DSPACE en su instalación por defecto el campo autor viene con los campos **dc.contributor y dc.contributor.advisor** 
	- Se recomienda específicamente crear los nuevos atributos/especificadores del campo de autor según la codificación propuesta.

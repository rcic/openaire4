.. _dci:creator:

Creator (Creador) (M)
=====================

``datacite:creator``

Definición y alcance del campo
------------------------------

Es la entrada principal, que describe a la entidad(es) responsable(s) por la creación del contenido del recurso. Esta entidad puede ser nombre de persona o corporativo/institucional o evento (Conferencia, reunión, etc.).

En caso de múltiples entidades responsables de la creación del recurso, se debe repetir el elemento tantas veces como sea necesario


Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR)
------------------------------------------------
Repetible (R): **1-n veces**.
Repita este campo para describir todas las entidades responsables de la creación del recurso en **orden prioritario.**

Esquema de metadatos
------------------------------
datacite:creator
**Nota:** Este campo se ha adaptado del esquema de metadatos DATACITE MetadataKernel versión 4.1 (http://doi.org/10.5438/0014) , el cual es utilizado ampliamente para la gestión de documentos y datos.

Traducción al español
---------------------
Creador - Autor (Personal, Corporativo ó Conferencia/Evento)

Forma de Descripción Normalizada (RDA / RCAA2 / ISBD)
-----------------------------------------------------

RDA (Recursos: descripción y acceso)
Revise la forma adecuada para ingresar el nombre de autor con su debida puntuación:

- Para nombres personales utilizar el formato invertido de tal forma que la sintaxis sea: “Apellido” + “, “ + “Nombre”. De manera complementaria, los nombres personales se pueden codificar utilizando los siguientes formatos:
  
  - APA (American Psychological Association)
  - MLA (Modern Language Association of America)
  - Vancouver 
  - Chicago

- Para nombre de autores corporativos, donde exista una jerarquía institucional clara, enumerar las partes de la jerarquía de mayor a menor y separarlas con puntos seguidos de un espacio. Si no queda clara la existencia de una jerarquía, o si se desconoce cuál es la parte más grande y más pequeña del cuerpo, facilitar el nombre tal como aparece en la copia electrónica

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Clase Principal Autores (creators) (M, 1-n): 
++++++++++++++++++++++++++++++++++++++++++++

Entidad que agrupa todos los autores del recurso.

Propiedad: Autor (creator) (M, 1-n):
++++++++++++++++++++++++++++++++++++

Entidad que identifica cada uno de los autores del recurso.

**Sub-Propiedad: Nombre Completo del Autor (creatorName) (M, 1):** Esta propiedad incluye el texto asociado al autor del recurso en cualquiera de los formas de descripción propuestas. Los nombres de autores que contienen caracteres no romanos deben seguir el esquema de codificación propuesto por  `ALA-LC <http://www.loc.gov/catdir/cpso/roman.html>`_. 

    **Atributo: Tipo de Autor (nameType) (O, 0-1):** Este atributo permite especificar el tipo de autor que se describe en el campo de metadatos. Se debe tener en cuenta los siguientes tipos de autores y su codificación normalizada según el vocabulario controlado propuesto: 

+-------------------------+----------------------------+------------------------+
| Vocabulario Normalizado | Descripción del Atributo   | Dominio de Vocabulario |
+=========================+============================+========================+
| Organizational          | Autor Corporativo          | datacite               |
+-------------------------+----------------------------+------------------------+
| Personal                | Autor Personal             | datacite               |
+-------------------------+----------------------------+------------------------+
| Event                   | Autor Conferencia - Evento | redcol                 |
+-------------------------+----------------------------+------------------------+

    **Sub-Propiedad: Nombres (givenName) (O, 0-1):** Esta propiedad de uso opcional, incluye el texto asociado exclusivamente a los nombres (primer y segundo nombres) del autor personal. Esta propiedad está pensada como un complemento aclaratorio a la propiedad creatorName.

    **Sub-Propiedad: Apellidos (familyName) (O, 0-1):** Esta propiedad de uso opcional, incluye el texto asociado exclusivamente a los apellidos (primer y segundo apellidos) del autor personal. Esta propiedad está pensada como un complemento aclaratorio a la propiedad creatorName.

    **Sub-Propiedad: Afiliación institucional (affiliation) (O, 0-n):** Esta propiedad de uso opcional, incluye el texto asociado a las distintas afiliación institucionales a las que pertenece el autor. 

    **Sub-Propiedad: Identificador de Nombre (nameIdentifier) (O, 0-n):** Esta propiedad de uso opcional, incluye el texto asociado que permite identificar de manera unívoca una persona natural o corporativa a partir del uso de diversos esquemas de identificación. El formato de texto asociado depende de cada esquema de identificación utilizado. Se debe tener en cuenta los siguientes tipos de identificadores existentes y su codificación normalizada en los atributos de esta propiedad (nameIdentifierScheme,  según el vocabulario controlado propuesto (Uso Opcional): 

+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| Vocabulario Normalizado (nameIdentifierScheme) | Descripción del Elemento                           | Esquema de Dominio del Vocabulario (schemeURI)    |
+================================================+====================================================+===================================================+
| EMAIL                                          | Dirección principal de correo electrónico          | https://schema.org/email                          |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| ORCID                                          | Open Researcher and Contributor ID                 | https://orcid.org                                 |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| ISNI                                           | International Standard Name Identifier (ISO 27729) | http://www.isni.org/                              |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| PUBLONS                                        | Clarivate Analytics Publons ID                     | https://publons.com                               |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| RESEARCHID                                     | Web of Science ResearcherID                        | https://www.researcherid.com                      |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| SCOPUS                                         | Author ID SCOPUS                                   | https://www.scopus.com/freelookup/form/author.uri |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| IRALISID                                       | IRA-LIS                                            | https://www.iralis.org/                           |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| VIAF                                           | Virtual International Authority File               | https://viaf.org/                                 |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| LCNAF                                          | Library of Congress authority ID                   | http://id.loc.gov/authorities/names.html          |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| OCLC                                           | OCLC FAST Authority File                           | http://experimental.worldcat.org/fast/            |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| WIKIDATA                                       | Wikidata databse                                   | https://www.wikidata.org                          |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| SCHOLAR                                        | Google Scholar Profile ID                          | https://scholar.google.com                        |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+
| OTHERS                                         | Incluye:                                           |                                                   |           
|                                                |    * Facebook                                      |                                                   |   
|                                                |    * Twitter                                       |                                                   |    
|                                                |    * Mendeley                                      |                                                   |  
|                                                |    * LinkedIn                                      |                                                   |   
|                                                |    * BNE                                           |                                                   |   
|                                                |    * BNC                                           |                                                   |  
|                                                |    * ResearchGate                                  |                                                   |
+------------------------------------------------+----------------------------------------------------+---------------------------------------------------+

        **Atributo Nombre del esquema del identificador (nameIdentifierScheme) (M, 1, si es utilizada la propiedad nameIdentifier):** Este atributo permite especificar el nombre del esquema identificador utilizado para describir al autor en el campo de metadatos. Se debe tener en cuenta el vocabulario controlado propuesto en la propiedad nameIdentifier

        **Atributo URI del esquema del identificador (schemeURI) (M, 1, si es utilizada la propiedad nameIdentifier):** Este atributo permite especificar la URI del nombre del esquema identificador utilizado para describir al autor en el campo de metadatos. Se debe tener en cuenta el vocabulario controlado propuesto en la propiedad nameIdentifier

Relaciones con otros campos
---------------------------

- No debe confundirse al creador (dc.creator) del recurso  con el colaborador (dc.contributor) incluidas sus especificadores de campo.
- No debe confundirse al creador (dc.creator) del recurso  con la entidad responsable de la publicación (dc.publisher) del mismo.
- Se aplica equivalencia semántica de los campos dc.creator con los campos (dc.contributor.author, dc.contributor.corporatename, dc.contributor.conferencename)

Restricciones
-------------
No Aplica


Ejemplos y ayudas
-----------------

Ayudas
++++++

- **Autor Personal:** Entidad o persona colaboradora del contenido del objeto.  (Apellidos , Nombre)
  - Ej: García Márquez, Gabriel
  - Ej (VIAF): https://viaf.org/viaf/54147956 
  - Ej (LCNAF): http://id.loc.gov/authorities/names/n79063441 
  - Ej (OCLC): http://id.worldcat.org/fast/37134/ 
  - Ej (WIKIDATA): https://www.wikidata.org/wiki/Q5878 
  - Ej (ISNI): 0000 0001 2133 3785

..

  - Ej: Gómez Dueñas, Laureano Felipe
  - Ej (EMAIL): felipe.gomez3@gmail.com
  - Ej (ORCID): https://orcid.org/0000-0003-3580-8766
  - Ej (PUBLONS): https://publons.com/researcher/2885983
  - Ej (RESEARCHID): https://www.researcherid.com/rid/B-7117-2008 
  - Ej (IRALIS): COLIS0219
  - Ej (CVLAC): 0000687219
  - Ej (LINKEDIN): https://co.linkedin.com/in/laureanofg
  - Ej (MENDELEY): https://www.mendeley.com/profiles/laureano-gomez3/
  - Ej (SCHOLAR): https://scholar.google.com/citations?user=OtnBIDYAAAAJ 

..

  - Ej: Frías Montoya, José Antonio
  - Ej (EMAIL): frias@usal.es
  - Ej (SCOPUS): https://www.scopus.com/authid/detail.uri?authorId=57189653757
  - Ej (ORCID): http://orcid.org/0000-0002-5425-8950
  - EJ (DIALNET): https://dialnet.unirioja.es/servlet/autor?codigo=49767
  - Ej (ISNI): http://www.isni.org/isni/0000000066372537
  - Ej (LCNAF): https://id.loc.gov/authorities/names/n2004030504.html 
  - Ej (VIAF): https://viaf.org/viaf/69235229/ 
  - Ej (FAST): http://id.worldcat.org/fast/509557/
  - Ej (BNE): http://datos.bne.es/persona/XX1562287.html 
  - Ej (SCHOLAR): https://scholar.google.es/citations?user=YYsK-tIAAAAJ
  - Ej (RESEARCHGATE): https://www.researchgate.net/profile/Jose_Frias
  - Ej (FACEBOOK): https://www.facebook.com/jose.a.frias
  - Ej (TWITTER): https://twitter.com/jafrimon

- **Autor Corporativo:** Entidad o Institución responsable del contenido del objeto.

  - Ej: Colombia. Departamento Administrativo de Ciencia, Tecnología e Innovación - MinCiencias.
* 
  - Ej: MetaBibliotea SAS

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

- Esquema oai_dc

.. code-block:: xml
   :linenos:

   <dc:creator>Universidad Nacional de Colombia. Biblioteca</dc:creator>

- Esquema DataCite

.. code-block:: xml
   :linenos:

   <datacite:creators>
     <datacite:creator>
       <datacite:creatorName>Ramírez, Carlos.</datacite:creatorName>
       <datacite:affiliation>Observatorio Colombiano de Ciencia y Tecnología</datacite:affiliation>
       <datacite:nameIdentifier nameIdentifierScheme="ORCID"
                       schemeURI="http://orcid.org">
         1234-1234-1234-1234
       </datacite:nameIdentifier>
     </datacite:creator>
   </datacite:creators>

- Esquema xoai

.. code-block:: xml
   :linenos:

    <element name="dc">
      <element name="contributor">
        <element name="author">
          <element name="none">
            <field name="value">Ruiz Muñoz, Francisco</field>
            <field name="authority">755</field>
            <field name="confidence">500</field>
            <field name="orcid_id">0000-0002-7110-3133</field>
          </element>
        </element>
      </element>
    </element>


- Esquema dim

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="contributor" qualifier="author" authority="755" confidence="500" orcid_id="0000-0002-7110-3133">Ruiz Muñoz, Francisco</dim:field>

.. 

Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de investigación reconocidos por MinCiencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------
El campo **Autor (datacite:creator)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+--------------------------------------+
| Esquema de Metadatos | Campo Relacionado                    |
+======================+======================================+
| dc                   | * dc.creator                         |  
|                      | * dc.contributor.author              |   
|                      | * dc.contributor.corporatename       | 
|                      | * dc.contributor.conferencename      |  
+----------------------+--------------------------------------+
| dcterms              | * dcterms.creator                    | 
|                      | * dcterms.contributor.author         | 
|                      | * dcterms.contributor.corporatename  | 
|                      | * dcterms.contributor.conferencename | 
+----------------------+--------------------------------------+
| lom                  | lom.lifecycle.contribute             |
+----------------------+--------------------------------------+
| marcxml              | field:100, 110,111                   |
+----------------------+--------------------------------------+


Niveles semánticos
------------------
- Este campo contempla la utilización de distintos **sistemas de gestión de autoridades de nombre** que normalizan semánticamente los autores. 
- Cada registro presente en estos **sistemas de gestión de autoridades de nombre provee una identificación persistente para cada autor.**
- **Adicionalmente dichos sistemas proveen una URI única que debe ser enlazada y utilizada en el campo de metadatos asociado.**
- **En su mayoría, los sistemas de gestión de autoridades de nombre** contemplan la exportación de registros en representaciones semánticas MADS/SKOS a través de formatos MARCXML, RDF, XML, N3, Turtle, JSON. 

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

+----------------------------------------+-----------------------+----------------+------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Cualificar     | Nota de alcance        |
+========================================+=======================+================+========================+
| Organizational                         | dc.contributor        | corporatename  | * corporate (MODS)     |
|                                        |                       |                | * corpauthor (MARC)    | 
|                                        |                       |                | * CorporateName (MADS) | 
+----------------------------------------+-----------------------+----------------+------------------------+
| Personal                               | dc.contributor        | author         | * PersonalName (MADS)  |
|                                        |                       |                | * personalname (MARC)  |
+----------------------------------------+-----------------------+----------------+------------------------+
| Event                                  | dc.contributor        | conferencename | * meetingname (MARC)   |
|                                        |                       |                | * conference (MODS)    |
|                                        |                       |                | * ConferenceName (MADS)|  
+----------------------------------------+-----------------------+----------------+------------------------+

NOTAS:

  - Los nombre de los calificadores de campos asociados a autor corporativo (**dc.contributor.corporatename**) y autor de evento/conferencia (**dc.contributor.conferencename**) han sido tomados de la ontología MADS provista por la Biblioteca del Congreso de los Estados Unidos (MADS/RDF Ontology - Metadata Authority Description Schema in RDF)
  - DSPACE utiliza por defecto el campo “**dc.contributor.author**” en reemplazo de “**dc.creator**”  y todas sus funcionalidades internas se encuentran asociados a este primer campo.
  - Debido a lo anterior, No es recomendado el uso interno en DSPACE del campo “**dc.creator**” en los formularios de ingreso de datos. En DSPACE cuando el uso de este campo es requerido (Este campo se utiliza principalmente en procesos de cosecha por el protocolo OAI-PMH)es automáticamente convertido desde el campo "**dc.contributor.author**".
  - En DSPACE en la definición de las hojas de entrada que viene por defecto, se utiliza específicamente el campo “**dc.contributor.author**” y en registro de metadatos se muestra el siguiente mensaje asociado al campo “**dc.creator**”: Do not use; only for harvested [#]_
  - Si desea utilizar en DSPACE por defecto el campo “**dc.creator**” se debe cambiar la configuración y varios elementos del código fuente en el software empleado, para que no haya ningún problema durante el proceso de cosecha de metadatos. “Este es un problema muy común que genera rechazos cuando se deben cosechar registros y la transformación se puede hacer a varios niveles: Local, nacional regional” (LaReferencia, 2015).
  - Con el fin de tener un alcance normalizado de las distintas propiedades y atributos (correos, afiliaciones, identificadores, etc..) asociadas a los autores, se recomienda utilizar la configuración de control de autoridades provista por DSPACE ó en su defecto incorporar características de sistema CRIS en DSPACE (**author profiles/ perfiles de autor**).

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

  - En las distintas directrices que han existido, siempre ha sido obligatorio el uso del campo autor aunque no se hace explícito contemplar las diferencias de los distintos tipos y características de los autores.
  - En el sistema DSPACE en su instalación por defecto el campo autor viene con los campos **dc.creator** y **dc.contributor.author** 
  - Se recomienda implementar módulos de gestión de autoridades ó perfiles de usuario en DSPACE para diferenciar claramente la información que describe al recurso de la información que describe al autor del mismo.
  - No es recomendable incorporar como metadatos descriptivos del "**recurso de información**", datos sensibles asociados al autor, como correo del autor, teléfonos, direcciones, afiliaciones, etc..
  - Se recomienda específicamente crear los nuevos atributos/especificadores del campo de autor según la codificación propuesta.


.. [#] https://github.com/DSpace/DSpace/blob/master/dspace/config/registries/dublin-core-types.xml 

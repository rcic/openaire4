.. _dci:creator:

Creator (Creador) (M)
=====================

``datacite:creator``

Definición y alcance del campo
------------------------------

Es la entrada principal, que describe a la entidad(es) responsables por la creación del contenido del recurso. Esta entidad puede ser nombre de persona o corporativo/institucional o evento (Conferencia, reunión, etc.).

En caso de múltiples entidades responsables de la creación del recurso, se debe repetir el elemento tantas veces como sea necesario


Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R): **1-n veces**
Repita este campo para describir todas las entidades responsables de la creación del recurso en **orden prioritario.**

Campo con esquema de metadatos
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

**Clase Principal Autores (creators) (M, 1-n):** Entidad que agrupa todos los autores del recurso.

**Propiedad: Autor (creator) (M, 1-n):** Entidad que identifica cada uno de los autores del recurso.

**Sub-Propiedad: Nombre Completo del Autor (creatorName) (M, 1):** Esta propiedad incluye el texto asociado al autor del recurso en cualquiera de los formas de descripción propuestas. Los nombres de autores que contienen caracteres no romanos deben seguir el esquema de codificación propuesto por  ALA-LC. 

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

Restricciones
-------------
No se debe colocar nombres de colaboradores y editores.


Ejemplos
--------

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

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

..

Atributos de campo
------------------
name type

Especificadores de campo
------------------------
- creatorName
- nameType
- givenName
- familyName 
- nameIdentifier 
- nameIdentifierScheme 
- schemeURI 
- affiliation 

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------
dc.creator

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear en Dspace los siguientes campos:
  
- datacite:creatorName
- datacite:nameType
- datacite:givenName
- datacite:familyName 
- datacite:nameIdentifier 
- datacite:nameIdentifierScheme 
- datacite:schemeURI 
- datacite:affiliation 


Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

- **OpenAIRE 3:** dc.creator
- **BDCOL:** dc.creator.corporativo


.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
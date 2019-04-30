.. _dci:creator:

Creador (M)
===========

``datacite:creator``

Definición y alcance del campo
------------------------------

Es la entrada principal, puede ser nombre de persona o corporativo/institucional. 

Consultar la siguiente información para diligenciar los campos en referencia.

ORCID: http://orcid.org/ 
Siga las siguientes pautas para el ingreso del ORCID: http://support.orcid.org/knowledgebase/articles/116780-structure-of-the-orcid-identifier ISNI: http://www.isni.org/

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R)

Campo con esquema de metadatos
------------------------------
datacite:creator

Traducción al español
---------------------
Creador - Autor

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
---------------------------------------------

**creatorName - Nombre del autor (M):** El formato utilizado debe ser el familiar, los nombres no romanos deben seguir el esquema de la ALA-LC.

**nameType - Tipo de nombre (R):** Hace referencia al nombre personal o de una institución.

**givenName - Nombre personal (R):** Nombre del autor.

**familyName - Apellido del autor (R):** Apellido del autor.

**nameIdentifier - Identificador de nombre (R):** Identifica la forma única de una persona natural o jurídica, según diversos esquemas. 

Se recomienda incluir un identificador de nombre como: 

- ORCID -  Código alfanumérico, no comercial, que identifica de manera única a científicos y otros autores académicos.

- ISNI (International Standard Name Identifier) - Identificador internacional estandarizado de nombre.

**nameIdentifierScheme - Esquema del identificador de nombre (M):** Nombre del esquema identificador. 

**schemeURI - Esquema del identificador de nombre (R):** URI del esquema de identificador de nombre.

**affiliation - Afiliación institucional (R):** Afiliación a la que pertenece el autor. 


Relaciones con otros campos
---------------------------
- Colaborador
- Editor

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
  
datacite:creatorName
datacite:nameType
datacite:givenName
datacite:familyName 
datacite:nameIdentifier 
datacite:nameIdentifierScheme 
datacite:schemeURI 
datacite:affiliation 


Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

- **OpenAIRE 3:** dc.creator
- **BDCOL:** dc.creator.corporativo


.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
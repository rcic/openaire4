.. _dci:contributor:

Colaborador (MA)
================

``datacite:contributor``

Definición y alcance del campo
------------------------------
Es la entrada secundaria, puede ser nombre de persona o corporativo/institucional. 

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio si es aplicable (MA)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R) 

Campo con esquema de metadatos
------------------------------
datacite:contributor

Traducción al español
---------------------
Colaborador

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar el nombre del colaborador con su debida puntuación:

- **creatorName - Nombre del autor (R):** El formato utilizado debe ser el familiar, los nombres no romanos deben seguir el esquema de la ALA-LC.

- **nameType - Tipo de nombre (O):** Hace referencia al nombre personal o de una institución.

- **givenName - Nombre personal (O):** Nombre del autor. Ej: Dueñas Gómez

- **familyName - Apellido del autor (R):** Apellido del autor. Ej: Laureano Felipe

- **nameIdentifier - Identificador de nombre (R):** Identifica la forma única de una persona natural o jurídica, según diversos esquemas. Ej: 0000-0003-3580-8766

Se recomienda incluir un identificador de nombre como: 

		- ORCID -  Código alfanumérico, no comercial, que identifica de manera única a científicos y otros autores académicos.

		- ISNI (International Standard Name Identifier) - Identificador internacional estandarizado de nombre.

- **nameIdentifierScheme - Esquema del identificador de nombre (M):** Nombre del esquema identificador. Ej: ORCID

- **schemeURI - Esquema del identificador de nombre (R):** URI del esquema de identificador de nombre. Ej: https://orcid.org/0000-0003-3580-8766

- **affiliation - Afiliación institucional (R):** Afiliación a la que pertenece el autor. Ej: Universidad Nacional de Colombia. Departamento de Investigaciones.


Valores permitidos (Vocabularios Controlados)
---------------------------------------------

- creatorName 
- nameType 
- givenName 
- familyName 
- nameIdentifier 
- nameIdentifierScheme 
- schemeURI
- affiliation  


Relaciones con otros campos
---------------------------
- Creador
- Editor

Restricciones
-------------
No se debe colocar nombres de creadores y editores. 
 

Ejemplos
~~~~~~~~

.. code-block:: xml
   :linenos:

   <datacite:contributors>
	   <datacite:contributor>
	     <datacite:contributorName>Ramírez, Carlos.</datacite:contributorName>
	   <datacite:contributor>
	   <datacite:contributor>
	     <datacite:contributorName>Departamento Administrativo de Ciencia, Tecnología e Innovación (Colciencias)</datacite:contributorName>
	   </datacite:contributor>
   </datacite:contributors>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

..

Atributos de campo 
------------------

- name type
- contributor type

Especificadores de campo
------------------------

- datacite:creatorName
- datacite:nameType
- datacite:givenName
- datacite:familyName 
- datacite:nameIdentifier 
- datacite:nameIdentifierScheme 
- datacite:schemeURI 
- datacite:affiliation 


Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------
dc.contributor

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


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

- **OpenAIRE 3:** dc.contributor
- **BDCOL:** dc.contributor, dc:contributor.advisor
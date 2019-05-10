.. _aire:fundingReference:

Referencia de financiación (MA)
===============================

``oaire:fundingReference``

Definición y alcance del campo
------------------------------
Institución o Entidad relacionada con el apoyo financiero o la cofinanciación del proyecto y del producto de investigación que se está registrando.  

Los nombres de las instituciones y/o entidades financiadoras y cofinanciadoras deben colocarse completos.

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio si es aplicable (MA)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R)

Campo con esquema de metadatos
------------------------------
oaire:fundingReference

Traducción al español
----------------------
Referencia de financiación

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar el financiador con su debida puntuación:

- **funderName - Nombre del financiador (M):** Nombre del proveedor de financiamiento. Ej: Departamento Administrativo de Ciencia, Tecnología e Innovación. Colciencias

- **funderIdentifier - Identificador único de la entidad financiadora (R):** Número de identificación único de la entidad financiadora. Ej: 0000 0001 2222 4476

- **funderIdentifiertype - Tipo de identificador único de la entidad financiadora (R):** Tipo de identificador de la entidad financiadora. Ej: ISNI

Se recomienda incluir los siguientes identificadores:

    - ISNI (International Standard Name Identifier) - Identificador internacional estandarizado de nombre.

    - GRID (Global Research Identifier Database) - Base de datos de identificadores de investigación global.

    - Crossref Funder - Registro de financiadores https://www.crossref.org/services/funder-registry/

- **fundingStream - Nombre del flujo de financiación (O):** Hace referencia al nombre que se le ha otorgado al flujo de financiación.

- **awardNumber - Número de adjudicación (MA):** Hace referencia al número de adjudicación que se le ha otorgado a la financiación.

- **awardURI - URI del proyecto proporcionada por el patrocinador (R):** La URI de la página de inicio del proyecto proporcionada por el patrocinador para obtener más información sobre el concesión. 

- **awardTitle - Título del proyecto (R):** Título del proyecto, adjudicación o subvención. Ej: Investigación y desplazamiento forzado: reflexiones éticas y metodológicas.


Valores permitidos (Vocabularios Controlados)
---------------------------------------------

- funderName 
- funderIdentifier 
- funderIdentifiertype 
- fundingStream 
- awardNumber 
- awardURI 
- awardTitle

Relaciones con otros campos
---------------------------
Costos de la financiación o cofinanciación 

Restricciones
-------------

Ejemplos
--------

.. code-block:: xml
   :linenos:

   <oaire:fundingReferences>
    <oaire:fundingReference>
     <oaire:funderName>Departamento Administrativo de Ciencia, Tecnología e innovación. Colciencias.</datacite:funderName>
     <oaire:funderIdentifier funderIdentifierType="Crossref Funder ID">http://doi.org/10.13039/100010661</oaire:funderIdentifier>
     <oaire:fundingStream>Horizon 2020 Framework Programme</oaire:fundingStream>
     <oaire:awardNumber awardURI="http://cordis.europa.eu/project/rcn/194062_en.html">643410</oaire:awardNumber>
     <oaire:awardTitle>Open Access Infrastructure for Research in Europe 2020</oaire:awardTitle>
    </oaire:fundingReference>
   </oaire:fundingReferences>

.. _Crossref Funder Registry: http://fundref.org/services/funder-registry

..

Atributos de campo 
------------------
funderIdentifier type

Especificadores de campo
------------------------

- oaire:fundingReference
- oaire:funderName  
- oaire:funderIdentifier  
- oaire:fundingReference.funderIdentifier-isni 
- oaire:fundingReference.funderIdentifier-grid
- oaire:fundingReference.funderIdentifier-crossrefFunderID
- oaire:fundingReference.funderIdentifier-others
- oaire:fundingStream
- oaire:awardNumber 
- oaire:awardTitle

Relaciones con otros modelos de metadatos
-----------------------------------------
Se aplica a los productos que han sido financiados. 

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear en Dspace los siguientes campos:

- oaire:fundingReference
- oaire:funderName  
- oaire:funderIdentifier  
- oaire:fundingReference.funderIdentifier-isni 
- oaire:fundingReference.funderIdentifier-grid
- oaire:fundingReference.funderIdentifier-crossrefFunderID
- oaire:fundingReference.funderIdentifier-others
- oaire:fundingStream
- oaire:awardNumber 
- oaire:awardTitle 


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

- **OpenAIRE 3:** dc:relation
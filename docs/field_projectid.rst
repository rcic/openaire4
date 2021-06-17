.. _aire:fundingReference:

Funding Reference (Referencia de financiación) (MA)
===================================================

``oaire:fundingReference``

Definición y alcance del campo
------------------------------
Es la Institución o Entidad relacionada con el apoyo financiero o la cofinanciación del proyecto y del producto de investigación que se está registrando. Los nombres de las instituciones y/o entidades financiadoras y cofinanciadoras deben colocarse completos y con sus siglas correspondientes. En caso de múltiples entidades responsables del apoyo financiero, se debe repetir el elemento tantas veces como sea necesario.

Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio si es aplicable (MA)

Niveles de ocurrencia (R / NR)
-------------------------------
Repetible (R): **1-n veces.**
..
Repita este campo para describir todas las entidades responsables de financiación en **orden prioritario**

Esquema de metadatos
------------------------------
oaire:fundingReference

Traducción al español
----------------------
Referencia de financiación, financiadores, cofinanciadores.

Forma de Descripción Normalizada (RDA / RCAA2 / ISBD)
-----------------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar el nombre del financiador con su debida puntuación:

  - Para nombres de entidades utilizar el nombre completo tal y como se ha registrado legalmente con su sigla correspondiente de tal forma que la sintaxis sea: “Nombre de la Entidad” + “-” + “Sigla”.
  - Se definen jerarquías en las entidades financiadoras o cofinanciadoras, enumerar las partes de la jerarquía de mayor a menor y separarlas con puntos seguidos de un espacio. Si no queda clara la existencia de una jerarquía, o si se desconoce cuál es la parte más grande y más pequeña del cuerpo, facilitar el nombre de la entidad tal como aparece en la copia electrónica.

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Clase Principal Referencias de Financiación (fundingReferences) (MA, 0-n): 
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Entidad que agrupa todas las entidades que financian proyectos de investigación.

- **Sub-Propiedad: Referencia de Financiación(fundingReference) (MA, 0-n):** Entidad que identifica  específicamente a una entidad que financia proyectos de investigación.

    - **Sub-Propiedad: Nombre del financiador (funderName)  (M, 1):** Nombre del proveedor de financiamiento (Financiador). Ej: Departamento Administrativo de Ciencia, Tecnología e Innovación, MinCiencias.

        - **Sub-Propiedad: Identificador único de la entidad financiadora (funderIdentifier) (R, 0-1):** Número de identificación único de la entidad financiadora. Es una propiedad opcional y única para cada **FundingReference** agregado. Ej: 0000 0001 2222 4476

              - **Atributo: Tipo de identificador único de la entidad financiadora (funderIdentifiertype) (R, 0-1):** Este atributo opcional permite especificar el número estandarizado de la entidad financiadora. Se debe tener en cuenta los siguientes tipos de identificador y su codificación normalizada según el vocabulario controlado propuesto:

              +-------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------+-------+
              | Vocabulario Normalizado | Descripción del Atributo                                                                                                                  | Dominio de Vocabulario           |       |
              +=========================+===========================================================================================================================================+==================================+=======+
              | ISNI                    | Identificador internacional estandarizado de nombre (International Standard Name Identifier ) Norma ISO 27729                             |  (http://www.isni.org)           | oaire |
              +-------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------+-------+
              | GRID                    | Base de datos de identificadores de investigación global (Global Research Identifier Database: GRID)                                      | (https://www.grid.ac/institutes) | oaire |
              +-------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------+-------+
              | Crossref Funder         | Registro de financiadores provisto por CROSSREF (https://search.crossref.org/funding)                                                     | oaire                            |       |
              +-------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------+-------+
              | Local                   | Identificador de institución de investigación colombiana (MinCiencias - Institulac) (https://scienti.MinCiencias.gov.co/institulac2-war/) | redcol                           |       |
              +-------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------+-------+
              | Other                   |                                                                                                                                           | oaire                            |       |
              +-------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+----------------------------------+-------+


        - **Sub-Propiedad: Nombre del flujo de financiación (fundingStream) (O, 0-1):** Esta propiedad de uso opcional, incluye el nombre del flujo o sub-propiedad de financiación. Esta propiedad está pensada como un complemento aclaratorio a la propiedad **funderName.**

        **NOTAS:**

        Para el caso de proyectos financiados por MinCiencias, este atributo debe contener los Programas Nacionales de MinCiencias, cuyos valores y descripción se presentan a continuación:

+--------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Programas Nacionales de CTel                                                                                       | Descripción                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+====================================================================================================================+================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================+
| `Programa Nacional de CTeI en Geociencias <https://www.MinCiencias.gov.co/node/1120>`_                             | Promover la generación de nuevo conocimiento geocientífico y el aprovechamiento del existente, el fortalecimiento de las capacidades de CTeI en el área de las geociencias a través de la investigación multidisciplinar y de la formulación de políticas, programas, proyectos, planes y estrategias, la apropiación social del conocimiento geocientífico del territorio nacional y el aprovechamiento racional y ambientalmente sostenible de los recursos.                                                                                                 |
+--------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| `Programa Nacional de CTeI en Salud <https://www.MinCiencias.gov.co/node/1113>`_                                   | Gestionar la ciencia, la tecnología y la innovación en el sector salud como soporte para la formulación de políticas y fortalecimiento de las capacidades científicas y tecnológicas del país que puedan responder a necesidades de desarrollo, prioridades del conocimiento y expectativas de la población.                                                                                                                                                                                                                                                   |
+--------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| `Programa Nacional en Ambiente, Biodiversidad y Hábitat <https://www.MinCiencias.gov.co/node/1122>`_               | Formular las políticas, planes, programas y estrategias con el fin de promover, fomentar y consolidar la generación, uso y apropiación del conocimiento, que apoye al logro de las metas nacionales y sectoriales, en relación a la gestión ambiental, la Biodiversidad y los asentamientos humanos, como parte del desarrollo sostenible de Colombia.                                                                                                                                                                                                         |
+--------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| `Programa Nacional en Ciencias Agropecuarias <https://www.MinCiencias.gov.co/node/1126>`_                          | Liderar la formulación de las políticas, planes, programas y estrategias de I+D+i, para el sector agropecuario y agroindustrial, que garanticen el aumento de su productividad y competitividad, en un contexto de uso eficiente y sostenible de los recursos naturales.                                                                                                                                                                                                                                                                                       |
+--------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| `Programa Nacional en Ciencias Básicas <https://www.MinCiencias.gov.co/node/1119>`_                                | Formular e implementar la política científica nacional y contribuir a fomentar la generación de nuevo conocimiento en las áreas de biología, física, química, matemáticas y básicas biomédicas, promoviendo su inserción en el contexto internacional. Las Ciencias Básicas se constituyen en la base fundamental de los procesos de desarrollo científico y tecnológico, sin los cuales es impensable la inserción del país en las dinámicas globales de desarrollo.                                                                                          |
+--------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| `Programa Nacional en Ciencias del Mar y los recursos hidrobiológicos <https://www.MinCiencias.gov.co/node/1123>`_ | Formular las políticas, planes, programas y estrategias con el fin de promover, fomentar y consolidar la generación, uso y apropiación del conocimiento, que apoye el logro de las metas nacionales y sectoriales, para el desarrollo sostenible del océano, los espacios costeros y fluviales del país.                                                                                                                                                                                                                                                       |
+--------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| `Programa Nacional en Ciencias Humanas, Sociales y Educación <https://www.MinCiencias.gov.co/node/1121>`_          | Formular, asesorar y realizar políticas y actividades de CTeI que propendan, desde las ciencias sociales y las humanidades, por la generación de conocimiento tanto disciplinar como para la solución de problemas de la sociedad colombiana, mediante el trabajo interdisciplinario con aliados.                                                                                                                                                                                                                                                              |
+--------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| `Programa Nacional en Energía y Minería <https://www.MinCiencias.gov.co/node/1124>`_                               | Generar políticas que promuevan la ciencia, la tecnología y la innovación en el sector minero energético, en coherencia con las políticas sectoriales, así como fomentar la generación de conocimiento científico y tecnológico que contribuya al desarrollo sostenible del sector minero energético.                                                                                                                                                                                                                                                          |
+--------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| `Programa Nacional en Ingeniería <https://www.MinCiencias.gov.co/node/1128>`_                                      | Generar políticas públicas para promover al avance de la I+D en Ingeniería, con enfoques que integren miradas interdisciplinarias e igualmente fomentar la generación de conocimiento científico y tecnológico que aporte desde la Ingeniería a la solución de problemáticas de los entornos sociales y productivos del país.                                                                                                                                                                                                                                  |
+--------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| `Programa Nacional en Seguridad y Defensa <https://www.MinCiencias.gov.co/node/1130>`_                             | Generar capacidades nacionales para la creación, transferencia y uso de conocimiento en el sector, a partir de la integración de las Fuerzas Armadas y la Sociedad, en la búsqueda del desarrollo de tecnologías duales (civiles y militares) y otras acciones, que contribuyan tanto al desarrollo económico nacional, como a la consolidación de capacidades estratégicas, tácticas y operacionales de actores del sector, encaminadas a proteger la soberanía y la integridad territorial con el fin de establecer un ambiente de seguridad en la sociedad. |
+--------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
**Tabla tomada de:** https://www.MinCiencias.gov.co/investigadores/programas-nacionales-ctei

+--------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Apropiación social | Descripción                                                                                                                                                                                                                                                                                                                                                                                               |
+====================+===========================================================================================================================================================================================================================================================================================================================================================================================================+
| A Ciencia cierta   | Es una estrategia de Apropiación Social del Conocimiento en innovación social de MinCiencias que reconoce las mejores experiencias desarrolladas por las comunidades haciendo uso de recursos científicos o tecnológicos, para dar solución a un problema o necesidad específica de su entorno, las cuales pueden ser compartidas y replicadas por otros ciudadanos para el beneficio de sus comunidades. |
+--------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

..


+-----------------------------------------------------+
| Otros Programas                                     |
+=====================================================+
| Programa de Cienciometría (Grupos, Pares y Centros) |
+-----------------------------------------------------+
| Programa de Difusión                                |
+-----------------------------------------------------+
| Programa Ideas Para El Cambio                       |
+-----------------------------------------------------+
| Programa Jóvenes Investigadores                     |
+-----------------------------------------------------+
| Programa Nexo Global                                |
+-----------------------------------------------------+
| Programa Ondas                                      |
+-----------------------------------------------------+
| Proyecto Colombia Bio                               |
+-----------------------------------------------------+
| Red Nacional de Información Científica              |
+-----------------------------------------------------+


..

        - **Sub-Propiedad: Número de adjudicación (awardNumber) (O, 1):** Esta propiedad de uso opcional, incluye el número de adjudicación exclusivamente al nombre de la entidad. Esta propiedad está pensada como un complemento aclaratorio a la propiedad funderName.
          
          **NOTAS:**
            - Para el caso de proyectos financiados por MinCiencias, este atributo debe contener el  número de contrato del proyecto de investigación para proyectos financiados.
 
          - **Atributo: URI de adjudicación (arwardURI) (R, 0-1):** Este atributo permite especificar la URI de la página del proyecto proporcionada por el patrocinador para obtener más información de la adjudicación,  concesión ó  financiamiento (grant).
 
        - **Sub-Propiedad: Proyecto de Investigación / Título de adjudicación (awardTitle) (R, 0-n):** Esta propiedad de uso opcional, incluye el nombre del proyecto, adjudicación o subvención.
 
           - **Atributo: ID del Proyecto de Investigación (arwardID) (R, 0-1):** Este atributo permite especificar un identificador normalizado asignado al proyecto de investigación.
		   
        - **Sub-Propiedad: Línea de Investigación  (researchArea) (R, 0-n):** Esta propiedad de uso opcional, incluye el nombre de la línea de investigación relacionada.
 
           - **Atributo: ID de la Línea de Investigación (researchAreaID) (R, 0-1):** Este atributo permite especificar un identificador normalizado asignado a la línea de investigación.

        - **Sub-Propiedad: Grupo de Investigación  (researchGroup) (R, 0-n):** Esta propiedad de uso opcional, incluye los nombres de los grupos de investigación relacionados.
 
           - **Atributo: ID de la Línea de Investigación (researchGroupID) (R, 0-1):** Este atributo permite especificar un identificador normalizado asignado a cada grupo de investigación.

        - **Sub-Propiedad: Costo del proyecto (researchCost) (R, 0-n):** Esta propiedad de uso opcional, incluye el costo (subvención) del proyecto asociado. Hace referencia al factor económico o a los recursos económicos utilizados para llevar a cabo el proyecto de investigación.
		
		

Relaciones con otros campos
---------------------------

  - No debe confundirse la **referencia de financiación (oaire: fundingReference)** del recurso con la entidad responsable de la **publicación (dc.publisher)** del mismo.
  - No debe confundirse la **referencia de financiación (oaire:fundingReference)** del recurso con el **creador (dc.creator)** del recurso  y/o **colaborador (dc.contributor) – (dc.contributor.corporatename).**
  - No debe confundirse la **referencia de financiación (oaire:fundingReference)** del recurso con la descripción del patrocinador **(dc.description.sponsorship)** ó las indicaciones detalladas del patrocinio **(dc.description.funder).**

Restricciones
-------------
No Aplica

Ejemplos y ayudas
-----------------

Ayudas
++++++

- Ej: Departamento Administrativo de Ciencia, Tecnología e Innovación – MinCiencias. **Nombre del Financiador:** Entidad financiadora del proyecto de investigación.  
- Ej: **(fundingStream):** Programa Nacional de Ciencia, Tecnología e Innovación Agropecuaria
- Ej: **(fundingStream):** Programa Nacional de CTel en Salud.
- Ej **(ISNI):** 0000 0001 0130 4813
- Ej: **(CrossrefFunder):** http://doi.org/10.1023/a:1010537606969
- Ej: **(awardNumber):** 0005-2013. Número del contrato del proyecto. 
- Ej: **(awardCost):** $50.000.000. Costo del proyecto.


Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++
 
**Esquema xml**

.. code-block:: xml
   :linenos:

    <fundingReferences>
      <fundingReference>
        <funderName>Universidad Nacional de Colombia</funderName>
        <funderIdentifier  funderIdentifiertype="GRID">grid.10689.36</funderIdentifier>
        <awardNumber>15TET-40582</ awardNumber >
        <awardTitle>Sistemas de Información</awardTitle>
      </fundingReference>
    </fundingReferences>



**Esquema DataCite - Oaire**

.. code-block:: xml
   :linenos:

   <oaire:fundingReferences>
    <oaire:fundingReference>
      <oaire:funderName>Departamento Administrativo de Ciencia, Tecnología e innovación - MinCiencias.</datacite:funderName>
      <oaire:funderIdentifier funderIdentifierType="Crossref Funder ID" > http://doi.org/10.1023/a:1010537606969</oaire:funderIdentifier>
      <oaire:fundingStream>Programa Nacional de Ciencia, Tecnología e Innovación Agropecuaria</oaire:fundingStream>
    </oaire:fundingReference>
   </oaire:fundingReferences>


**Esquema oai_dc**

.. code-block:: xml
   :linenos:

    <dc:relation>info:eu-repo/grantAgreement/MINECO [CTQ2014-52769-C3-R-1, CTQ2014-62234-EXP, CTQ2015-70795-P, CTQ2014-54306-P, CTQ2014-52525P]</dc:relation>
    <dc:relation>info:eu-repo/grantAgreement/Junta de Andalucia [P10-FQM-06292]</dc:relation>

**Esquema xoai**

.. code-block:: xml
   :linenos:

    <element name="sponsorship">
    <element name="spa">
      <field name="value">Support for this work was provided by the MINECO (CTQ2014-52769-C3-R-1, CTQ2014-62234-EXP, CTQ2015-70795-P, CTQ2014-54306-P, and CTQ2014-52525P), and the Junta de Andalucia (P10-FQM-06292). A.C. thanks Junta de Andalucia for a research contract. M.C. acknowledges an ICREA Academia Award, 2014 SGR 862 from Generalitat de Catalunya, and ERC-239910.</field>
    </element>
    </element>

    <element name="projectID">
    <element name="spa">
      <field name="value">info:eu-repo/grantAgreement/MINECO [CTQ2014-52769-C3-R-1, CTQ2014-62234-EXP, CTQ2015-70795-P, CTQ2014-54306-P, CTQ2014-52525P]</field>
    </element>


..

Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de investigación reconocidos por MinCiencias.


Relaciones con otros modelos de metadatos
-----------------------------------------
El campo Referencia de Financiación **(oaire:fundingReference)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+---------------------------------+
| Esquema de Metadatos | Campo Relacionado               |
+======================+=================================+
| dc                   | dc.relation.projectID           |
+----------------------+---------------------------------+
| dcterms              | dcterms.description.sponsorship |
+----------------------+---------------------------------+
| marcxml              | field: 536                      |
+----------------------+---------------------------------+

Niveles semánticos
------------------

- Este campo contempla la utilización de distintos sistemas de gestión de autoridades de nombre que normalizan semánticamente las instituciones que financian proyectos de investigación (Principalmente VIAF, ISNI, GRID, CROSSREF, InstituLAC).
- En el ámbito del nombre del campo **funderIdentifiertype,** se recomienda utilizar los valores autorizados provistos.

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:


**DSPACE 6.X o anteriores**

+-------------------------------------------+---------------------+-----------------------+----------------------+----------------------+
| Descripción                               | Modelo de Metadatos | Campo Elemento DSPACE | Calificadores        | Propiedades          |
+===========================================+=====================+=======================+======================+======================+
| Nombre del financiador                    | oaire               | fundername            |                      |                      |
+-------------------------------------------+---------------------+-----------------------+----------------------+----------------------+
| Identificador de financiador              | oaire               | funderidentifier      | - ISNI               | funderIdentifiertype |
|                                           |                     |                       | - GRID               |                      |
|                                           |                     |                       | - Crossref Funder    |                      |
|                                           |                     |                       | - Local              |                      |
|                                           |                     |                       | - Other              |                      |
+-------------------------------------------+---------------------+-----------------------+----------------------+----------------------+
| Especificación de la financiación         | oaire               | fundingstream         |                      |                      |
| - Programa Nacional de CTel MinCiencias)  |                     |                       |                      |                      |
+-------------------------------------------+---------------------+-----------------------+----------------------+----------------------+
| Identificador de la financiación          | oaire               | awardnumber           |                      | arwardURI            |
+-------------------------------------------+---------------------+-----------------------+----------------------+----------------------+
| Nombre de la convocatoria de financiación | oaire               | awardtitle            |                      | awardtitleID         |
| Nombre Proyecto de Investigación          |                     |                       |                      |                      |
+-------------------------------------------+---------------------+-----------------------+----------------------+----------------------+
| Línea de Investigación                    | dc.description      | researcharea          |                      | researchareaID       |
+-------------------------------------------+---------------------+-----------------------+----------------------+----------------------+
| Grupo de Investigación                    | dc.contributor      | researchgroup         |                      | researchGroupID      |
+-------------------------------------------+---------------------+-----------------------+----------------------+----------------------+
| Semillero de Investigación                | dc.contributor      | researchhotbed        |                      |                      | +-------------------------------------------+---------------------+-----------------------+----------------------+----------------------+
| Costos (subvenciones) del proyecto        | dc.description      | researchcost          |                      |                      |
+-------------------------------------------+---------------------+-----------------------+----------------------+----------------------+

**DSPACE 7.X o superior**

- Se debe utilizar la entidad **funding** provista en el ámbito del sistema CRIS

**NOTA:**

- DSPACE 7.X y superior, permite la gestión avanzada de propiedades, sub-propiedades y atributos de campo asociado a entidades predefinidas.

- DSPACE CRIS  incluye la definición de una entidad llamada FUNDING que es compatible con DATACITE.

- Para las instituciones que poseen DSPACE en versión 6.X o inferior, se recomienda crear los campos indicados anteriormente y poder ingresar información detallada de la institución patrocinadora.

- Adicionalmente a los campos normalizados indicados anteriormente, se recomienda hacer una descripción general de la fuente de financiación a través de los siguientes campos:

    - **dc.description.sponsorship:** información sobre agencias patrocinadoras 
    - **dc.description.funder:** Indicaciones del patrocinio y datos específicos de financiación. 


Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

- Se recomienda específicamente crear los nuevos atributos/especificadores del campo de referencia de financiación según la codificación propuesta.
- En las directrices Driver 2.0 y Open Aire 3.0 fue introducido el campo **grantAgreement (Algunos DSPACE almacenan esta información en dc.relation.projectID)** con información asociada al vocabulario info:eu-repo/grantAgreement 
- Se considera obsoleto el uso de estructuras de campos que contengan  (info:eu-repo)  en favor de la utilización del campo **fundingReference** con sus propiedades y atributos relacionados **que está definido en el esquema de metadatos de DataCite MetadataKernel**
- Adicionalmente se agrega la propiedad **fundingStream** a este perfil de aplicación.
- En el caso que se haya utilizado algún campo siguiendo la estructura  de espacios de nombre para describir la información de financiación del proyecto:  info:eu-repo/grantAgreement/Funder/FundingProgram/ProjectNumber/Jurisdiction/ProjectName/ProjectAcronym/, la equivalencia de campo debe ser:
  
+----------------+-------------------------+
| OpenAIRE 3.X   | OpenAire 4.X / Datacite |
+================+=========================+
|                | funderIdentifier        |
+----------------+-------------------------+
| Funder         | funderName              |
+----------------+-------------------------+
| FundingProgram | fundingStream           |
+----------------+-------------------------+
| ProjectNumber  | awardNumber             |
+----------------+-------------------------+
| ProjectName    | awardTitle              |
+----------------+-------------------------+
|                | awardURI                |
+----------------+-------------------------+
| ProjectAcronym |                         |
+----------------+-------------------------+
| Jurisdiction   |                         |
+----------------+-------------------------+

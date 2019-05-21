.. _aire:fundingReference:

Funding Reference (Referencia de financiación) (MA)
===================================================

``oaire:fundingReference``

Definición y alcance del campo
------------------------------
Es la Institución o Entidad relacionada con el apoyo financiero o la cofinanciación del proyecto y del producto de investigación que se está registrando.  
 
Los nombres de las instituciones y/o entidades financiadoras y cofinanciadoras deben colocarse completos y con sus siglas correspondientes.
 
En caso de múltiples entidades responsables del apoyo financiero, se debe repetir el elemento tantas veces como sea necesario.

Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio si es aplicable (MA)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R): **1-n veces**
Repita este campo para describir todas las entidades responsables de financiación en **orden prioritario.**

Esquema de metadatos
------------------------------
oaire:fundingReference
**Nota:** Este campo se ha adaptado del esquema de metadatos DATACITE MetadataKernel versión 4.1 (http://doi.org/10.5438/0014), el cual es utilizado ampliamente para la gestión de documentos y datos.

Traducción al español
----------------------
Referencia de financiación, financiadores, cofinanciadores.

Forma de Descripción Normalizada (RDA / RCAA2 / ISBD)
-----------------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar el financiador con su debida puntuación:

  - Para nombres de entidades utilizar el nombre completo tal y como se ha registrado legalmente con su sigla correspondiente de tal forma que la sintaxis sea: “Nombre de la Entidad” + “-” + “Sigla”.

  - Se definen jerarquías en las entidades financiadoras o cofinanciadoras, enumerar las partes de la jerarquía de mayor a menor y separarlas con puntos seguidos de un espacio. Si no queda clara la existencia de una jerarquía, o si se desconoce cuál es la parte más grande y más pequeña del cuerpo, facilitar el nombre de la entidad tal como aparece en la copia electrónica.

Propiedades, atributos y especificadores de campo
-------------------------------------------------

**funderName - Nombre del financiador (M) (M, 1-n):** Nombre del proveedor de financiamiento. Ej: Departamento Administrativo de Ciencia, Tecnología e Innovación, Colciencias.

**funderIdentifier - Identificador único de la entidad financiadora (R) (M, 1-n):** Número de identificación único de la entidad financiadora. Ej: 0000 0001 2222 4476

**funderIdentifiertype - Tipo de identificador único de la entidad financiadora (R) (M, 1-n):** Tipo de identificador de la entidad financiadora. Ej: ISNI

**fundingStream - Nombre del flujo de financiación (O) (M, 1-n):** Hace referencia al nombre que se le ha otorgado al flujo de financiación.

**awardNumber - Número de adjudicación (MA) (M, 1-n):** Hace referencia al número de adjudicación que se le ha otorgado a la financiación.

**awardURI - URI del proyecto proporcionada por el patrocinador (R) (M, 1-n):** La URI de la página de inicio del proyecto proporcionada por el patrocinador para obtener más información sobre la concesión.

**awardTitle - Título del proyecto (R) (M, 1-n):** Título del proyecto, adjudicación o subvención. Ej: Investigación y desplazamiento forzado: reflexiones éticas y metodológicas.
 
**Atributo: Tipo de identificador único de la entidad financiadora (funderIdentifiertype) (O, 0-1):** Este atributo permite especificar el número estandarizado de la entidad financiadora. Se debe tener en cuenta los siguientes tipos de identificador y su codificación normalizada según el vocabulario controlado propuesto:

+-------------------------+----------------------------------------------------------+------------------------+
| Vocabulario Normalizado | Descripción del Atributo                                 | Dominio de Vocabulario |
+=========================+==========================================================+========================+
| ISNI                    | Identificador internacional estandarizado de nombre      | oaire                  |
+-------------------------+----------------------------------------------------------+------------------------+
| GRID                    | Base de datos de identificadores de investigación global | oaire                  |
+-------------------------+----------------------------------------------------------+------------------------+
| Crossref Funder         | Registro de financiadores                                | oaire                  |
+-------------------------+----------------------------------------------------------+------------------------+

**Sub-Propiedad: Financiamiento (Funding stream) (O, 0-1):** Esta propiedad de uso opcional, incluye el nombre del flujo o sub-propiedad de financiación.
Esta propiedad está pensada como un complemento aclaratorio a la propiedad funderName.
 
**Sub-Propiedad: Número de adjudicación (awardNumber) (O, 0-1):** Esta propiedad de uso opcional, incluye el número de adjudicación exclusivamente al nombre de la entidad. Esta propiedad está pensada como un complemento aclaratorio a la propiedad funderName.
 
**Atributo: URI de adjudicación (arwardURI) (O, 0-1):** Este atributo permite especificar la URI de la página de inicio del proyecto proporcionada por el patrocinador para obtener más información de la adjudicación o concesión.
 
**Sub-Propiedad: Título de adjudicación (awardTitle) (O, 0-n):** Esta propiedad de uso opcional, incluye el título del proyecto, adjudicación o subvención.


Relaciones con otros campos
---------------------------
  - No debe confundirse la **referencia de financiación (oaire: fundingReference)** del recurso con la entidad responsable de la publicación (dc.publisher) del mismo.
  - No debe confundirse la **referencia de financiación (oaire:fundingReference)** del recurso con el **creador (dc.creator)** del recurso  y/o **colaborador (dc.contributor) – (dc.contributor.corpauthor).** Costos de la financiación o cofinanciación 

Restricciones
-------------
No Aplica

Ejemplos y ayudas
-----------------

**Ayudas**

  - **Nombre del Financiador:** Entidad financiadora del proyecto de investigación.  
  - Ej: Departamento Administrativo de Ciencia, Tecnología e Innovación – Colciencias.
  - Ej (ISNI): 0000 0001 0130 4813
  - Ej: (Crossref Funder): http://doi.org/10.1023/a:1010537606969
  - Ej: (fundingStream): Programa Nacional de Ciencia, Tecnología e Innovación Agropecuaria

**Ejemplo en XML (Interoperabilidad OAI-PMH)**
 
**Esquema oai_dc**

.. code-block:: xml
   :linenos:

**Esquema DataCite - Oaire**

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

**Esquema xoai**

.. code-block:: xml
   :linenos:

**Esquema xoai**

.. code-block:: xml
   :linenos:


..

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de investigación reconocidos por Colciencias.


Relaciones con otros modelos de metadatos
-----------------------------------------
El campo Referencia de Financiación (oaire:fundingReference) es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+----------------------------+
| Esquema de Metadatos | Campo Relacionado          |
+======================+============================+
| dc                   | dc.description.sponsorship |
|                      | dc.description.funder      |
+----------------------+----------------------------+
| marcxml              | field: 536                 |
+----------------------+----------------------------+

Niveles semánticos
------------------
  - Este campo contempla la utilización de distintos **sistemas de gestión de autoridades de nombre** que normalizan semánticamente los autores.
  - Cada registro presente en estos **sistemas de gestión de autoridades de nombre provee una Identificación persistente.**
  - Adicionalmente dichos sistemas proveen una URI única que debe ser enlazada y utilizada en el campo de metadatos asociado.
  - En su mayoría, los sistemas de gestión de autoridades de nombre contemplan la exportación de registros en representaciones semánticas MADS/SKOS a través de formatos MARCXML, RDF, XML, N3, Turtle, JSON.


Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

+----------------------------------------+-----------------------+-------------+--------------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Cualificar  | Nota de alcance                |
+========================================+=======================+=============+================================+
| Nombre del financiador                 | description           | sponsorship | funderNameCorporateName (MADS) |
+----------------------------------------+-----------------------+-------------+--------------------------------+

NOTAS:

- Los nombre de los cualificadores/especificadores de campos asociados a la Referencia de Financiación (oaire:fundingReference) y Nombre del Financiador (funderName) han sido tomados de la ontología MADS provista por la Biblioteca del Congreso de los Estados Unidos (MADS/RDF Ontology - Metadata Authority Description Schema in RDF)
- Si desea utilizar en DSPACE por defecto el campo “dc. description.sponsorship” se debe la configuración en el software empleado, para que no haya ningún problema durante el proceso de cosecha de metadatos. “Este es un problema muy común que genera rechazos cuando se deben cosechar registros y la transformación se puede hacer a varios niveles: Local, nacional regional” (LaReferencia, 2015).
- Con el fin de tener un alcance normalizado de las distintas propiedades y atributos (correos, afiliaciones, identificadores, etc.) asociadas a las entidades, se recomienda utilizar la configuración de control de autoridades provista por DSPACE o en su defecto incorporar características de sistema CRIS en DSPACE.


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

- Se recomienda específicamente crear los nuevos atributos/especificadores del campo de referencia de financiación según la codificación propuesta.
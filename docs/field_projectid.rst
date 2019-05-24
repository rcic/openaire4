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

Clase Principal Referencias de Financiación (fundingReferences) (M, 1-n): 
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Entidad que agrupa todas las entidades que financian proyectos de investigación.

Sub-Propiedad: Referencia de Financiación(fundingReference) (MA, 0-n): 
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Entidad que identifica  entidades que financian proyectos de investigación.

  - **Sub-Propiedad: Nombre del financiador (funderName) - (M) (O, 1-n):** Nombre del proveedor de financiamiento. Ej: Departamento Administrativo de Ciencia, Tecnología e Innovación, Colciencias.

  - **Sub-Propiedad: Identificador único de la entidad financiadora (funderIdentifier)  (R) (O, 1-n):** Número de identificación único de la entidad financiadora. Ej: 0000 0001 2222 4476

      - **Atributo: Tipo de identificador único de la entidad financiadora (funderIdentifiertype) (O, 0-1):** Este atributo permite especificar el número estandarizado de la entidad financiadora. Se debe tener en cuenta los siguientes tipos de identificador y su codificación normalizada según el vocabulario controlado propuesto:

          +-------------------------+----------------------------------------------------------+------------------------+
          | Vocabulario Normalizado | Descripción del Atributo                                 | Dominio de Vocabulario |
          +=========================+==========================================================+========================+
          | ISNI                    | Identificador internacional estandarizado de nombre      | oaire                  |
          +-------------------------+----------------------------------------------------------+------------------------+
          | GRID                    | Base de datos de identificadores de investigación global | oaire                  |
          +-------------------------+----------------------------------------------------------+------------------------+
          | Crossref Funder         | Registro de financiadores                                | oaire                  |
          +-------------------------+----------------------------------------------------------+------------------------+

  - **Sub-Propiedad: Nombre del flujo de financiación (fundingStream) (O) (O, 1-n):** Esta propiedad de uso opcional, incluye el nombre del flujo o sub-propiedad de financiación. Esta propiedad está pensada como un complemento aclaratorio a la propiedad funderName.

  - **Sub-Propiedad: Número de adjudicación (awardNumber) (O, 0-1):** Esta propiedad de uso opcional, incluye el número de adjudicación exclusivamente al nombre de la entidad. Esta propiedad está pensada como un complemento aclaratorio a la propiedad funderName.
 
  - **Atributo: URI de adjudicación (arwardURI) (O, 0-1):** Este atributo permite especificar la URI de la página del proyecto proporcionada por el patrocinador para obtener más información de la adjudicación o concesión.
 
  - **Sub-Propiedad: Título de adjudicación (awardTitle) (O, 0-n):** Esta propiedad de uso opcional, incluye el título del proyecto, adjudicación o subvención.


Relaciones con otros campos
---------------------------
  - No debe confundirse la **referencia de financiación (oaire: fundingReference)** del recurso con la entidad responsable de la publicación (dc.publisher) del mismo.
  - No debe confundirse la **referencia de financiación (oaire:fundingReference)** del recurso con el **creador (dc.creator)** del recurso  y/o **colaborador (dc.contributor) – (dc.contributor.corpauthor).** Costos de la financiación o cofinanciación 

Restricciones
-------------
No Aplica

Ejemplos y ayudas
-----------------

Ayudas
++++++

  - **Nombre del Financiador:** Entidad financiadora del proyecto de investigación.  
  - Ej: Departamento Administrativo de Ciencia, Tecnología e Innovación – Colciencias.
  - Ej (ISNI): 0000 0001 0130 4813
  - Ej: (Crossref Funder): http://doi.org/10.1023/a:1010537606969
  - Ej: (fundingStream): Programa Nacional de Ciencia, Tecnología e Innovación Agropecuaria

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++
 
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
El campo Referencia de Financiación **(oaire:fundingReference)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

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


Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

+-------------------------------------------+-----------------------+------------------+--------------------------------+
| Vocabulario controlado OpenAire/RedCol    | Campo Elemento DSPACE | Cualificar       | Nota de alcance                |
+===========================================+=======================+==================+================================+
| Nombre del financiador                    | dc.description        | sponsorship      | campo equivalente a funderName |
+-------------------------------------------+-----------------------+------------------+--------------------------------+
| Identificador de financiador              | dc.description        | funderIdentifier |                                |
+-------------------------------------------+-----------------------+------------------+--------------------------------+
| Especificación de la financiación         | dc.description        | fundingStream    |                                |
+-------------------------------------------+-----------------------+------------------+--------------------------------+
| Identificador de la financiación          | dc.description        | awardNumber      |                                |
+-------------------------------------------+-----------------------+------------------+--------------------------------+
| Nombre de la convocatoria de financiación | dc.description        | awardTitle       |                                |
+-------------------------------------------+-----------------------+------------------+--------------------------------+

**NOTA:**

- DSPACE en su versión 7.0 permite la gestión avanzada de propiedades, subpropiestades y atributos de campo.
- DSPACE CRIS  incluye la definición de una entidad llamada FUNDING que es compatible con DATACITE.
- Para las instituciones que poseen DSPACE en versión 6.X o inferior, se recomienda crear los campos indicados anteriormente y poder ingresar información detallada de la institución patrocinadora. 


Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

- Se recomienda específicamente crear los nuevos atributos/especificadores del campo de referencia de financiación según la codificación propuesta.
- En las directrices Driver 2.0 y Open Aire 3.0 fue introducido el campo **grantAgreement (Algunos DSPACE almacenan esta información en dc.relation.projectID)** con información asociada al vocabulario info:eu-repo/grantAgreement 
- Esta directriz deja obsoleto este campo en favor de la utilización del campo y las subpropiedades denominada  FinanceReference que está definido en el esquema de metadatos de DataCite MetadataKernel
- Adicionalmente se agrega la propiedad fundingStream a este perfil de aplicación.

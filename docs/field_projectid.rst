.. _aire:referenciaFinanciacion:

Referencia de financiación (MA)
===============================

``oaire:referenciaFinanciación``

Cardinalidad
~~~~~~~~~~~~

*Obligatoria si aplica*

*Ocurrencia: 0-n*

Definición y instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Información sobre el apoyo financiero (financiación) para el recurso que se está registrando.

**Instrucciones de uso**

.. include:: projectid.rst

**Observaciones**

* introducido como ``info:eu-repo/grantAgreement`` en versiones anteriores de las pautas o directrices de OpenAIRE
* adoptando elementos y subpropiedades de referenciaFiananciación desde DataCite MetadataKernel v4.1 que reemplaza la sintaxis de ``info:eu-repo/grantAgreement``.
* agregar subpropiedad flujoFinanciación a este perfil de aplicación.

Propiedad referenciaFinanciación (MA, 0-n)
-------------------------------------------

Repita esta propiedad para indicar varios financiadores y proyectos diferentes.

Subpropiedad nombreFundador (M)
-------------------------------

Nombre del proveedor del financiamiento (ocurrencia: 1). Obligatoria si *referenciaFinanciación* es usada.

Subpropiedad identificadorFondos (R)
------------------------------------

Identificador unico de la entidad financiadora (ocurrencia: 0-1).

Atributo tipoIdentificadorfondo (R)
***********************************

Tipo de identificador único de la entidad financiadora (ocurrencia: 0-1).

.. include:: vocabularies/funderidentifiertype.rst

además ver `Crossref Funder Registry`_

Subpropiedad flujoFinanciación (O)
----------------------------------

Nombre del flujo de financiación (opcional) (ocurrencia: 0-1).

Subpropiedad númeroAdjudicación (MA)
------------------------------------

Proyecto idSubvención or númeroAdjudicación (ocurrencia: 1).

Atributo URIadjudicación (R)
****************************

URI de la página de inicio del proyecto proporcionada por el financiador para obtener más información sobre la adjudicación (subvención) (ocurrencia: 0-1). 

Subpropiedad títuloAdjudicación (R)
-----------------------------------

Título del proyecto, adjudicación o subvención (ocurrencia: 0-1).


Ejemplo
~~~~~~~

Un ejemplo utilizando todos los campos:

.. code-block:: xml
   :linenos:

   <oaire:fundingReferences>
    <oaire:fundingReference>
     <oaire:funderName>European Commission</datacite:funderName>
     <oaire:funderIdentifier funderIdentifierType="Crossref Funder ID">http://doi.org/10.13039/100010661</oaire:funderIdentifier>
     <oaire:fundingStream>Horizon 2020 Framework Programme</oaire:fundingStream>
     <oaire:awardNumber awardURI="http://cordis.europa.eu/project/rcn/194062_en.html">643410</oaire:awardNumber>
     <oaire:awardTitle>Open Access Infrastructure for Research in Europe 2020</oaire:awardTitle>
    </oaire:fundingReference>
   </oaire:fundingReferences>

.. _Crossref Funder Registry: http://fundref.org/services/funder-registry
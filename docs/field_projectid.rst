.. _aire:fundingReference:

Referencia de financiación (MA)
===============================

``oaire:referenciaFinanciación``

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

Valores permitidos (Vocabularios Controlados)
---------------------------------------------
funderIdentifier type

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
     <oaire:funderName>European Commission</datacite:funderName>
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
Niveles de aplicación para productos de investigación de Colciencias
Se aplica a los productos que han sido financiados. 

Relaciones con otros modelos de metadatos
-----------------------------------------

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

- **OpenAIRE 3:** dc:relation
.. _aire:fundingReference:

Referencia de financiación (MA)
===============================

``oaire:referenciaFinanciación``

Nombre del campo
----------------

Campo normalizado:
~~~~~~~~~~~~~~~~~~
fundingReference

Campo con esquema de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
oaire:fundingReference

Traducción al español:
~~~~~~~~~~~~~~~~~~~~~~
Referencia de financiación

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio si es aplicable (MA)

Niveles de Ocurrencia (R/NR - Cantidad Veces)
---------------------------------------------
Repetible (R)

Definición y Alcance del campo
------------------------------
Información relacionada con el apoyo financiero o la financiación del proyecto y del producto que se está registrando.  

Forma de Descripción Normalizada (RDA/RCAA2)
-----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
funderIdentifier 

Relaciones con otros campos
~~~~~~~~~~~~~~~~~~~~~~~~~~~
Creador
Editor

Restricciones
~~~~~~~~~~~~~

Ejemplos
~~~~~~~~
Observatorio Colombiano de Ciencia y Tecnología (OCyT).

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

Atributos de Campo
------------------
funderIdentifier type 

Especificadores de Campo
------------------------

Niveles de Aplicación - Productos de Colciencias
------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Observaciones del Campo
-----------------------

Adaptado de
~~~~~~~~~~~

Relaciones con otros modelos de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Niveles Semánticos
~~~~~~~~~~~~~~~~~~

Recomendación de Campos de aplicación en DSPACE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LAREFERENCIA, OPENAIRE2, OPENAIRE3)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

- **OpenAIRE 3:** dc:relation

Otras Observaciones
~~~~~~~~~~~~~~~~~~~



.. _Crossref Funder Registry: http://fundref.org/services/funder-registry
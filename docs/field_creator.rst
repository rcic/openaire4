.. _dci:creator:

Creador (M)
===========

``datacite:creator``

Nombre del campo
----------------

Campo normalizado:
~~~~~~~~~~~~~~~~~~
creator

Campo con esquema de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
datacite:creator

Traducción al español:
~~~~~~~~~~~~~~~~~~~~~~
creador

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de Ocurrencia (R/NR - Cantidad Veces)
---------------------------------------------
Repetible (R)

Definición y Alcance del campo
------------------------------
Es la entrada principal, puede ser nombre de personal o corporativo/institucional.

Forma de Descripción Normalizada (RDA/RCAA2)
-----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
name type

Relaciones con otros campos
~~~~~~~~~~~~~~~~~~~~~~~~~~~
- Colaborador
- Editor

Restricciones
~~~~~~~~~~~~~
No se debe colocar nombres de colaboradores y editores.

Ejemplos
~~~~~~~~
Observatorio Colombiano de Ciencia y Tecnología (OCyT).

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

Atributos de Campo
------------------
name type

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
- OpenAire 3: dc:creator
- BDCOL: dc.creator.corporativo

Otras Observaciones
~~~~~~~~~~~~~~~~~~~

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
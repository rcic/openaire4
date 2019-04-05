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

Valores permitidos (Vocabularios Controlados)
---------------------------------------------
- name type
- contributor type

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

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------
dc.contributor

Niveles semánticos
------------------

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

- **OpenAIRE 3:** dc.contributor
- **BDCOL:** dc.contributor, dc:contributor.advisor
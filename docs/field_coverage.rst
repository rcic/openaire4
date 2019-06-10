.. _dc.coverage:

Coverage (Cobertura) (R)
========================

``dc.coverage``

Definición y alcance del campo
------------------------------
Este campo describe la cobertura **espacial ó temporal** sobre el cual trata el recurso de información. La cobertura generalmente incluirá la ubicación espacial (un nombre del lugar o coordenadas geográficas), el período temporal (una etiqueta del período, la fecha o el rango de fechas) o la jurisdicción (como una entidad administrativa nombrada). La mejor práctica recomendada es seleccionar un valor de un vocabulario controlado.  

Niveles de persitencia (M/MA/R/O)
------------------------------------
Obligatorio (MA)

Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R): 0-n veces

Esquema de metadatos
------------------------------
dc:coverage

Traducción al español
---------------------
Cobertura Espacial / Cobertura Temporal

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar el identificador del recurso:

	- Para el caso de describir ciudades y países separe con una como (,). Y siga la misma estructura para demás delimitaciones geográficas. 
		Ej: Bogotá, Colombia
		Ej: Aguachica, Cesar, Colombia 
		Ej: Aguacatico, Medio Baudó, Chocó, Colombia

	- También puede incluir subdivisiones geográficas cronológicas (años, siglos, décadas, etc.)
		Ej: Siglo XIV
		Ej: China - Siglo XX
		Ej: Tolima, Colombia - 1950-2000



Valores permitidos (Vocabularios Controlados)
---------------------------------------------
dc.coverage

Relaciones con otros campos
---------------------------

Restricciones
-------------

Ejemplos
--------

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

  	<dc.coverage>2000-2010</dc.coverage>
	<dc.coverage>Siglo XX</dc.coverage>
	<dc.coverage>Colombia</dc.coverage>



**Esquema DataCite**

.. code-block:: xml
   :linenos:

**Esquema xoai**

.. code-block:: xml
   :linenos:

**Esquema xoai**

.. code-block:: xml
   :linenos:


Atributos de Campo
------------------
Se recomienda utilizar los siguientes vocabularios controlados:

Getty tesauro geográfico: http://www.getty.edu/research/tools/vocabularies/tgn/ 
Tesauro geográfico: https://www.vocabularyserver.com/toponimos/ 

Especificadores de campo
------------------------

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear los siguientes campos en Dspace:

- dc.coverage

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

.. _dc.coverage:

Cobertura (M)
=============

``dc.coverage``

Definición y alcance del campo
------------------------------
La cobertura generalmente incluirá la ubicación espacial (un nombre del lugar o coordenadas geográficas), el período temporal (una etiqueta del período, la fecha o el rango de fechas) o la jurisdicción (como una entidad administrativa nombrada). La mejor práctica recomendada es seleccionar un valor de un vocabulario controlado. 

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R)

Campo con esquema de metadatos
------------------------------
dc:coverage

Traducción al español
---------------------
Cobertura

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar la cobertura geográfica del recurso:

- **dc:coverage:** El campo de cobertura geográfica es obligatorio. Y permitirá conocer los lugares geográficos donde se llevaron a cabo las investigaciones o el lugar de referencia dentro del recurso. Está información delimitará a cada producto o recurso de investigación y se podrán obtener con precisión la cantidad de investigaciones realizadas. 

Para el caso de colocar ciudades y países separe con una como (,). Y siga la misma estructura para demás delimitaciones geográficas. 

- Ej: Bogotá, Colombia
- Ej: Aguachica, Cesar, Colombia 
- Ej: Aguacatico, Medio Baudó, Chocó, Colombia

También puede incluir subdivisiones geográficas cronológicas (años, siglos, décadas, etc.)

- Ej: Siglo XIV
- Ej: China - Siglo XX
- Ej: Tolima, Colombia - 1950-2000


Valores permitidos (Vocabularios Controlados)
---------------------------------------------
dc.coverage

Relaciones con otros campos
---------------------------

Restricciones
-------------

Ejemplos
--------

.. code-block:: xml
   :linenos:

  	<dc.coverage>2000-2010</dc.coverage>
	<dc.coverage>Siglo XX</dc.coverage>
	<dc.coverage>Colombia</dc.coverage>

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

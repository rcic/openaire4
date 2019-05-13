.. _redcol.financingcosts:

Costos de financiación (MA)
===========================

- ``redcol.financingcosts``
- ``redcol.totalcost``

Definición y alcance del campo
------------------------------
Hace referencia al factor económico o a los recursos económicos utilización para llevar a cabo el proyecto de investigación.

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio si es aplicable (MA)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
No repetible (NR)

Campo con esquema de metadatos
------------------------------
- redcol.financingcosts
- redcol.totalcost

Traducción al español
---------------------
Costos de financiación

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar los costos de financiación:

- **redcol.financingcosts:** Fuente inmediata de financiación o auspicio financiero de un proyecto. También puede incluirse información sobre la entidad que financia o auspicia el proyecto. 

	Ej: Consejo Latinoamericano de Ciencias Sociales ($10.000.000)

- **redcol.financingcosts:** Costo total del proyecto de investigación.

	Ej: $1.000.000.000


Valores permitidos (Vocabularios Controlados)
---------------------------------------------
- redcol.financingcosts
- redcol.totalcost

Relaciones con otros campos
---------------------------
dc.publisher

Restricciones
-------------

Ejemplos
--------

.. code-block:: xml
   :linenos:

    <redcol.financingcosts>Consejo Latinoamericano de Ciencias Sociales ($10.000.000)</redcol.financingcosts>
	<redcol.totalcosts>$1.000.000.000</redcol.totalcosts>


Atributos de campo
------------------

- financingcosts
- totalcost

Especificadores de campo
------------------------
linkedcommunity

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

- redcol.financingcosts
- redcol.totalcost

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------
.. _dci:size:

Size (Tamaño) (O)
=================

``datacite:size``

Definición y alcance del campo
------------------------------
Información del tamaño del recurso.

Campo con esquema de metadatos
------------------------------
datacite:size

Traducción al español
---------------------
Tamaño

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Opcional (O)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
No repetible (NR)

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

datacite.sizes: Descripción del recurso, incluyendo su extensión y materiales acompañantes. 

- Ej: 65 páginas + 45 fotografías a color. 
- Ej: 20 diapositivas. 
- Ej: 5 GB

Valores permitidos (Vocabularios Controlados)
---------------------------------------------
datacite:size

Relaciones con otros campos
---------------------------

Restricciones
-------------

Ejemplos
--------

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

**Esquema DataCite**

.. code-block:: xml
   :linenos:

	<datacite.sizes>
          <datacite:size>15 páginas</datacite:size>
          <datacite:size>6 MB</datacite:size>
 	</datacite.sizes>


**Esquema xoai**

.. code-block:: xml
   :linenos:

**Esquema xoai**

.. code-block:: xml
   :linenos:



Atributos de campo 
------------------

Especificadores de campo
------------------------

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

- dc.description

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear los siguientes campos en Dspace:

- datacite.sizes

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

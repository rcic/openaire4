.. _dci:datePublication:

Publication Date (Fecha de publicación) (M)
===========================================

``datacite:date``

Definición y alcance del campo
-------------------------------
Fecha asociada a la creación del recurso. 

La mejor práctica es codificar el valor de la fecha con el perfil que define ISO 8601 [W3CDTF] con formato YYYY-MM-DD

Campo con esquema de metadatos
------------------------------
datacite:date

Traducción al español
---------------------
Fecha de publicación 

Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR)
------------------------------------------------
Repetible (R)

Forma de Descripción Normalizada (RDA/ RCAA2/ ISBD)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Relaciones con otros campos
---------------------------

Restricciones
-------------

Ejemplos y ayudas
-----------------

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <datacite:date dateType="Issued">2010-12-25</datacite:date>

**Esquema xaoi**

.. code-block:: xml
   :linenos:

**Esquema xaoi**

.. code-block:: xml
   :linenos:


Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear en Dspace los siguientes campos:

- datacite:date

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------
OpenAIRE 3: dc.date 
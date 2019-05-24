.. _aire:licenseCondition:

License Condition (Condición de la licencia) (R)
================================================

``oaire:licenseCondition``

Definición y alcance del campo
------------------------------
Información sobre los derechos de la licencia. Está información deberá contener los derechos de autor y de propiedad intelectual definidos por la institución, de igual forma derechos de uso y reutilización del recurso. 

Pueden utilizarse las licencias de Creative Commons. 

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Recomendado (R)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
No repetible (NR)

Campo con esquema de metadatos
------------------------------
oaire:licenseCondition

Traducción al español
---------------------
Condición de la licencia

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
---------------------------------------------
oaire:licenseCondition

Relaciones con otros campos
---------------------------

- dc.rights
- dc.rights.uri
- dc.rights.accessrights

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

**Esquema xoai**

.. code-block:: xml
   :linenos:

**Esquema xoai**

.. code-block:: xml
   :linenos:


.. code-block:: xml
   :linenos:

   <oaire:licenseCondition startDate="2019-02-01" uri="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial</oaire:licenseCondition>

Atributos de Campo
------------------
Se recomienda utilizar el atributo de fecha, es la mejor práctica recomendada para codificar según  ISO 8601 [W3CDTF]. Utilizando el formato:
YYYY-MM-DD

Especificadores de campo
------------------------

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

- dc.rights
- dc.rights.uri
- dc.rights.accessrights

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear los siguientes campos en Dspace:

- oaire:licenseCondition

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

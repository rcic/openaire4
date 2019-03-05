.. _aire:licenseCondition:

Condición de la licencia (R)
============================

``oaire:licenseCondition``

Nombre del campo
----------------

Campo normalizado:
~~~~~~~~~~~~~~~~~~
licenseCondition

Campo con esquema de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
oaire:licenseCondition

Traducción al español:
~~~~~~~~~~~~~~~~~~~~~~
Condición de la licencia

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Recomendado (R)

Niveles de Ocurrencia (R/NR - Cantidad Veces)
---------------------------------------------
No repetible (NR)

Definición y Alcance del campo
------------------------------
Información sobre los derechos de la licencia. Está información deberá contener los derechos de autor y de propiedad intelectual definidos por la institución, de igual forma derechos de uso y reutilización del recurso. 

Forma de Descripción Normalizada (RDA/RCAA2)
--------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
oaire:licenseCondition

Relaciones con otros campos
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Restricciones
~~~~~~~~~~~~~

Ejemplos
~~~~~~~~

.. code-block:: xml
   :linenos:

   <!-- example 1 -->
   <oaire:licenseCondition startDate="2019-02-01" uri="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial</oaire:licenseCondition>

Atributos de Campo
------------------
Se recomienda utilizar el atributo de fecha, es la mejor práctica recomendada para codificar según  ISO 8601 [W3CDTF]. Utilizando el formato:
YYYY-MM-DD

Especificadores de Campo
------------------------

Niveles de Aplicación - Productos de Colciencias
------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Observaciones del Campo
-----------------------
Pueden utilizarse las licencias de Creative Commons.

Adaptado de..
~~~~~~~~~~~~~

Relaciones con otros modelos de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Niveles Semánticos
~~~~~~~~~~~~~~~~~~

Recomendación de Campos de aplicación en DSPACE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LAREFERENCIA, OPENAIRE2, OPENAIRE3)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Otras Observaciones
~~~~~~~~~~~~~~~~~~~
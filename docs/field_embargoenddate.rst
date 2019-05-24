.. _dci:dateEmbargo:

Embargo Period Date (Fecha de Periodo de Embargo)  (MA)
=======================================================

``datacite:date``

Definición y alcance del campo
------------------------------
Fecha asociada a la disponibilidad del recurso de información cuando este posee algún tipo de restricción de acceso.


Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio cuando sea aplicable (MA)

Niveles de ocurrencia (R / NR)
------------------------------------------------
No repetible (NR)

Esquema de metadatos
------------------------------
datacite:date

Traducción al español
---------------------
Fecha de periodo de embargo

Forma de Descripción Normalizada (RDA / RCAA2/ ISBD)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar la fecha con su debida puntuación:

- **datacite:date-Accepted:** Fecha de aceptación. Ej: 2019-02-01
- **datacite:date-Available:** Fecha de disponibilidad. Ej: 2019-04-01

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Clase Principal Autores (creators) (M, 1-n):
++++++++++++++++++++++++++++++++++++++++++++

- **Sub-Propiedad: Autor (creator) (M, 1-n):**

Relaciones con otros campos
---------------------------

Restricciones
-------------


Ejemplos y ayudas
-----------------

Ayudas
++++++

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <datacite:dates>
     <datacite:date dateType="Accepted">2017-11-01</datacite:date>
     <datacite:date dateType="Available">2017-12-01</datacite:date>
   </datacite:dates>

**Esquema xoai**

.. code-block:: xml
   :linenos:

**Esquema xoai**

.. code-block:: xml
   :linenos:

Niveles de aplicación para  productos de investigación de Colciencias
---------------------------------------------------------------------
Revistas, artículos, documentos de trabajo.

Relaciones con otros modelos de metadatos
-----------------------------------------
dc.date

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear en Dspace los siguientes campos:

- datacite:date-Accepted
- datacite:date-Available


Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------
OpenAIRE 3: dc.date
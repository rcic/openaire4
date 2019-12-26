.. _aire:citationConferenceDate:

Citation Conference Date (Fechas de conferencia del recurso fuente) (R)
=======================================================================

``oaire:citationConferenceDate``

Definición y alcance del campo
------------------------------
Este campo hace referencia al rango de fechas de la realización del evento asociado al recurso fuente (conferencia, congreso, encuentro, etc..).  Esta propiedad se considera parte de la cita. La mejor práctica recomendada es codificar la fecha según ISO 8601 [W3CDTF], siguiendo el formato YYYY-MM-DD

Niveles de persistencia (M/MA/R/O)
----------------------------------
Recomendado (R) 

Niveles de ocurrencia (R / NR)
------------------------------
No repetible (NR): 0-1

Esquema de metadatos
--------------------
oaire:citationConferenceDate

Traducción al español
---------------------
Rango de fechas de la realización del evento asociado al recurso fuente

Forma de Descripción Normalizada (RDA/RCAA2/ISBD)
-------------------------------------------------
RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar el rango de fechas de realización del evento asociado al recurso de información fuente. 

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad Principal Ejemplar del recurso fuente (citationConferenceDate) (R, 0-1): 
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Utilice una fecha / rango de fechas de realización del evento como valor.

Relaciones con otros campos
---------------------------

El campo  rango de fechas de realización del evento asociado al recurso fuente (oaire:citationConferenceDate) complementa la información del campo Título del recurso fuente (oaire:citationTitle) donde se describe el nombre del evento.

Restricciones
-------------
No aplica

Ejemplos y ayudas
-----------------

Ayudas
++++++

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:relation>1977-07-11</dc:relation>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <oaire:citationConferenceDate>2013-09-22/2013-09-26</oaire:citationConferenceDate>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="relation">
     <element name="citationConferenceDate">
     <element name="spa">
        <field name="value">2013-09-22/2013-09-26</field>
     </element>
   </element>
   </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="relation" qualifier="citationConferenceDate" lang="spa">2013-09-22/2013-09-26</dim:field>

.. code-block:: xml
   :linenos:

   <dim:field mdschema="oaire" element="citationConferenceDate" qualifier="" lang="spa">2013-09-22/2013-09-26</dim:field>


Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica exclusivamente a todos los productos de MinCiencias que estén relacionados con un **evento/congreso** del que se tenga las **fechas** de realización del mismo. 

Relaciones con otros modelos de metadatos
-----------------------------------------
El campo fechas de realización del evento del recurso de información fuente **(oaire:citationConferenceDate)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

======================  ===================
Esquema de Metadatos    Campo Relacionado  
======================  ===================
marcxml                 field:773$d        
======================  ===================

Niveles semánticos
------------------
No aplica

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

+----------------------------------------+-----------------------+------------------------+---------------------------------------------------------------------------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores          | Nota de alcance                                                                             |
+========================================+=======================+========================+=============================================================================================+
| OpenAire                               | dc.relation           | conferencedate         | Fechas del evento. Se pueden utilizar cualquiera de los dos esquemas provistos (dc, oaire). |
+----------------------------------------+-----------------------+------------------------+---------------------------------------------------------------------------------------------+
| OpenAire                               | oaire                 | citationConferenceDate | Fechas del evento. Se pueden utilizar cualquiera de los dos esquemas provistos (dc, oaire). |
+----------------------------------------+-----------------------+------------------------+---------------------------------------------------------------------------------------------+


Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

- Se recomienda específicamente crear los nuevos atributos/especificadores de campo de **Fechas del evento** según la codificación propuesta.
.. _aire:citationConferencePlace:

Citation Conference Place (Lugar de conferencia del recurso fuente) (R)
=======================================================================

``oaire:citationConferencePlace``

Definición y alcance del campo
------------------------------
Este campo hace referencia al **lugar de de realización del evento** asociado al recurso fuente (conferencia, congreso, encuentro, etc..).  Esta propiedad se considera parte de la cita.

Niveles de persistencia (M/MA/R/O)
----------------------------------
Recomendado (R) 

Niveles de ocurrencia (R / NR)
------------------------------
No repetible (NR): 0-1


Esquema de metadatos
--------------------
oaire:citationConferencePlace

Traducción al español
---------------------
Lugar de realización del evento asociado al recurso fuente


Forma de Descripción Normalizada (RDA/RCAA2/ISBD)
-------------------------------------------------
RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar el lugar de realización del evento asociado al recurso de información fuente. Si el evento se realizó de forma virtual se debe colocar como valor  asociado “Internet”.

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad Principal Ejemplar del recurso fuente (citationConferencePlace) (R, 0-1): 
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Utilice el nombre de un lugar de realización del evento como valor.

Relaciones con otros campos
---------------------------
El campo lugar de realización del evento asociado al recurso fuente **(oaire:citationConferencePlace)** complementa la información del campo Título del recurso fuente **(oaire:citationTitle)** donde se describe el nombre del evento.

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

   <dc:relation>Cartagena, Colombia</dc:relation>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <oaire:citationConferencePlace>Berlin</oaire:citationConferencePlace>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="relation">
     <element name="citationConferencePlace">
     <element name="spa">
        <field name="value">Madrid</field>
     </element>
   </element>
   </element>


**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="relation" qualifier="citationConferencePlace" lang="spa">Bogotá, Colombia</dim:field>

.. code-block:: xml
   :linenos:

   <dim:field mdschema="oaire" element="citationConferencePlace" qualifier="" lang="spa">Villavicencio, Meta</dim:field>


Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica exclusivamente a todos los productos de MinCiencias que estén relacionados con un **evento/congreso** del que se tenga la ubicación de realización del mismo. 

Relaciones con otros modelos de metadatos
-----------------------------------------

El campo lugar del evento del recurso de información fuente **(oaire:citationConferencePlace)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

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

+----------------------------------------+-----------------------+-------------------------+-------------------------------------------------------------------------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores           | Nota de alcance                                                                           |
+========================================+=======================+=========================+===========================================================================================+
| OpenAire                               | dc.relation           | conferenceplace         | Lugar el evento. Se pueden utilizar cualquiera de los dos esquemas provistos (dc, oaire). |
+----------------------------------------+-----------------------+-------------------------+-------------------------------------------------------------------------------------------+
| OpenAire                               | oaire                 | citationConferencePlace | Lugar el evento. Se pueden utilizar cualquiera de los dos esquemas provistos (dc, oaire). |
+----------------------------------------+-----------------------+-------------------------+-------------------------------------------------------------------------------------------+



Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

	- Se recomienda específicamente crear los nuevos atributos/especificadores de campo de **Lugar del evento** según la codificación propuesta.
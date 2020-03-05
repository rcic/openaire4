.. _aire:citationVolume:

Citation Volume (Volumen del recurso fuente) (R)
================================================

``oaire:citationVolume``

Definición y alcance del campo
------------------------------
Este campo Hace referencia a la designación numérica/secuencial del volumen del recurso fuente. Esta propiedad es parte de la cita bibliográfica.

Niveles de persistencia (M/MA/R/O)
----------------------------------
Recomendado (R) 

Niveles de ocurrencia (R / NR)
------------------------------
No repetible (NR): 0-1

Esquema de metadatos
--------------------
oaire:citationVolume

Traducción al español
---------------------
Volumen del recurso fuente

Forma de Descripción Normalizada (RDA/RCAA2/ISBD)
-------------------------------------------------
RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar el volumen del recurso de información fuente (enfocado especialmente para recursos seriados).

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad Principal Volumen del recurso fuente (citationVolume) (R, 0-1): 
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Utilice el número de volumen como valor.

Relaciones con otros campos
---------------------------
El campo volumen del recurso fuente **(oaire:citationVolume)** complementa la información del campo Título del recurso fuente **(oaire:citationTitle)** para tipologías documentales seriadas que utilicen volúmen (principalmente - Artículos de revista)

Restricciones
-------------
No aplica


Ejemplos y ayudas
-----------------

Ayudas
++++++

- **Ejemplo de un artículo de una revista:**
	- <citationTitle>Chemistry</citationTitle>
	- <citationVolume>23</citationVolume>
	- <citationIssue>31</citationIssue>
	- <citationStartPage>7444</citationStartPage>
	- <citationEndPage>7447</citationEndPage>
    - <citationEdition>Enero - Junio 2018</citationEdition>

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:relation>11</dc:relation>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <oaire:citationVolume>10</oaire:citationVolume>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="relation">
     <element name="citationvolume">
     <element name="spa">
        <field name="value">34</field>
     </element>
   </element>
   </element>


**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="relation" qualifier="citationvolume" lang="spa">45</dim:field>

.. code-block:: xml
   :linenos:

   <dim:field mdschema="oaire" element="citationvolume" qualifier="" lang="spa">45</dim:field>


Niveles de aplicación para  productos de investigación de MinCiencias
---------------------------------------------------------------------
Se aplica exclusivamente a todos los productos seriados de MinCiencias que utilicen volumen de publicación.

Relaciones con otros modelos de metadatos
-----------------------------------------

El campo volumen de recurso de información fuente **(oaire:citationVolume)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

======================  ======================
Esquema de Metadatos    Campo Relacionado     
======================  ======================
marcxml                 field:773$g           
dc                      dc.relation.ispartof  
dcterms                 dcterms.ispartof      
======================  ======================


Niveles semánticos
------------------
No aplica


Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

+----------------------------------------+-----------------------+----------------+--------------------------------------------------------------------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores  | Nota de alcance                                                                      |
+========================================+=======================+================+======================================================================================+
| OpenAire                               | dc.relation           | citationvolume | Volumen de publicación. Se pueden utilizar cualquiera de los dos esquemas provistos. |
|                                        |                       |                | * Equivalencia Semántica: oaire.citationvolume / dc.relation.citationvolume          |
+----------------------------------------+-----------------------+----------------+--------------------------------------------------------------------------------------+



Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

	- Se recomienda específicamente crear los nuevos atributos/especificadores de campo de volumen según la codificación propuesta.

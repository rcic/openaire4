.. _aire:citationIssue:

Citation Issue (Ejemplar/Número del recurso fuente) (R)
=======================================================

``oaire:citationIssue``

Definición y alcance del campo
------------------------------
Este campo hace referencia a la designación numérica/secuencial del ejemplar (número tomo, parte o capítulo) del recurso fuente. Esta propiedad es parte de la cita bibliográfica.

Niveles de persistencia (M/MA/R/O)
----------------------------------
Recomendado (R) 

Niveles de ocurrencia (R / NR)
------------------------------
No repetible (NR): 0-1

Esquema de metadatos
--------------------
oaire:citationIssue

Traducción al español
---------------------
Ejemplar  del recurso fuente

Forma de Descripción Normalizada (RDA/RCAA2/ISBD)
-------------------------------------------------
RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar el ejemplar del recurso de información fuente (enfocado especialmente para recursos seriados).


Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad Principal Ejemplar del recurso fuente (citationIssue) (R, 0-1): 
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Utilice el número de ejemplar como valor.

Relaciones con otros campos
---------------------------
El campo ejemplar del recurso fuente **(oaire:citationIssue)** complementa la información del campo Título del recurso fuente **(oaire:citationTitle)** para tipologías documentales seriadas que utilicen este valor (principalmente - Artículos de revista)

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

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:relation>1</dc:relation>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <oaire:citationIssue>1</oaire:citationIssue>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="relation">
     <element name="citationissue">
     <element name="spa">
        <field name="value">4</field>
     </element>
   </element>
   </element>


**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="relation" qualifier="citationissue" lang="spa">5</dim:field>

.. code-block:: xml
   :linenos:

   <dim:field mdschema="oaire" element="citationissue" qualifier="" lang="spa">5</dim:field>


Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica exclusivamente a todos los productos seriados de MinCiencias que utilicen ejemplar de publicación. 

Relaciones con otros modelos de metadatos
-----------------------------------------
El campo ejemplar del recurso de información fuente **(oaire:citationIssue)**   es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

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

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

+----------------------------------------+-----------------------+---------------+---------------------------------------------------------------------------------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores | Nota de alcance                                                                                   |
+========================================+=======================+===============+===================================================================================================+
| OpenAire                               | dc.relation           | citationissue | Ejemplar de publicación. Se pueden utilizar cualquiera de los dos esquemas provistos (dc, oaire). |
+----------------------------------------+-----------------------+---------------+---------------------------------------------------------------------------------------------------+



Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

	- Se recomienda específicamente crear los nuevos atributos/especificadores de campo de **ejemplar** según la codificación propuesta.

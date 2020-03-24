.. _aire:citationTitle:

Citation Title (Título del recurso fuente) (R)
==============================================

``oaire:citationTitle``

Definición y alcance del campo
------------------------------
Cuando se está  haciendo una catalogación analítica, este campo **(oaire:citationTitle)** hace referencia al título de donde es publicado el recurso de información (revista, libro, conferencia, etc.), esta propiedad es parte de la cita bibliográfica.

La catalogación analítica consiste en la descripción y análisis de un recurso de información visto como una parte contenida en otra parte denominada documento fuente. Por tanto, el registro bibliográfico del recurso de información fuente de llama registro fuente (otros lo llaman registro padre) y los registros de las partes, cuando se catalogan de forma independiente, se llaman registros analíticos

El  recurso de información fuente **(oaire:citationTitle)** puede ser una monografía (texto o audiovisual) o una publicación periódica (revista, serie monográfica). por tanto los recursos de información analíticos pueden ser de carácter monográfico ó seriado. 

	- En el caso de que sea una monografía los registros analíticos describirían  los capítulos de un libro (suele hacerse con las obras escritas en colaboración) o las ponencias de un Congreso, encuentro  o evento (Nombre de reunión, congreso o de jurisdicción).
	- En el caso de publicaciones periódicas, lo que se cataloga individualizadamente son los artículos de cada número.

**Notas:** 

	- No es necesario catalogar de forma analítica todas y cada una de las partes componentes, sino que se puede hacer una selección de las mismas dentro de cada recurso de información fuente.
	- En los registros analíticos es necesario hacer referencia al recurso de información fuente **(oaire:citationTitle).** En cambio en el registro fuente no es tan importante esa relación, aunque se considera conveniente informar de ello en una nota (dc.description.note).


Niveles de persistencia (M/MA/R/O)
----------------------------------
Recomendado (R) 


Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R) 0-1 veces


Esquema de metadatos
--------------------
oaire:citationTitle


Traducción al español
---------------------
Título de recurso de información fuente (documento anfitrión)

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar el título del recurso de información fuente.


Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad Principal Título del recurso fuente (citationTitle) (R, 0-1): 
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Utilice el nombre del título como valor.

Relaciones con otros campos
---------------------------

	- No se debe confundir el campo título de recurso de información fuente **(oaire:citationTitle)** con el campo colaborador **(dc.contributor.conferencename)** cuando es utilizado como entrada principal del recurso.
	- No se debe confundir el campo título de recurso de información fuente **(oaire:citationTitle)** con el campo título de serie **(dc.relation.ispartofseries/datacite:relatedIdentifier.isParOfSeries)**

Restricciones
-------------

No Aplica

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

	- **Ej: (Título de una Revista) (dc.relation.ispartofjournal):**	Clinical Biomechanics
	- **Ej: (Título de una Libro ) (dc.relation.ispartofbook): Colombia:** manual comercial e industrial
	- **Ej: (Título de un Evento/Congreso) (dc.relation.ispartofconference):** VI Encuentro Científico Continental

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:relation>Colombia : manual comercial e industrial</dc:relation>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <oaire:citationTitle>Revista Nómadas</oaire:citationTitle>

.. code-block:: xml
   :linenos:

   <oaire:citationTitle>Colombia : manual comercial e industrial<//oaire:citationTitle>


**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="relation">
     <element name="ispartofjournal">
     <element name="spa">
        <field name="value">Revista EIA</field>
     </element>
   	</element>
   </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="relation" qualifier="ispartofbook" lang="spa">Colombia : manual comercial e industrial</dim:field>

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="relation" qualifier="ispartofjournal" lang="spa">Revista apuntes del CENES</dim:field>

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="relation" qualifier="ispartofconference" lang="spa">XII Encuentro de catalogadores OpenAire</dim:field>

Niveles de aplicación para  productos de investigación de MinCiencias
---------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias. 
 

Relaciones con otros modelos de metadatos
-----------------------------------------
El campo título de recurso de información fuente **(oaire:citationTitle)**   es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

======================  ======================
Esquema de Metadatos    Campo Relacionado     
======================  ======================
marcxml                 field:773$t           
dc                      dc.relation.ispartof  
dcterms                 dcterms.ispartof      
======================  ======================


Niveles semánticos
------------------

No aplica

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

+----------------------------------------+-----------------------+--------------------+---------------------------------------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores      | Nota de alcance                                         |
+========================================+=======================+====================+=========================================================+
| OpenAire                               | dc.relation           | ispartofjournal    | Título de revista como documento anfitrión              |
|                                        |                       |                    |                                                         |
|                                        |                       |                    | -Para Título abreviado ver nota asociada.               |
+----------------------------------------+-----------------------+--------------------+---------------------------------------------------------+
| OpenAire                               | dc.relation           | ispartofbook       | Título de libro como documento anfitrión                |
+----------------------------------------+-----------------------+--------------------+---------------------------------------------------------+
| OpenAire                               | dc.relation           | ispartofconference | Nombre de Conferencia / Evento como documento anfitrión |
+----------------------------------------+-----------------------+--------------------+---------------------------------------------------------+

Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

	- Se recomienda específicamente crear los nuevos atributos/especificadores de campo de **título del recurso fuente** según la codificación propuesta.
	- Se presenta equivalencia semántica de los campos sugeridos para usar en Dspace (**dc.relation.ispartofjournal, dc.relation.ispartofbook, dc.relation.ispartofconference**) con el **campo oaire.citationtitle.**
	- Para registrar el título abreviado del documento anfitrión, se recomienda utilizar el campo **dc.relation.ispartofjournalabbrev**
	
	

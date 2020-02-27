.. _dci:title:

.. _dci:title_title:

Title (Título) (M)
==================

``datacite:title``

Definición y alcance del campo
------------------------------
Texto libre que contiene el nombre(s) del recurso o variantes del mismo con el que es conocido/utilizado. Este campo puede utilizarse para generar puntos de acceso con despliegue a los diversos títulos existentes. Se debe transcribir el título del recurso original, en orden y ortografía presente. Los subtítulos deben separarse del título mediante dos puntos, precedidos y seguidos por un espacio.

Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R): **1-n veces**.

..

Repita este campo utilizando las distintas propiedades/tipo de título con su correspondientes atributos de idioma según se considere.


Esquema de metadatos
------------------------------
datacite:title

..

**Nota:** Este campo se ha adaptado del esquema de metadatos DATACITE MetadataKernel versión 4.1 (http://doi.org/10.5438/0014), el cual es utilizado ampliamente para la gestión de documentos y datos. 

Traducción al español
---------------------
Título (Título propiamente dicho)

Forma de Descripción Normalizada (RDA / RCAA2 / ISBD)
-----------------------------------------------------
RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar la información de título con su debida puntuación:

	- **Título:** Ingrese el título del recurso, la primera letra en mayúscula y finalice con punto. Ej: Acuerdos de paz en Colombia.
	- **Subtítulo:** Seguido del título principal del recurso colocar "espacio : espacio" e ingrese el subtítulo. Ejemplo: Acuerdos de paz en Colombia : una mirada al conflicto armado 
	
Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad Título (title) (M, 1-n): Utilice el nombre del título como valor
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

	- **Atributo IDIOMA (xml:lang) (O, 0-1):** Este atributo especifica el idioma asociado al tipo de título que se describe. Se debe tener en cuenta su codificación normalizada según el vocabulario propuesto por el estándar ISO 639-3 utilizando carácteres en UTF-8 (https://iso639-3.sil.org/code_tables/download_tables)

	- **Atributo Tipo de Título (titleType) (O, 0-1):** Este atributo permite especificar el tipo de título que se describe en el campo de metadatos. Se debe tener en cuenta los siguientes tipos de título y su codificación normalizada según el vocabulario controlado propuesto: 

+-------------------------+--------------------------------------------------------------------+------------------------+
| Vocabulario Normalizado | Descripción del Atributo                                           | Dominio de Vocabulario |
+=========================+====================================================================+========================+
| AlternativeTitle        | Título Alternativo / Variantes del Título                          | datacite [#]_          |
+-------------------------+--------------------------------------------------------------------+------------------------+
| Subtitle                | Subtítulo (Recomendado unificar en Título: Subtítulo)              | datacite               |
+-------------------------+--------------------------------------------------------------------+------------------------+
| TranslatedTitle         | Título Traducido                                                   | datacite               |
+-------------------------+--------------------------------------------------------------------+------------------------+
| AbbreviatedTitle        | Título Abreviado                                                   | redcol                 |
+-------------------------+--------------------------------------------------------------------+------------------------+
| FormerTitle             | Título Anterior                                                    | redcol                 |
+-------------------------+--------------------------------------------------------------------+------------------------+
| Other                   | Otros Títulos                                                      | datacite               |
+-------------------------+--------------------------------------------------------------------+------------------------+


Relaciones con otros campos
---------------------------

  - El título de una colección o serie se debe ingresar en el campo dc.relation.ispartofseries
  - El título anterior de un recurso de información se debe ingresar en el campo dc.relation.isversionof
  - Para describir el título del documento anfitrión (Aplica para documentos analíticos), es recomendado utilizar oaire:citationTitle       (https://redcol.readthedocs.io/es/latest/field_citationtitle.html).

Restricciones
-------------
No Aplica

Ejemplos y ayudas
-----------------

**Ayudas**

- **Título:** Coloque el título del recurso tal como aparece en la obra. Ej: Acuerdos Paz en Colombia
- **Título alternativo:** Coloque el título alternativo del recurso si lo tiene. Ej: Paz en Colombia. 
- **Título traducido:** Coloque la traducción del título del recurso. Ej: Peace agreements in Colombia.
- **Variante del título:** Es la forma de un título que aparece en diferentes partes del recurso y es diferente al título registrado en el campo datacite:title. Ej: Colombia y sus acuerdos de paz. 
- **Otro título:** Ingrese un título adicional del recurso si aparece referenciado en el recurso. Ejemplo: Políticas de los acuerdos de paz en Colombia. 

**Ejemplo en XML  (Interoperabilidad OAI-PMH)**

- Esquema oai_dc

.. code-block:: xml
   :linenos:

    <dc:title>La construcción de la historia subjetiva en la clínica psicológica</dc:title>
	<dc:title>The construction of subjective history in the clinical practice of psychology</dc:title>
	<dc:title>Construção da história subjetiva na clínica psicológica</dc:title>

- Esquema DataCite

.. code-block:: xml
   :linenos:

   <datacite:title xml:lang="en-US">
 	Estudio para identificar conocimientos, capacidades, percepciones y experiencias de los investigadores del país frente a la ciencia abierta
	</datacite:title>
	<datacite:title xml:lang="en-US" titleType="Subtitle">A survey</datacite:title>

- Esquema xoai

.. code-block:: xml
   :linenos:

   <element name="title">
     <element name="spa">
          <field name="value">La construcción de la historia subjetiva en la clínica psicológica</field>
     </element>
     <element name="translated">
       <element name="eng">
         <field name="value">The construction of subjective history in the clinical practice of psychology</field>
        <field name="por">Construção da história subjetiva na clínica psicológica</field>
      </element>
    </element>
	</element>

- Esquema dim

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="title" lang="spa">La construcción de la historia subjetiva en la clínica psicológica</dim:field>
   <dim:field mdschema="dc" element="title" qualifier="translated" lang="eng">The construction of subjective history in the clinical practice of psychology</dim:field>
   <dim:field mdschema="dc" element="title" qualifier="translated" lang="por">Construção da história subjetiva na clínica psicológica</dim:field> 
   
   <dim:field mdschema="dc" element="title" lang="spa">El cantar del Mio Cid</dim:field>
   <dim:field mdschema="dc" element="title" qualifier="alternative" lang="spa">El Cid campeador</dim:field>
   <dim:field mdschema="dc" element="title" qualifier="alternative" lang="spa">Poema de Mio Cid</dim:field>
   <dim:field mdschema="dc" element="title" qualifier="alternative" lang="spa">El cantar de los cantares</dim:field>


..


Niveles de aplicación para  productos de investigación de MinCiencias
---------------------------------------------------------------------
Se aplica a todos los productos de investigación reconocidos por MinCiencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------
El campo **Título** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+-------------------+
| Esquema de Metadatos | Campo Relacionado |
+======================+===================+
| dc                   | dc.title          |
+----------------------+-------------------+
| dcterms              | dcterms.title     |
+----------------------+-------------------+
| lom                  | lom.title         |
+----------------------+-------------------+
| marcxml              | field:245         |
+----------------------+-------------------+

Niveles semánticos
------------------
No Aplica

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

.. tabularcolumns:: |\Y{0.3}|\Y{0.2}|\Y{0.2}|\Y{0.3}|

+----------------------------------------+-----------------------+-------------+--------------------------------------------------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Cualificar  | Nota de alcance                                                    |
+========================================+=======================+=============+====================================================================+
| Title                                  | dc.title              |             | Título propiamente dicho                                           |
+----------------------------------------+-----------------------+-------------+--------------------------------------------------------------------+
| AlternativeTitle                       | dc.title              | alternative | Título Alternativo / Variantes del Título                          |
+----------------------------------------+-----------------------+-------------+--------------------------------------------------------------------+
| Subtitle                               | dc.title              |             | Integrado en el campo Título (Separar con el signo ":")            |
+----------------------------------------+-----------------------+-------------+--------------------------------------------------------------------+
| TranslatedTitle                        | dc.title              | translated  | Título Traducido                                                   |
+----------------------------------------+-----------------------+-------------+--------------------------------------------------------------------+
| AbbreviatedTitle                       | dc.title              | abbreviated | Título Abreviado                                                   |
+----------------------------------------+-----------------------+-------------+--------------------------------------------------------------------+
| FormerTitle                            | dc.title              | former      | Título Anterior                                                    |
+----------------------------------------+-----------------------+-------------+--------------------------------------------------------------------+
| Other                                  | dc.title              | other       | Otros Títulos                                                      |
+----------------------------------------+-----------------------+-------------+--------------------------------------------------------------------+


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

- En las distintas directrices que han existido, siempre ha sido obligatorio el uso del campo título.
- En el sistema DSPACE en su instalación por defecto viene con los campo **dc.title** y **dc.title.alternative.** 
- Se recomienda específicamente crear los nuevos atributos/especificadores de campo de título según la codificación propuesta.


.. [#] http://schema.datacite.org/meta/kernel-4.0/include/datacite-titleType-v4.xsd

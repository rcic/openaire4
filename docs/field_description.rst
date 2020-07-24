.. _dc.description:

Description (Descripción) (MA)
==============================

``dc:description``

Definición y alcance del campo
------------------------------
Información general o específica del recurso utilizada para la descripción textual. En la descripción se puede incluir resumen, tabla de contenido, representación gráfica del contenido o un texto libre que describa el contenido del recurso. Cuando un recurso consta de varios recursos,anexos u objetos separados no utilice este campo para enumerar las URL de los archivos.   

Niveles de persistencia (M/MA/R/O)
----------------------------------
Obligatorio si es aplicable (MA)

Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R): **0-n veces**

..

Repita este campo utilizando el atributo para indicar el idioma de la descripción.

Esquema de metadatos
---------------------
dc.description 

Traducción al español
---------------------
Descripción del recurso(Resumen, tabla de contenido) 

Forma de Descripción Normalizada (RDA/RCAA2/ISBD)
-------------------------------------------------
RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar la información la descripción con su debida puntuación:

  - **Descripción (dc.description):** Descripción general del recurso.
  - **Resumen (dc.description.abstract):** Describe el alcance de los contenidos, puede ser un sumario, un resumen, una reseña, una anotación o una frase que describe el recurso. Si la información es tomada textualmente del recurso, se coloca al final del resumen: (Apartes del texto). 
  - **Notas (dc.description.notes):** Coloque notas generales de interés al público relacionadas con el recurso. 
  - **Comentarios (dc.description.comments):** Coloque los comentarios generados sobre el recurso omitiendo datos de la entidad que lo generó y fechas de generación. 
  - **Tabla de Contenidos (dc.description.tableofcontents):** Coloque el índice del recurso de información omitiendo  números de página y caracteres sin valor semántico (puntos, guiones tabuladores, espacios, etc..)


Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad de Descripción (Description) (MA, 1-n):
+++++++++++++++++++++++++++++++++++++++++++++++++

Use la descripción textual como un valor.

    - **Atributo IDIOMA (xml:lang) (O, 0-1):** Este atributo especifica el idioma utilizado en la descripción. Se debe tener en cuenta su codificación normalizada según el vocabulario propuesto por el estándar ISO 639-3 utilizando carácteres en UTF-8 (https://iso639-3.sil.org/code_tables/download_tables)
      
    - **Atributo Tipo de Descripción (descriptionType) (O, 0-1):** Este atributo permite especificar el tipo de descripción asociada al recurso. Se debe tener en cuenta los siguientes tipos de descripción y su codificación normalizada según el vocabulario controlado propuesto: 

+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| Vocabulario Normalizado   | Descripción del Atributo                                                                                                                  | Dominio de Vocabulario |
+===========================+===========================================================================================================================================+========================+
| abstract                  | Una breve descripción del recurso y el contexto en el que se creó el recurso.                                                             | datacite               |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| comments                  | Comentarios y observaciones hechos al recurso                                                                                             | redcol                 |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| methods                   | La metodología empleada para el estudio o investigación.                                                                                  | datacite               |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| notes                     | Notas asociadas al recurso                                                                                                                | redcol                 |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| tableofcontents           | Una lista de la tabla de contenidos.                                                                                                      | datacite               |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| technicalinfo             | Información detallada que puede estar asociada con el diseño, implementación, operación, uso y / o mantenimiento de un proceso o sistema. | datacite               |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| provenance                | Describir la historia de la custodia del recurso desde su creación, incluyendo los cambios que se le hicieron.                            | redcol                 |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| seriesinformation         | Información sobre una serie que se repite, como volumen, número, número.                                                                  | datacite               |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| sponsorship               | Información sobre agencias patrocinadoras                                                                                                 | datacite               |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| funder                    | Indicaciones del patrocinio y datos específicos de financiación.                                                                          | datacite               |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| statementofresponsibility | Declaración de responsabilidad sobre el recurso                                                                                           | redcol                 |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
| other                     | Otro tipo de descripción                                                                                                                  | datacite               |
+---------------------------+-------------------------------------------------------------------------------------------------------------------------------------------+------------------------+


Relaciones con otros campos
---------------------------

  - No confundir el campo descripción del recurso (dc.description) en todas sus facetas con el campo licencia del recurso (dc.rights).
  - No confundir el campo  que amplía la información sobre las agencias patrocinadoras (dc.description.sponsorship) con el campo de referencia de financiación (oaire: fundingReference) del recurso.
  - No confundir el campo  que ofrece indicaciones del patrocinio y datos específicos de financiación (dc.description.funder) con el campo de referencia de financiación (oaire: fundingReference) del recurso

Restricciones
-------------

No aplica

Ejemplos y ayudas
-----------------

Ayudas
++++++

  - **Ej: Resumen (Español):** Aislamiento y purificación de compuestos; Actividad antileishmanial a partir de Cordia dentada Poir; Heliotropium indicum; etc. 
  - **Ej: Notas:** dc.description.notes: Convenio Interadministrativo No. 271 de 2015.
  - **Ej: Mención de responsabilidad:** dc.description.statementofresponsibility  by Heather M. Phipps.

Ejemplo en XML  (Interoperabilidad OAI-PMH)
+++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc.description xml:lang="es-spa">
   Aislamiento y purificación de compuestos; Actividad antileishmanial a partir de Cordia dentada Poir; Heliotropium indicum; etc. 
   </dc.description abstract>

.. code-block:: xml
   :linenos:

   <dc.description>
   Convenio Interadministrativo No. 271 de 2015. 
   </dc.description>


**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <dc:description>
   Foreword [by] Hazel Anderson; Introduction; The scientific heresy: transformation of a society; Consciousness as causal reality [etc]
   </dc:description>

.. code-block:: xml
   :linenos:

   <dc:description xml:lang="en-US">
    A number of problems in quantum state and system identification are addressed.
   </dc:description>


**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="description">
    <element name="spa">
      <field name="value">Artículo de investigación</field>
    </element>
    <element name="abstract">
      <element name="spa">
        <fieldname="value">El artículo revisa la normatividad y jurisprudencia relacionada con la evolución y alcance del derecho prestacional</field>
      </element>
    </element>
    <element name="provenance">
      <element name="en">
        <field name="value">Submitted by Autoarchivo Repositorio UCaC (riucac@ucatolica.edu.co) on 2017-10-09T22:16:46Z</field>
     </element>
    </element>
    <element name="notes">
      <element name="spa">
        <field name="value">30 p.</field>
      </element>
    </element>
    <element name="tableofcontents">
      <element name="spa">
        <field name="value">Introducción. 
          1. Caracterización del sistema pensional colombiano. 
          2. Régimen solidario pensional. 
          3. Acceso solidario a una pensión de personas en situación de discapacidad en la jurisprudencia de la Corte Constitucional. 
          4. Acceso solidario a una pensión de las madres comunitarias en la jurisprudencia de la Corte Constitucional. 
          Conclusiones. 
          Referencias. 
          Normatividad. 
          Jurisprudencia.</field>
      </element>
    </element>
   </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="description" lang="en_US">Includes bibliographical references (leaves 24-27).</dim:field>
   <dim:field mdschema="dc" element="description" qualifier="abstract" lang="en_US">Durante la Guerra Civil Espafiola y los años de Franco, habia poco lugar para los pintores y los autores de obras literarias, especialmente aquellos de inclinación liberal. </dim:field>
   <dim:field mdschema="dc" element="description" qualifier="statementofresponsibility" lang="en_US">by Heather M. Phipps.</dim:field>
   <dim:field mdschema="dc" element="description" qualifier="notes" lang="en_US">S.B.in Humanities and Engineering</dim:field>


Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

El campo de descripción es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+---------------------+
| Esquema de Metadatos | Campo Relacionado   |
+======================+=====================+
| dc                   | dc.description      |
+----------------------+---------------------+
| dcterms              | dcterms.description |
+----------------------+---------------------+
| marcxml              | Campos :3XX y 5XX   |
+----------------------+---------------------+

Niveles semánticos
------------------

No aplica.

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Vocabulario controlado OpenAire/RedCol                          | Campo Elemento DSPACE | Calificadores             | Nota de alcance |
+=================================================================+=======================+===========================+=================+
| Descripción general                                             | dc.description        |                           |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Resumen                                                         | dc.description        | abstract                  |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Comentarios                                                     | dc.description        | comments                  |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Metodología de investigación                                    | dc.description        | methods                   |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Notas                                                           | dc.description        | notes                     |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Tabla de contenido                                              | dc.description        | tableofcontents           |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Información técnica                                             | dc.description        | technicalinfo             |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Procedencia                                                     | dc.description        | provenance                |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Usos recomendados                                               | dc.description        | recommendeduse            |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Información de Series                                           | dc.description        | seriesinformation         |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Declaración de responsabilidad                                  | dc.description        | statementofresponsibility |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Agencias patrocinadoras                                         | dc.description        | sponsorship               |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Indicaciones del patrocinio y datos específicos de financiación | dc.description        | funder                    |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Escala (Serie de elementos de la misma especie, ordenados       | dc.description        | scale                     |                 |
| en función de alguna de sus características o cualidades)       |                       |                           |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+
| Otros                                                           | dc.description        | other                     |                 |
+-----------------------------------------------------------------+-----------------------+---------------------------+-----------------+


Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

Se recomienda específicamente crear los nuevos atributos/especificadores del campo de descripción según la codificación propuesta.



.. _dci:subject:

Subject (Materia) (MA)
======================

``datacite:subject``

Definición y alcance del campo
------------------------------
Asunto, palabra clave, tema o frase que describe al recurso. Es un punto de acceso que tiene el recurso para ser consultado por el usuario. Puede elegir palabras más significativas evitando que sea demasiado general sino más específica. 

Se recomienda el uso de términos controlados localizados en tesauros o listas de encabezamientos de materias. En caso de que no estén controladas utilice el calificador de campo especial para registrar esta información.
 


Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio si es aplicable (MA)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R): **0-n veces**

..

**Notas:** Repita este campo utilizando los distintos atributos del elemento según se considere

Esquema de metadatos
------------------------------
datacite:subject

**Nota:** Este campo se ha adaptado del esquema de metadatos DATACITE MetadataKernel versión 4.2 (http://doi.org/10.5438/0014), el cual es utilizado ampliamente para la gestión de documentos y datos. 

Traducción al español
---------------------
Palabras clave / Materia / Punto de acceso, descriptores y/o códigos de clasificación.

Forma de Descripción Normalizada (RDA/RCAA2/ISBD)
-------------------------------------------------
**RDA (Recursos: descripción y acceso):** Revise la forma adecuada para ingresar la información de descriptor con su debida puntuación.

Donde los términos se toman de un esquema de clasificación estándar: codifique cada término usando los atributos adicionales de la propiedad del sujeto. Codifique el descriptor de materia completo de acuerdo con el esquema relevante. Utilice el uso de mayúsculas y puntuación tal cual como aparece en el esquema original.

Se recomienda usar un URI cuando se usan esquemas de clasificación o vocabularios controlados semánticamente por una ontología ó bajo un esquema de datos enlazados (LOD), esto es útil para la identificación normalizada del descriptor por parte de los sistemas agregadores y/o proveedores de servicios.

Para las palabras clave o términos del lenguaje natural (no controladas por un vocabulario o tesauro) y /o descriptores (términos controlados por un vocabulario o tesauro), repetir el elemento tantas veces como sea necesario. Poner primero los términos en el idioma original y luego en el/los idioma/s en se encuentren disponibles. 

Para agregar una subdivisión general o subdivisión de forma (si aplica) que permita complementar el punto de acceso para una efectiva recuperación, utilice guión separado por espacios (-). Ejemplo:

- **Materia (Lemb):** Lista de encabezamientos de materia para bibliotecas. Ej: Feminismo - Historia - Videos


Propiedades, atributos y especificadores de campo
-------------------------------------------------

Clase Materias (subjects) (MA, 0-n):
++++++++++++++++++++++++++++++++++++

Entidad que agrupa todos los descriptores del recurso.

    - Propiedad Materia (subject) (MA, 0-n): Utilice la materia o palabra clave como valor.

        - Atributo Nombre del lenguaje documental (subjectScheme) (O, 0-1): Nombre del esquema de materia o código de clasificación o autoridad. Se deben tener en cuenta el siguiente o vocabulario controlado propuesto:

+-------------------------+------------------------------------------------------------------------------+------------------------+
| Vocabulario Normalizado | Descripción del Atributo                                                     | Dominio de Vocabulario |
+=========================+==============================================================================+========================+
| armarc                  | Archivo en línea de autoridades de materia                                   | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| udc                     | Clasificación Decimal Universal                                              | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| ddc                     | Clasificación Decimal Dewey                                                  | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| lcc                     | Clasificación de la Biblioteca del Congreso de EE.UU                         | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| lcsh                    | Listado de encabezamiento de materias de la Biblioteca del Congreso de EE.UU | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| lem                     | Lista de encabezamientos de materia de la Biblioteca Nacional de España      | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| lemb                    | Lista de encabezamientos de materia para biblioteca Luis Ángel Arango        | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| ecm                     | Catálogo de unión de autoridades de materia de México DGB/UNAM               | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| mesh                    | Lista de términos en temas médicos                                           | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| agrovoc                 | Vocabulario controlado de agricultura                                        | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| decs                    | Descriptores en ciencia de la salud                                          | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| unesco                  | Tesauro multidisciplinario                                                   | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| tee                     | Tesauro europeo de educación                                                 | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| ocde                    | Lista de términos en desarrollo económico y social                           | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| jel                     | Códigos de clasificación en economía                                         | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| proposal                | Descriptores Propuestos No normalizados                                      | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| classification          | Esquema de clasificación local                                               | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| spines                  | Tesauro Spines                                                               | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+
| other                   | Otros Vocabularios                                                           | datacite               |
+-------------------------+------------------------------------------------------------------------------+------------------------+

        - **Atributo URI (schemeURI) (O, 0-1):** URI del esquema identificador del vocabulario controlado cuando este lo posee. En este campo se puede colocar la URL de acceso al vocabulario controlado en Internet. Ejemplos:
            - Sistema de Clasificación Dewey (ddc): http://dewey.info/
            - Agrovoc (agrovoc):  http://aims.fao.org/aos/agrovoc 
            - Listado de encabezamiento de materias de la Biblioteca Luis Ángel Arango - Colombia (lemb): http://search.lembdigital.com/lemb 
            - Listado de encabezamiento de materias de la Biblioteca del Congreso de EE.UU (lcsh): http://id.loc.gov/authorities/subjects 
            - DGB/UNAM: http://librunam.dgbiblio.unam.mx:8991/F/?func=find-b-0&local_base=ecm12 

..

        - **Atributo URI (valueURI) (O, 0-1):** Este atributo permite almacenar la URI del descriptor utilizado **en el caso que esté disponible y se encuentre construido con una  ontología ó utilizando enlaces de Linked Open Data (LOD).** Ejemplos:
            - Descriptor (Water - Concept):  http://id.loc.gov/authorities/subjects/sh85145447 
            - Clasificación UDC (60  Biotechnology - 601 Fundamental concepts) :  http://udcdata.info/037278 

Relaciones con otros campos
---------------------------

- No confundir con Condición de la licencia (R).

Restricciones
-------------

No aplica


Ejemplos y ayudas
-----------------

Ayudas 
++++++

  - **Materia:** Punto de acceso, palabra clave de la temática del recurso. Ej: Matemáticas financieras.
  - **Materia (DDC):** Clasificación Decimal Dewey según la temática del recurso. Ej: 519 - Probabilidad y estadística.
  - **Materia (Armarc):** Archivo en línea de autoridades de materia según la temática del recurso. Ej: Economía política. 

Ejemplo en XML  (Interoperabilidad OAI-PMH)
-------------------------------------------

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:subject>Tributos locales</dc:subject>
   <dc:subject>Impuesto sobre el Incremento de Valor de los Terrenos de Naturaleza Urbana</dc:subject>
   <dc:subject>Tribunal Constitucional</dc:subject>
   <dc:subject>Capacidad Económica</dc:subject>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <datacite:subjects>
    <datacite:subject>Arenes</datacite:subject>
    <datacite:subject>Carbene</datacite:subject>
    <datacite:subject>C-H activation</datacite:subject>
    <datacite:subject>Iron</datacite:subject>
    <datacite:subject>Manganese</datacite:subject>
   </datacite:subjects>

.. code-block:: xml
   :linenos:

   <datacite:subjects>
    <datacite:subject>Geología</datacite:subject>
    <datacite:subject subjectScheme="DDC" schemeURI="http://dewey.info/" valueURI="">551 Geología, hidrología</datacite:subject>
   </datacite:subjects>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="subject">
   <element name="other">
       <element name="es_ES">
           <field name="value">Arenes</field>
           <field name="value">Carbene</field>
           <field name="value">C-H activation</field>
           <field name="value">Iron</field>
           <field name="value">Manganese</field>
       </element>
   </element>
   </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="subject" qualifier="other" lang="es_ES">Arenes</dim:field>
   <dim:field mdschema="dc" element="subject" qualifier="other" lang="es_ES">Carbene</dim:field>
   <dim:field mdschema="dc" element="subject" qualifier="other" lang="es_ES">C-H activation</dim:field>
   <dim:field mdschema="dc" element="subject" qualifier="other" lang="es_ES">Iron</dim:field>
   <dim:field mdschema="dc" element="subject" qualifier="other" lang="es_ES">Manganese</dim:field>


Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias.


Relaciones con otros modelos de metadatos
-----------------------------------------

El campo **Materia** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+-------------------+
| Esquema de Metadatos | Campo Relacionado |
+======================+===================+
| dc                   | dc.subject        |
+----------------------+-------------------+
| dcterms              | dcterms.subject   |
+----------------------+-------------------+
| lom                  | lom.subject       |
+----------------------+-------------------+
| marcxml              | field:6XX         |
+----------------------+-------------------+

Niveles semánticos
------------------

No aplica

Recomendación de Campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE    | Calificadores     | Nota de alcance                                                                   |
+========================================+==========================+===================+===================================================================================+
|      **Descriptores libres**                                                                                                                                              |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               |                   | Texto Libre                                                                       |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | proposal          | Descriptores no normalizados propuestos por el autor.                             |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | classification    | Sistema de clasificación local                                                    |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
|             **Descriptores basados en vocabularios controlados**                                                                                                          |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | armarc            | Archivo en línea de autoridades de materia en español                             |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | udc               | Clasificación Universal Decimal                                                   |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | ddc               | Clasificación Decimal Dewey                                                       |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | lcc               | Clasificación Biblioteca del Congreso                                             |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | lcsh              | Encabezamientos de la Biblioteca del Congreso                                     |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | lem               | Encabezamientos de la Biblioteca Nacional de España                               |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | lemb              | Encabezamientos de la Biblioteca Luis Ángel Arango                                |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | ecm               | Encabezamientos de la Biblioteca Universidad Nacional Autónoma de México DGB/UNAM |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | mesh              | Medical Subject Headings                                                          |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | agrovoc           | Vocabulario Controlado desarrollado por FAO                                       |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | decs              | Descriptores en Ciencias de la salud - Bireme                                     |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | unesco            |                                                                                   |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | tee               |                                                                                   |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | ocde              |                                                                                   |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | jel               |                                                                                   |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | other             |                                                                                   |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire                               | dc.subject               | spines            |                                                                                   |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
|              **Descriptores con URI relacionada (Ontología, Linked Open Data)**                                                                                           |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire lcsh Linked Open Data         | dc.subject               | lcshURI           | Ejemplo: http://id.loc.gov/authorities/subjects/sh85026196.html                   |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire ddc Linked Open Data          | dc.subject               | ddcURI            | Ejemplo: http://dewey.info/class/539.7/e23/2012-06-14/about.en                    |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire udc Linked Open Data          | dc.subject               | udcURI            | Ejemplo: http://udcdata.info/037278                                               |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+
| OpenAire Agrovoc Linked Open Data      | dc.subject               | agrovocURI        | Ejemplo: http://aims.fao.org/aos/agrovoc/c_13551                                  |
+----------------------------------------+--------------------------+-------------------+-----------------------------------------------------------------------------------+

**NOTAS:**

- Se recomienda construir en DSPACE todos nombres de campos que provean una  URI relacionada (Ontología, Linked Open Data) de la siguiente forma: Nombre del Vocabulario + “URI”, por ejemplo:

    - Vocabulario: AGROVOC
    - Nombre normalizado del vocabulario: agrovoc
    - Campo en DSPACE para agregar los términos relacionados: **dc.subject.agrovoc**
    - Campo en DSPACE para agregar las URI relacionadas a los término: **dc.subject.agrovocURI**


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

  - Se recomienda específicamente crear los nuevos atributos/especificadores de campo de **subject** según la codificación propuesta.

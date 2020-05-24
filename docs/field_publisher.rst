.. _dc.publisher:

Publisher (Editor) (MA)
=======================

``dc:publisher``

Definición y alcance del campo
------------------------------
Entidad responsable de hacer que el recurso esté disponible. Los editores pueden ser personas, organizaciones o servicios. 

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio cuando sea aplicable (MA)

Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R): **0-n veces**

..

Repita este campo para describir todas las entidades responsables de la publicación editorial del recurso en **orden prioritario** ó de presentación

Esquema de metadatos
--------------------
dc.publisher

- **Nota:** Este campo se ha adaptado del esquema de metadatos DUBLIN CORE (http://dublincore.org/schemas/), e introducido en el esquema DRIVER Guidelines - elementos del idioma versión 2.

Traducción al español
---------------------
Editor, distribuidor, editorial

Forma de Descripción Normalizada (RDA / RCAA2/ ISBD)
----------------------------------------------------
RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar el editor:

	- En el caso de que sea una publicación universitaria, es importante colocar el nombre de la facultad, departamento, área o grupo que corresponda después del nombre de la Universidad. En el caso de identificar un nivel jerárquico utilice “ . ”, si son editores diferentes, registre en un nuevo campo. Si no queda clara la existencia de una jerarquía, o si se desconoce cuál es la parte más grande y más pequeña de la entidad descrita, se debe utilizar el nombre tal como aparece en el recurso de información. 
	- Aunque es opcional, se recomienda el uso de nombres de editores de listas de autoridad creadas según archivos de tesauros locales o nacionales. 
	- Adicionalmente, se recomienda evitar el uso de acrónimos o abreviaturas para la designación de una institución.


Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad de editor (publisher) (MA, 0-n):
++++++++++++++++++++++++++++++++++++++++++

Texto libre. Utilice el nombre del editor como un valor.


Relaciones con otros campos
---------------------------

	- No confundir con colaborador (MA) y creador (M). En la mayoría de los casos el colaborador y el editor no son los mismos.

Restricciones
-------------
No aplica

Ejemplos y ayudas
-----------------

Ayudas
++++++

- **dc.publisher:** Nombre del editor, distribuidor, etc. 
	- Ej: Metabiblioteca. Si hay más de dos editores se registra en un nuevo campo.

Ejemplo en XML  (Interoperabilidad OAI-PMH)
-------------------------------------------

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc.publisher>
     Universidad Nacional de Colombia. Departamento de Investigaciones.
   </dc.publisher>
   <dc.publisher>John Campos. (US)</dc.publisher>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <dc:publisher>Universidad de Huelva</dc:publisher>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   	<element name="publisher">
   	<element name="spa">
           <field name="value">Universidad Católica de Colombia. Facultad de Psicología</field>
    </element>
	</element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="publisher" lang="spa">Universidad Católica de Colombia. Facultad de Psicología</dim:field>

Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias.


Relaciones con otros modelos de metadatos
-----------------------------------------
No aplica


Niveles semánticos
------------------
No aplica


Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores | Nota de alcance                                                   |
+========================================+=======================+===============+===================================================================+
| publisher                              | dc.publisher          |               |                                                                   |
+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------+
| publisher                              | dc.publisher          | place         | Lugar de producción, publicación, distribución, manufactura, etc. |
+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------+


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------
Se recomienda específicamente crear los nuevos atributos/especificadores de campo de título según la codificación propuesta.

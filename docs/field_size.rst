.. _dci:size:

Size (Tamaño) (O)
=================

``datacite:size``

Definición y alcance del campo
------------------------------
Información del tamaño y la extensión del recurso.

Niveles de persistencia (M/MA/R/O)
----------------------------------
Opcional (O)

Niveles de ocurrencia (R / NR)
------------------------------

Repetible (R) 0-n veces

Esquema de metadatos
--------------------
datacite:size

**Nota:** Este campo se ha adaptado del esquema de metadatos DATACITE MetadataKernel versión 4.2 (http://doi.org/10.5438/0014), el cual es utilizado ampliamente para la gestión de documentos y datos. 

Traducción al español
----------------------
Tamaño / Extensión del recurso

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso). Revise la forma adecuada para ingresar el tamaño / extensión del recurso con su debida puntuación:

- Indique la descripción del tamaño recurso, incluyendo su extensión y de los materiales acompañantes. 
- Repita la propiedad para diferentes dominios de información de tamaño. 

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Clase Tamaños (sizes) (O, 0-n): 
+++++++++++++++++++++++++++++++

Usa la información del tamaño como valor de los distintos tamaños/propiedades a describir.

Propiedad Tamaño (size) (O, 0-n): 
+++++++++++++++++++++++++++++++++

Usa la información del tamaño como valor de cada una de las propiedades asociadas al recurso.

Relaciones con otros campos
---------------------------

	- Existe equivalencia semántica del campo **datacite:size** con el campo **dc.format.size** el cual es ampliamente utilizado en DSPACE

Restricciones
-------------
No aplica

Ejemplos y ayudas
-----------------

Ayudas
++++++

	- Ej:(Peso del Archivo): Coloque tamaño o extensión del recurso. Ej: 7 MB
	- Ej:(Cantidad de páginas): 65 páginas + 45 fotografías a color 
	- Ej:(Tamaño del Objeto Físico):33 x 23 cm
	- Ej:(Cantidad de elementos):: 20 diapositivas 
	- Ej:(Cantidad de Minutos): Duración 5’ 32’’

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:format>15 páginas</dc:format>
   <dc:format>33 x 23 cm</dc:format>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <datacite.sizes>
          <datacite:size>15 páginas</datacite:size>
          <datacite:size>6 MB</datacite:size>
   </datacite.sizes>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="format">
     <element name="extent">
         <element name="en_US">
                <field name="value">15 páginas</field>
         </element>
     </element>
     <element name="size">
         <element name="en_US">
                    <field name="value">33 x 23 cm</field>
         </element>
    </element>
   </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="format" qualifier="extent" lang="en_US">15 páginas</dim:field>
   <dim:field mdschema="dc" element="format" qualifier="size" lang="en_US">33 x 23 cm</dim:field>


Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias.

Relaciones con otros modelos de metadatos
-----------------------------------------

El campo tamaño **(datacite:size)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+--------------------+
| Esquema de Metadatos | Campo Relacionado  |
+======================+====================+
| dc                   | * dc.format        |
|                      | * dc.format.extent |
|                      | * dc.format.size   |
+----------------------+--------------------+
| dcterms              | dcterms:extent     |
+----------------------+--------------------+
| marcxml              | field: 300, 306    |
+----------------------+--------------------+


Niveles semánticos
------------------

No aplica

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

+----------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------+
| Esquema de Metadatos | Campo Elemento DSPACE | Calificadores | Nota de alcance                                                                           |
+======================+=======================+===============+===========================================================================================+
| dc                   | dc.format             | extent        | Extensión del recurso en páginas, tiempo, cantidad de elementos, entro otros.             |
+----------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------+
| dc                   | dc.format             | size          | Se utiliza para describir Tamaños de objetos físicos.                                     |
|                      |                       |               |   *En Bytes  para Archivos Digitales                                                      |
|                      |                       |               |   *En cm/mts para Planos y fotografías                                                    |
+----------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------+
| dc                   | dc.format             | medium        | Se utiliza para describir el soporte/medio en el cual se encuentra registrado el recurso  |
+----------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------+


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

	- Se recomienda específicamente crear los nuevos atributos/especificadores de campo de tamaño según la codificación propuesta.


.. _dc.publisher:

Publisher (Editor) (MA)
=======================

``dc.publisher``

Definición y alcance del campo
------------------------------
Entidad responsable de hacer que el recurso esté disponible. Los editores pueden ser personas, organizaciones o servicios. 

No confundir con colaborador (MA) y creador (M). En la mayoría de los casos el colaborador y el editor no son los mismos. 

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio cuando sea aplicable (MA)

Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R): **0-n veces**

..

Repita este campo para describir todas las entidades responsables de la creación del recurso en **orden prioritario** ó de presentación

Esquema de metadatos
--------------------
dc.publisher

- **Nota:** Este campo se ha adaptado del esquema de metadatos DUBLIN CORE (http://dublincore.org/schemas/), e introducido de DRIVER Guidelines - elementos del idioma versión 2.

Traducción al español
---------------------
Editor, distribuidor, editorial

Forma de Descripción Normalizada (RDA / RCAA2/ ISBD)
----------------------------------------------------
RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar el editor:

En el caso de que sea una publicación universitaria, es importante colocar el nombre de la facultad, departamento, área o grupo que corresponda después del nombre de la Universidad. En el caso de identificar un nivel jerárquico utilice “ . ”, si son editores diferentes, registre en un nuevo campo.

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad de editor (publisher) (MA, 0-n): 
++++++++++++++++++++++++++++++++++++++++++

Utilice el nombre del editor como un valor.

Relaciones con otros campos
---------------------------
No aplica

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

**Esquema xoai**

.. code-block:: xml
   :linenos:

**Esquema xoai**

.. code-block:: xml
   :linenos:

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias.


Relaciones con otros modelos de metadatos
-----------------------------------------
No aplica


Niveles semánticos
------------------
No aplica


Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear en Dspace los siguientes campos:

+----------------------------------------+-----------------------+---------------+-----------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores | Nota de alcance |
+========================================+=======================+===============+=================+
| publisher                              | dc.publisher          |               |                 |
+----------------------------------------+-----------------------+---------------+-----------------+

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------
No aplica
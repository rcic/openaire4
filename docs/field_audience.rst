.. _dct:audience:

Audience (Audiencia) (O)
========================

``dcterms:audience``

Definición y alcance del campo
------------------------------
Hace referencia al público a quien va dirigido el recurso o es útil 

Niveles de persistencia (M/MA/R/O)
----------------------------------
Opcional (O)

Niveles de ocurrencia (R / NR)
------------------------------
Repetible (NR): 0-n veces


Esquema de metadatos
--------------------
dcterms:audience

Traducción al español
---------------------
Audiencia

Forma de Descripción Normalizada (RDA/RCAA2/ISBD)
-------------------------------------------------

RDA (Recursos: descripción y acceso):

	- Texto libre. Se recomienda utilizar un texto normalizado de la entidad que debe ser mostrado para el usuario final como valor.
	- **Ámbito Profesional:** En este campo se puede utilizar para describir los ámbitos profesionales a los que estaría dirigido el recurso de información. Para este campo se recomienda utilizar el vocabulario propuesto por “Common Education Data Standards”: https://ceds.ed.gov/element/001492 
	- **Nivel Educativo:** En este campo se puede describir el nivel educativo del usuario al que va dirigido el recurso. Para  definir  este  campo  se  debe  tener  en  cuenta  el  vocabulario  controlado  propuesto  por MinEducación y los atributos que lo componen.
	- **Comunidad vinculada de MinCiencias:** en este campo también hace referencia a las comunidades científicas, académicas, empresariales del país y demás que han estado adscritas o vinculadas a diferentes proyectos con **MinCiencias.**

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad Principal Audiencia (Audience) (O, 0-n): 
++++++++++++++++++++++++++++++++++++++++++++++++++
Utilice el texto normalizado de la entidad como valor.

	- **Ámbito Profesional:**  Un ejemplo del vocabulario propuesto derivado del  “Common Education Data Standards vocabulary” se presenta a continuación:

		- Administradores
		- Grupos comunitarios
		- Consejeros
		- Receptores de fondos federales y solicitantes
		- Bibliotecarios
		- Medios de comunicación
		- Padres y familias
		- Responsables políticos
		- Investigadores
		- Personal de apoyo escolar
		- Proveedores de ayuda financiera para estudiantes
		- Estudiantes
		- Maestros
		- Público general 

	- **Nivel Educativo:** Se recomienda utilizar el siguiente vocabulario controlado:

		- Primera infancia
			- Pre-Jardín
			- Jardín
		- Preescolar
			- Transición o Grado Cero
		- Educación básica primaria
			- 1° - 3°
			- 4° - 5°
		- Educación básica secundaria
			- 6° - 7°
			- 8° - 9°
		- Educación media
			- 10° - 11°
		- Ciclo complementario
			- 12° - 13°
		- Educación para el Trabajo y el Desarrollo Humano
			- Nivel C
		- Educación superior
			- Técnica profesional
			- Tecnológica
			- Pregrado
			- Especialización
			- Maestría
			- Doctorado
			- Posdoctorado

	- **Comunidad vinculada de MinCiencias:** Texto libre. Se recomienda describir en este campo las diversas comunidades científicas y profesionales que se impactan con el uso del recurso de información.

		- Ej: Comunidad científica colombiana
		- Ej: Comunidad pesquera y acuícola
		- Ej: Comunidad agrícola de Colombia
		- Ej: Comunidad científica colombiana área de biotecnología
		- Ej: Comunidad agropecuaria
		- Ej: Comunidad apícola colombiana

Relaciones con otros campos
---------------------------
No aplica

Restricciones
-------------
No aplica

Ejemplos y ayudas
-----------------

Ayudas
------

	- **Ej: dcterms.audience.professionaldevelopment:** Investigador
	- **Ej: dcterms.audience.professionaldevelopment:** Técnico
	- **Ej: dcterms.audience.professionaldevelopment:**	Profesional

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:description>Investigadores</dc:description>
   <dc:description>Público general</dc:description>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <dcterms:audience>Investigadores</dcterms:audience>
   <dcterms:audience>Público general</dcterms:audience>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="audience">
     <element name="eng">
           <field name="value">Policymakers</field>
           <field name="value">Researchers</field>
           <field name="value">Students</field>
          <field name="value">Teachers</field>
    </element>
   </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dcterms" element="audience" lang="eng">Policymakers</dim:field>
   <dim:field mdschema="dcterms" element="audience" lang="eng">Researchers</dim:field>
   <dim:field mdschema="dcterms" element="audience" lang="eng">Students</dim:field>
   <dim:field mdschema="dcterms" element="audience" lang="eng">Teachers</dim:field>


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

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

+-----------------------------------------+-----------------------+-------------------------+------------------------------------------------------------------------------------------------+
| Vocabulario controlado OpenAire /RedCol | Campo Elemento DSPACE | Calificadores           | Nota de alcance                                                                                |
+=========================================+=======================+=========================+================================================================================================+
| OpenAire                                | dcterms.audience      |                         | Texto general                                                                                  |
+-----------------------------------------+-----------------------+-------------------------+------------------------------------------------------------------------------------------------+
| OpenAire                                | dcterms.audience      | professionaldevelopment | Una categorización de la audiencia a la que se destina la actividad de desarrollo profesional. |
+-----------------------------------------+-----------------------+-------------------------+------------------------------------------------------------------------------------------------+
| OpenAire                                | dcterms.audience      | educationalcontext      | Nivel educativo del usuario al que va dirigido el recurso.                                     |
+-----------------------------------------+-----------------------+-------------------------+------------------------------------------------------------------------------------------------+
| OpenAire                                | dcterms.audience      | redcol                  | Coloque la comunidad vinculada que ha promovido los proyectos de investigación.                |
+-----------------------------------------+-----------------------+-------------------------+------------------------------------------------------------------------------------------------+

Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

	- Se recomienda específicamente crear los nuevos atributos/especificadores del campo **Audiencia** según la codificación propuesta.

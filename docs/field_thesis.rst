.. _thesis.degree:

Thesis, Monographic work (Tesis/Trabajo de grado) (MA)
======================================================

- ``thesis:degree``

Definición y alcance del campo
------------------------------
Hace referencia a la información específica asociada a un trabajo de grado que incluye: la titulación obtenida, el nivel de estudio realizado, el área o departamento e institución donde se realizó el trabajo de grado. 

Niveles de persistencia (M/MA/R/O)
----------------------------------
Obligatorio si es aplicable (MA)

Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R)  (NR): 0-1


Esquema de metadatos
--------------------

- thesis.degree.name
- thesis.degree.level
- thesis.degree.discipline
- thesis.degree.grantor

Traducción al español
---------------------

Tesis - Disertaciones y/o trabajos de grado

	- **thesis.degree.name:** Título obtenido
	- **thesis.degree.level:** Nivel del programa académico asociado - Nivel de estudio
	- **thesis.degree.discipline:** Departamento - Programa académico
	- **thesis.degree.grantor:** Institución que otorga el grado académico.

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------

RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar los datos de **tesis:**

	- **thesis.degree.name:** Nombre del grado asociado, debe colocarle tal cual como aparece en el título obtenido o diploma de grado. Ej: Magister en Educación Virtual
	- **thesis.degree.level:** Nivel del Programa Académico Asociado - Nivel de estudio. 
	      - Ej: Doctorado 
	      - Ej: Pregrado
	      
	   **Nota:** Para este campo se recomienda utilizar el siguiente vocabulario controlado (Niveles Educación Superior MEN):
		- Técnica profesional
		- Tecnológica
		- Pregrado
		- Especialización
		- Maestría
		- Doctorado
		- Posdoctorado

	- **thesis.degree.discipline:** Se debe colocar la facultad, área o departamento relacionado con la unidad organizacional que otorga el grado. Si es necesario detallar ó especificar, se debe colocar siempre el área más grande al principio. 
	     Ej: Facultad de Ingenierías. Departamento de Ingeniería de Sistemas. Carrera de Ingeniería de Sistemas.
	     
	- **thesis.degree.grantor:** Institución que otorga el grado asociado al trabajo. Al igual que otros nombres de instituciones y entidades, este campo debe ingresarse en forma de texto libre tal como aparece en la página de título o equivalente, con un enlace a un registro de autoridad, si está disponible.Consulte la sección "Autoridad" para obtener más información. Ej: Universidad Nacional de Colombia

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Atributo de Idioma (lang) (O, 0-n): 
+++++++++++++++++++++++++++++++++++

Indicación del idioma en el que se escribe el valor de un campo. Esto es completamente independiente del elemento dc.language, que indica el idioma principal del trabajo.

Atributo de esquema (scheme) (O, 0-n): 
++++++++++++++++++++++++++++++++++++++

Descripción del vocabulario controlado o esquema utilizado para determinar los temas, materias o puntos de acceso. 

Relaciones con otros campos
---------------------------

	- No se debe confundir la institución **(thesis.degree.grantor)** que otorga el grado con el autor/colaborador del recurso de información **(datacite.contributor)**
	- Generalmente el campo editor **(dc.publisher)** es el mismo que la institución que otorga el grado **(thesis.degree.grantor).**

Restricciones
-------------
No aplica

Ejemplos y ayudas
-----------------

Ayudas
++++++

	- **thesis.degree.name:** Coloque el nombre de grado otorgado. Ej: Ingeniero de Sistemas.
	- **tesis.degree.level:** Coloque el nivel del programa cursado. Ej: Pregrado.
	- **thesis.degree.discipline:** Coloque la facultad, área, departamento o disciplina donde es perteneciente el estudio. Ej: Departamento de Ciencia de la Información. 
	- **thesis.degree.grantor:** Coloque el nombre de la institución que otorga el grado. Ej: Universidad de los Andes.

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

    <dc:desciption>Administrador de Negocios Internacionales</dc:desciption>
    <dc:publisher>Universidad de La Sabana</dc:publisher>
    <dc:publisher>Administración de Negocios Internacionales</dc:publisher>
    <dc:publisher>Escuela Internacional de Ciencias Económicas y Administrativas</dc:publisher>

..

**Esquema DataCite**

.. code-block:: xml
   :linenos:

    No aplica

..

**Esquema xoai**

.. code-block:: xml
   :linenos:

    <element name="publisher">
     <element name="es_CO">
        <field name="value">Universidad de La Sabana</field>
    </element>

    <element name="program">
         <element name="none">
            <field name="value">Administración de Negocios Internacionales</field>
        </element>
    </element>

    <element name="department">
        <element name="none">
            <field name="value">Escuela Internacional de Ciencias Económicas y Administrativas</field>
        </element>
      </element>
    </element>

	<element name="description">
     <element name="degreename">
          <element name="none">
                <field name="value">Administrador de Negocios Internacionales</field>
           </element>
    </element>

    <element name="degreelevel">
         <element name="none">
            <field name="value">Pregrado</field>
        </element>
    </element>
	</element>

..

.. code-block:: xml
   :linenos:

    <element name="thesis">
          <element name="name">
               <element name="none">
                    <field name="value">Administrador de Negocios Internacionales</field>
            </element>
          </element>

        <element name="discipline">
          <element name="none">
              <field name="value">Administración de Negocios Internacionales</field>
          </element>
     </element>
    </element>

..

**Esquema dim**

.. code-block:: xml
   :linenos:

    <dim:field mdschema="thesis" element="name" qualifier="" lang="spa">Fonoaudiología</dim:field>
    <dim:field mdschema="thesis" element="level" qualifier="" lang="spa">Pregrado</dim:field>
    <dim:field mdschema="thesis" element="discipline" qualifier="" lang="spa">Facultad de Ciencias de la Salud - Fonoaudiología</dim:field>

..

**Esquema ETD-MS**

.. code-block:: xml
   :linenos:

    <thesis.degree.name>Administradora de Empresas</thesis.degree.name>
    <thesis.degree.level>Tesis de pregrado</thesis.degree.level>
    <thesis.degree.discipline>Facultad de Administración y Contaduría</thesis.degree.discipline>
    <thesis.degree.grantor>Universidad Nacional de Colombia</thesis.degree.grantor>

..

Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a los productos de tesis de doctorado, trabajos de grado de maestría y trabajos de grado de pregrado.

Relaciones con otros modelos de metadatos
-----------------------------------------

El campo tesis del recurso de información fuente (thesis.degree) es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+-------------------------------------------------------------------------------------------------+
| Esquema de Metadatos | Campo Relacionado                                                                               |
+======================+=================================================================================================+
| marcxml              | field:502, 710                                                                                  |
+----------------------+-------------------------------------------------------------------------------------------------+
| dc                   | * thesis.degree.name: dc.description.degreename                                                 |
|                      | * thesis.degree.level: dc.description.degreelevel                                               |
|                      | * thesis.degree.discipline: dc.publisher.faculty, dc.publisher.department, dc.publisher.program |
|                      | * thesis.degree.grantor: dc.publisher                                                           |
+----------------------+-------------------------------------------------------------------------------------------------+

Niveles semánticos
------------------

No aplica

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:


+------------------------+---------------+------------------------------------------------------------------------+
| Campo Elemento DSPACE  | Calificadores | Nota de alcance                                                        |
+========================+===============+========================================================================+
| thesis (thesis.degree) | name          | Título obtenido -                                                      |
|                        |               | Este campo se puede homologar semánticamente con la combinación de:    |
|                        |               |                                                                        |
|                        |               | * dc.description.degreename                                            |
+------------------------+---------------+------------------------------------------------------------------------+
| thesis (thesis.degree) | level         | Nivel del estudio -                                                    |
|                        |               | Este campo se puede homologar semánticamente con la combinación de:    |
|                        |               |                                                                        |
|                        |               | * dc.description.degreelevel                                           |
+------------------------+---------------+------------------------------------------------------------------------+
| thesis (thesis.degree) | discipline    | Programa/Departamento/Facultad -                                       |
|                        |               | Este campo se puede homologar semánticamente con la combinación de:    |
|                        |               |                                                                        |
|                        |               | * dc.publisher.faculty (Facultad)                                      |
|                        |               | * dc.publisher.department (Departamento)                               |
|                        |               | * dc.publisher.program (Programa)                                      |
|                        |               | * dc.publisher.branch (Sede)                                           |
+------------------------+---------------+------------------------------------------------------------------------+
| thesis (thesis.degree) | grantor       | Institución que otorga el grado -                                      |
|                        |               | Este campo se puede homologar semánticamente con la combinación de:    |
|                        |               |                                                                        |
|                        |               | * dc.publisher (Institución)                                           |
+------------------------+---------------+------------------------------------------------------------------------+



Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

- Se recomienda específicamente crear los nuevos atributos/especificadores del campo **Tesis/Trabajo de grado** según la codificación propuesta.


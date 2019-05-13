.. _thesis.degree:

Tesis (MA)
==========

``thesis.degree.name``
``thesis.degree.level``
``thesis.degree.discipline``
``thesis.degree.grantor``

Definición y alcance del campo
------------------------------
Hace referencia a la titulación obtenida, nivel de estudio realizado, área o departamento e institución donde se realizó el estudio. 

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio si es aplicable (MA)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R)

Campo con esquema de metadatos
------------------------------
- thesis.degree.name
- thesis.degree.level
- thesis.degree.discipline
- thesis.degree.grantor

Traducción al español
---------------------
Tesis

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)
 
Revise la forma adecuada para ingresar el título obtenido con su debida puntuación:

- **thesis.degree.name:** Nombre del grado asociado, debe colocarle tal cual como aparece en el título obtenido o diploma de grado.

	Ej: Magistra en Educación Virtual

- **thesis.degree.level:** Son válidos los siguientes niveles:

	- Pregrado
	- Maestría
	- Doctorado
	- Postdoctorado

		Ej: Tesis de doctorado

- **thesis.degree.discipline:** Se debe colocar la facultad, área o departamento de donde es perteneciente el estudio. Si es necesario segregar colocar siempre el área más grande al principio.

	Ej: Facultad de Ingenierías. Departamento de Ingeniería de Sistemas. Carrera de Ingeniería de Sistemas.

- **thesis.degree.grantor:** Institución que otorga el grado asociado al trabajo. Al igual que otros nombres de instituciones y entidades, este campo debe ingresarse en forma de texto libre tal como aparece en la página de título o equivalente, con un enlace a un registro de autoridad, si está disponible.Consulte la sección "Autoridad" para obtener más información.

	Ej: Universidad Nacional de Colombia


Valores permitidos (Vocabularios Controlados)
---------------------------------------------

- thesis.degree.name
- thesis.degree.level
- thesis.degree.discipline
- thesis.degree.grantor

Relaciones con otros campos
---------------------------

- thesis.degree.name
- thesis.degree.level
- thesis.degree.discipline
- thesis.degree.grantor

Restricciones
-------------


Ejemplos
--------

.. block-code:: xml
   :linenos:

   	<thesis.degree.name>Administradora de Empresas</thesis.degree.name>
   	<thesis.degree.level>Tesis de pregrado</thesis.degree.level>
   	<thesis.degree.discipline>Facultad de Administración y Contaduría</thesis.degree.discipline>
   	<thesis.degree.grantor>Universidad Nacional de Colombia</thesis.degree.grantor>

Atributos de campo 
------------------

- thesis.degree.name
- thesis.degree.level
- thesis.degree.discipline
- thesis.degree.grantor

Especificadores de campo
------------------------

- thesis.degree.name
- thesis.degree.level
- thesis.degree.discipline
- thesis.degree.grantor

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a los productos de tesis de doctorado, trabajos de grado de maestría y trabajos de grado de pregrado.

Relaciones con otros modelos de metadatos
-----------------------------------------

- dc.creator.degree
- dc.publisher.program
- dc.publisher.department
- dc.creator.degreetype

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear los siguientes campos en Dspace:

- thesis.degree.name
- thesis.degree.level
- thesis.degree.discipline
- thesis.degree.grantor

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------
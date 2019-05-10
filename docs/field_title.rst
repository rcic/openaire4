.. _dci:title:

.. _dci:title_title:

Título (M)
==========

``datacite:title``

Definición y alcance del campo
------------------------------
Nombre del recurso o variantes del mismo. Este campo puede utilizarse para generar puntos de acceso con despliegue a los diversos títulos existentes.

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R)

Campo con esquema de metadatos
------------------------------
datacite:title

Traducción al español
---------------------
Título

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar la información de título con su debida puntuación:

- **Título:** Ingrese el título del recurso, la primera letra en mayúscula y finalice con punto. Ej: Acuerdos de paz en Colombia.

- **Otro título:** Ingrese un título adicional del recurso. Ejemplo: Políticas de los acuerdos de paz en Colombia. 

- **Subtítulo:** Seguido del título principal del recurso colo espacio : espacio e ingrese el subtítulo. Ejemplo: Acuerdos de paz en Colombia : una mirada al conflicto armado.

- **Título alternativo:** Coloque el título alternativo del recurso si lo tiene. Ej: Paz en Colombia. 

- **Título traducido:** Coloque la traducción del título del recurso. Ej: Peace agreements in Colombia.

- **Variante del título:** Es la forma de un título que aparece en diferentes partes del recurso y es diferente al título registrado en el campo datacite:title. Ej: Colombia y sus acuerdos de paz. 
	

Valores permitidos (Vocabularios Controlados)
---------------------------------------------

- title type
- title.othertitle
- title.alternative
- title.translated
- title.variant

Relaciones con otros campos
---------------------------

- Otro título
- Subtítulo
- Título alternativo
- Título traducido
- Variante del título


Restricciones
-------------

Ejemplos
--------
Estudio para identificar conocimientos, capacidades, percepciones y experiencias de los investigadores del país frente a la ciencia abierta


.. code-block:: xml
   :linenos:

    <datacite:title xml:lang="en-US">
      Estudio para identificar conocimientos, capacidades, percepciones y experiencias de los investigadores del país frente a la ciencia abierta
    </datacite:title>
    <datacite:title xml:lang="en-US" titleType="Subtitle">A survey</datacite:title>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

..

Atributos de campo
------------------
title type

Especificadores de campo
------------------------
type

Niveles de aplicación para  productos de investigación de Colciencias
---------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------
dc.title

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear en Dspace los siguientes campos:

- dc.title.othertitle
- dc.title.alternative
- dc.title.translated
- dc.title.variant


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

- **OpenAire 3:** dc.title
- **BDCOL:** dc.title, dc.title.short, dc.title.full, dc.title.full.unstemmed


.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
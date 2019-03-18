.. _dci:title:

.. _dci:title_title:

Título (M)
==========

``datacite:title``

Nombre del campo
----------------

Campo normalizado:
~~~~~~~~~~~~~~~~~~
title

Campo con esquema de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
datacite:title

Traducción al español:
~~~~~~~~~~~~~~~~~~~~~~
Título

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de Ocurrencia (R/NR - Cantidad Veces)
---------------------------------------------
Repetible (R)

Definición y Alcance del campo
------------------------------
Nombre del recurso o variantes del mismo. Este campo puede utilizarse para generar puntos de acceso con despliegue a los diversos títulos existentes.

Forma de Descripción Normalizada (RDA/RCAA2)
-----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
title type

Relaciones con otros campos
~~~~~~~~~~~~~~~~~~~~~~~~~~~
- Otro título
- Subtítulo      	
- Título abreviado
- Título anterior
- Título clave
- Título uniforme
- Título uniforme colectivo
- Traducción del título por agencia catalogadora
- Variante del título

Restricciones
~~~~~~~~~~~~~

Ejemplos
~~~~~~~~
Estudio para identificar conocimientos, capacidades, percepciones y experiencias de los investigadores del país frente a la ciencia abierta.

.. code-block:: xml
   :linenos:

    <datacite:title xml:lang="en-US">
      Estudio para identificar conocimientos, capacidades, percepciones y experiencias de los investigadores del país frente a la ciencia abierta
    </datacite:title>
    <datacite:title xml:lang="en-US" titleType="Subtitle">A survey</datacite:title>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

Atributos de Campo
------------------
title type

Especificadores de Campo
------------------------

Niveles de Aplicación - Productos de Colciencias
------------------------------------------------
Se aplica a todos los productos de Colciencias.

Observaciones del Campo
-----------------------

Adaptado de
~~~~~~~~~~~

Relaciones con otros modelos de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Niveles Semánticos
~~~~~~~~~~~~~~~~~~

Recomendación de Campos de aplicación en DSPACE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LAREFERENCIA, OPENAIRE2, OPENAIRE3)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Para realizar la migración correcta de metadatos, se deben revisar los siguientes modelos de migración y ajustarlos al nuevo esquema de metadatos Openaire 4. 

OpenAire 3: dc.title
BDCOL: dc.title, dc.title.short, dc.title.full, dc.title.full.unstemmed

Otras Observaciones
~~~~~~~~~~~~~~~~~~~

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
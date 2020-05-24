.. _dc.format:

Format (Formato) (R)
====================

``dc:format``


Definición y alcance del campo
------------------------------
Hace referencia a la manifestación física o digital del recurso, se puede incluir el medio del recurso. El formato es una guía para el usuario que le permite determinar el software o hardware necesario para operar el recurso.

Niveles de persistencia (M/MA/R/O)
-----------------------------------
Recomendado (R)

Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R) : 0-n **veces**

Esquema de metadatos
--------------------
dc:format

Traducción al español
---------------------
Formato

Forma de Descripción Normalizada (RDA / RCAA2/ ISBD)
----------------------------------------------------
RDA (Recursos: descripción y acceso).

   - El campo formato del recurso de información está íntimamente ligado con el contenido y la extensión de los nombres del archivos adjuntos.
   - La práctica recomendada consiste en seleccionar un valor de la lista registrada de IANA de tipos de medios de Internet (tipos MIME) cuyos valores admitidos están controlados por un vocabulario que se encuentra en: http://www.iana.org/assignments/media-types/media-types.xhtml 
   - Adicionalmente incluye información del soporte (físico/digital) utilizado y el medio requerido para acceder al recurso (Cloud, CD, DVD, etc..) si aplica.

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad de Formato (Format) (R, 1-n):
+++++++++++++++++++++++++++++++++++++++++++++++++

Use la Manifestación física o digital del recurso como un valor.


Relaciones con otros campos
---------------------------

   - No confundir el formato del recurso **(dc.format)** con el tipo de recurso **(oaire:resourceType)**
   - No confundir el formato del recurso **(dc.format)** con el identificador del recurso (datacite:identifier).

Restricciones
-------------
Ninguna

Ejemplos y ayudas
------------------

Ayudas
++++++

   - Ej: Formato PDF: application/pdf
   - Ej: Formato XML: application/xml

Ejemplo en XML  (Interoperabilidad OAI-PMH)
+++++++++++++++++++++++++++++++++++++++++++


**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc.format>video/quicktime</dc.format>
   <dc.format>application/pdf</dc.format>
   <dc.format>application/xml</dc.format>
   <dc.format>application/xhtml+xml</dc.format>
   <dc.format>application/html</dc.format>
   <dc.format>application/vnd.oasis.opendocument.text</dc.format>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <dc:format>application/pdf</dc:format>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="format">
      <element name="mimetype">
           <element name="spa">
             <field name="value">application/pdf</field>
          </element>
     </element>
   </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="format" lang="es">pdf-A/3</dim:field>

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="format" qualifier="mimetype" lang="spa">application/pdf</dim:field>


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

+-----------------------+---------------+-----------------------------------------------+
| Campo Elemento DSPACE | Calificadores | Nota de alcance                               |
+=======================+===============+===============================================+
| dc.format             |               | Incluir aquí, Descripción general del formato |
+-----------------------+---------------+-----------------------------------------------+
| dc.format             | mimetype      | Incluir aquí el formato codificado IANA       |
+-----------------------+---------------+-----------------------------------------------+
| dc.format             | medium        | Incluir aquí el Soporte Físico asociado       |
+-----------------------+---------------+-----------------------------------------------+


Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

Se recomienda específicamente crear los nuevos atributos/especificadores de campo de título según la codificación propuesta.


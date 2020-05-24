.. _dc.coverage:

Coverage (Cobertura) (R)
========================

``dc:coverage``

Definición y alcance del campo
------------------------------
Este campo describe la cobertura **espacial ó temporal** sobre el cual trata el recurso de información. La cobertura generalmente incluirá la ubicación espacial (un nombre del lugar o coordenadas geográficas), el período temporal (una etiqueta del período, la fecha o el rango de fechas) o la jurisdicción (como una entidad administrativa nombrada). La mejor práctica recomendada es seleccionar un valor de un vocabulario controlado.  

Niveles de persitencia (M/MA/R/O)
------------------------------------
Obligatorio (MA)

Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R): 0-n veces

Esquema de metadatos
------------------------------
dc:coverage

Traducción al español
---------------------
Cobertura Espacial / Cobertura Temporal

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar el identificador del recurso:

	- Para el caso de describir ciudades y países separe con una como (,). Y siga la misma estructura para demás delimitaciones geográficas. 
		Ej: Bogotá, Colombia
		Ej: Aguachica, Cesar, Colombia 
		Ej: Aguacatico, Medio Baudó, Chocó, Colombia

	- También puede incluir subdivisiones geográficas cronológicas (años, siglos, décadas, etc.)
		Ej: Siglo XIV
		Ej: China - Siglo XX
		Ej: Tolima, Colombia - 1950-2000

**NOTAS:**

	- Para el caso de proyectos de investigación asociados a los productos descritos, se recomienda utilizar el campo **(dc.coverage.projectdates)** que contiene un rango de fechas de inicio / finalización del proyecto de investigación en formato normalizado (AAA-MM-DD/AAAA-MM-DD) Ej: **10/02/2013-16/07/2015**

Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad Principal Cobertura (coverage) (O, 0-n):
++++++++++++++++++++++++++++++++++++++++++++++++++

Utilice un período temporal o geográfico como valor del campo.

Relaciones con otros campos
---------------------------

- No confundir la cobertura espacial de la que trata el contenido del recurso de información **(dc.coverage.spatial)** con la localización geográfica/espacial en la cual fue realizada la investigación ó publicado el recurso de información, creados los documentos, tomados los datos y que deberían ser registrados en el campo **(datacite:geoLocation).** 
- Para indicar el lugar de producción, publicación, distribución, manufactura, etc, utilice el campo **(dc.publisher.place)**

Restricciones
-------------
Ninguna

Ejemplos y ayudas
-----------------

Ayudas
++++++

	- Ej: (Cobertura Temporal): 2000-2010
	- Ej: (Cobertura Espacial): Guaduas, Tolima, Colombia
	- Ej: (Cobertura Espacial TGN):http://vocab.getty.edu/page/tgn/7005073 
	- Ej: (Coordenadas): Longitud: O75°33'48.92" Latitud: N6°15'6.62"
	- Ej: (Rango de Fechas): dc.coverage.temporal	10/02/2013-16/07/2015

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

  	<dc.coverage>2000-2010</dc.coverage>
	<dc.coverage>Siglo XX</dc.coverage>
	<dc.coverage>Amazonas, Colombia</dc.coverage>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <dc:coverage>Europa</dc:coverage>
   <dc:coverage>Latinoamérica</dc:coverage>
   <dc:coverage>Iberoamérica</dc:coverage>
   <dc:coverage>10/02/2013-16/07/2015</dc:coverage>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="coverage">
    <element name="spatial">
        <element name="spa">
             <fieldname="value">Cali; Lat: 03 24 00 N degrees minutes; Lat: 3.4000 decimal degrees; Long: 076 30 00 W degrees minutes; Long: -76.5000 decimal degrees</field>
        </element>
    </element>
   </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="coverage" element="spatial" lang="spa">Cali; Lat: 03 24 00 N degrees minutes; Lat: 3.4000 decimal degrees; Long: 076 30 00 W degrees minutes; Long: -76.5000 decimal degrees</dim:field>

Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias. 


Relaciones con otros modelos de metadatos
-----------------------------------------

El campo cobertura **(dc.coverage)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

======================  ===================
Esquema de Metadatos    Campo Relacionado  
======================  ===================
dc                      dc.coverage        
dcterms                 dcterms.coverage   
marcxml                 field: 651         
======================  ===================

Niveles semánticos
------------------

Cuando aplique, se recomienda seleccionar un valor de un vocabulario controlado (por ejemplo, del Thesaurus of Geographic Names (TGN) y especificar la URL del término utilizado (https://www.getty.edu/research/tools/vocabularies/tgn/).

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

+----------------------+-----------------------+---------------+------------------------------------------------------------------------------+
| Esquema de Metadatos | Campo Elemento DSPACE | Calificadores | Nota de alcance                                                              |
+======================+=======================+===============+==============================================================================+
| dc                   | dc.coverage           |               | Cobertura, texto general                                                     |
+----------------------+-----------------------+---------------+------------------------------------------------------------------------------+
| dc                   | dc.coverage           | spatial       | Cobertura Espacial Texto General                                             |
+----------------------+-----------------------+---------------+------------------------------------------------------------------------------+
| dc                   | dc.coverage           | temporal      | Cobertura Temporal Texto General                                             |
+----------------------+-----------------------+---------------+------------------------------------------------------------------------------+
| dc                   | dc.coverage           | projectdates  | Rango de fechas de ejecución del proyecto asociado al recurso de información |
+----------------------+-----------------------+---------------+------------------------------------------------------------------------------+
| dc                   | dc.coverage           | tgn           | Cobertura Espacial Tesauro TGN                                               |
+----------------------+-----------------------+---------------+------------------------------------------------------------------------------+
| dc                   | dc.coverage           | country       | Cobertura Espacial Nombre de País                                            |
+----------------------+-----------------------+---------------+------------------------------------------------------------------------------+
| OpenAire             | dc.coverage           | city          | Cobertura Espacial Nombre de Ciudad                                          |
+----------------------+-----------------------+---------------+------------------------------------------------------------------------------+
| OpenAire             | dc.coverage           | region        | Cobertura Espacial Nombre de Región ó municipio relacionado                  |
+----------------------+-----------------------+---------------+------------------------------------------------------------------------------+
| OpenAire             | dc.coverage           | box           | Cobertura Espacial Coordenadas                                               |
+----------------------+-----------------------+---------------+------------------------------------------------------------------------------+

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

	- Se recomienda específicamente crear los nuevos atributos/especificadores del campo **coverage** según la codificación propuesta.

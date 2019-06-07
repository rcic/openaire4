.. _dc.source:

Source (Fuente) (R) 
===================

``dc.source``

Definición y alcance del campo
------------------------------
Hace referencia a un recurso del cual se deriva el recurso presente. El recurso fuente puede derivarse en su totalidad o en partes. La mejor práctica recomendada es hacer referencia al recurso por medio de una cadena o número que se ajuste a un sistema de identificación formal.

En este campo también se incluye información sobre la bibliografía (referencias bibliográficas) que contiene el recurso. 

Niveles de persistencia (M/MA/R/O)
------------------------------------
Recomendado (R)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R): **0-n veces**

..

Nota: Repita este campo utilizando los distintos atributos de fuente según se considere.

Esquema de metadatos
--------------------

dc.source

Traducción al español
---------------------

Fuente del recurso / Bibliografía / Fuente Bibliográfica

Forma de Descripción Normalizada (RDA / RCAA2)
-----------------------------------------------
**RDA (Recursos: descripción y acceso):** Revise la forma adecuada para ingresar la información de la fuente con su debida puntuación:

	- **Fuente:** Ingrese la fuente principal de donde se tomo el recurso. Ej: Documentos CEDE. 
	- **Fuente URL:** Utilice cuando el mismo recurso de información haya sido publicado,  se encuentra disponible en otro sistema de información en Internet (URL) y este haya sido la fuente del cual se toma el documento para publicarlo en el sistema de información local.
	- **Fuente de citación bibliográfica:** Ingrese las referencias bibliográficas del recurso. Se recomienda tomarlas tal cual como aparecen en el recurso. Ej: Frank, R. H., & Bernanke, B. (2007). Principios de microeconomía. (3rd ed.). Boston, MA: McGraw-Hill/Irwin. 

Propiedades, atributos y especificadores de campo
-------------------------------------------------


Propiedad Fuente (Source) (R, 0-n):
+++++++++++++++++++++++++++++++++++

Utilice la información de la fuente como valor.

Para tener una guía de los estilos de citación, se recomienda revisar las siguientes normas:

- **APA (American Psychological Association):**  Este estilo ya cuenta con seis ediciones y explica cómo se deben presentar artículos científicos: márgenes, fuente, tamaño de letra, uso de color, gráficas, tablas, y citación y referenciación. 
- **ICONTEC:** Estas normas fueron definidas por el comité técnico del Instituto Colombiano de Normas Técnicas y Certificación, el cual es un organismo multinacional de carácter privado, dedicado a la gestión de la calidad en Colombia, Chile, Ecuador, El Salvador, Guatemala, Honduras y Perú.
- **IEEE (Institute of Electrical and Electronics Engineers):** Este estilo de citación es definido por la asociación científica internacional de técnicos e ingenieros dedicados a la estandarización y desarrollo, es el más utilizado en áreas de ingeniería para todo tipo de documentos. 
- **MLA (Modern Language Association):** Es un estilo y formato de citación bibliográfica para revistas, libros y otro tipo de textos académicos. Es utilizado principalmente en áreas de humanidades y artes,​ sobre todo en filosofía, crítica literaria, literatura comparada y en campos interdisciplinarios, como los estudios culturales.
- **VANCOUVER:** Este estilo de citación válidas para todo tipo de documentos específico para las áreas de Ciencias de la Salud.

Relaciones con otros campos
---------------------------

	- Si la fuente del recurso descrito es el resultado de la digitalización de originales utilice el campo dc.source, de lo contrario, utilice el campo: dc.relatedIdentifier.
	- Opcionalmente, se pueden agregar metadatos sobre la ubicación actual y el número de llamada de la publicación digitalizada.
	- No confundir con el campo Identificador de recurso (resource.Identifier), ni con el campo identificador del recurso relacionado (relatedIdentifier).
	- Cuando se esté describiendo un recurso de información del tipo analítico, los datos del documento anfitrión deben ser descritos en los campos “oaire.citation.” 
	- Las citas bibliográficas también se pueden describir utilizando exclusivamente un identificador normalizado a través del uso del campo identificador del recurso relacionado (relatedIdentifier) con el atributo tipo de relación  (relationType) que contenga el valor “Cites”.

.. code-block:: xml
	:linenos:

	<relatedIdentifier relatedIdentifierType="DOI"relationType="Cites">10.4232/10.ASEAS-5.2-1 </relatedIdentifier> 

Restricciones
-------------

No aplica

Ejemplos y ayudas
-----------------

**Esquema oai_dc**

Ayudas
++++++

	- **Fuente:** Coloque la fuente principal de donde se tomo el recurso. Ej: Cuadernos de Economía. 
	- **Fuente URL (Directrices OpenAire):** https://openaire-guidelines-for-literature-repository-managers.readthedocs.io/en/v4.0.0/index.html 
	- **Fuente de citación bibliográfica:** Ingrese las referencias bibliográficas del recurso. Se recomienda tomarlas tal cual como aparecen en el recurso. Ej: Loyola A, Tagami H, Bonaldi T, Roche D, Quivy JP, Imhof A, et al. The HP1alpha-CAF1-SetDB1-containing complex provides H3K9me1 for Suv39-mediated K9me3 in pericentric heterochromatin. EMBO Rep [Internet]. 2009 Jul;10(7):769–75.

Ejemplo en XML  (Interoperabilidad OAI-PMH)
+++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc.source>Cuadernos de ecología volumen 4 (2001)</dc.source>


**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <dc:source>Ecology  Letters (1461023X)  vol.4 (2001)</dc:source>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="dcterms">
      <element name="bibliographicCitation">
         <element name="spa">
                 <field name="value">ABColombia, Corporación SISMA Mujer y The U.S. Office en Colombia (USOC) (2013). Colombia: Women, conflict – related sexual violence and the peace process. Recuperado de https://www.christianaid.org.uk/images/ABColombia-conflict-relatedsexual-violence-report.pdf</field>
       </element> 
     </element> 
   </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dcterms" element="bibliographicCitation" lang="spa">Arias, A. (2008). Multiculturalismo y Derechos Indígenas. El caso mexicano. México D.F: Comisión Nacional de los Derechos Humanos.</dim:field>


Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

El campo Fuente es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+--------------------------------------+
| Esquema de Metadatos | Campo Relacionado                    |
+======================+======================================+
| dc                   | * dc.source                          |
|                      | * dc.soruce.bibliographicCitation    |
+----------------------+--------------------------------------+
| dcterms              | * dcterms.source                     |
|                      | * dcterms.bibliographicCitation      |
+----------------------+--------------------------------------+
| lom                  | lom.source                           |
+----------------------+--------------------------------------+
| marcxml              | field:504                            |
+----------------------+--------------------------------------+

Niveles semánticos
------------------

- Se aplica equivalencia semántica para los campos dc.source.bibliographicCitation y dcterms.bibliographicCitation

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

+----------------------------------------+-----------------------+-----------------------+-----------------------------------------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores         | Nota de alcance                                           |
+========================================+=======================+=======================+===========================================================+
| OpenAire                               | dc.source             |                       | Texto libre que contiene la Fuente principal del recurso. |
+----------------------------------------+-----------------------+-----------------------+-----------------------------------------------------------+
| Redcol                                 | * dc.source           | bibliographicCitation | Cita bibliográfica                                        |
|                                        | * dc.source dcterms   |                       |                                                           |
+----------------------------------------+-----------------------+-----------------------+-----------------------------------------------------------+


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

Se recomienda específicamente crear los nuevos atributos/especificadores de campo de título según la codificación propuesta.

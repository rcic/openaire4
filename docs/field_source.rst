.. _dc.source:

Source (Fuente) (R) 
===================

``dc:source``

Definición y alcance del campo
------------------------------
Hace referencia a un recurso del cual se deriva el recurso presente. El recurso fuente puede derivarse en su totalidad o en partes. La mejor práctica recomendada es hacer referencia al recurso por medio de una cadena o número que se ajuste a un sistema de identificación formal.

Es recomendable utilizar este campo sólo si el recurso descrito es el resultado de la digitalización de originales no digitales ó si el mismo recurso publicado fue tomado integralmente de otro lugar, de lo contrario, utilizar el elemento ‘relation’ con sus respectivo cualificadores.
 

Niveles de persistencia (M/MA/R/O)
------------------------------------
Recomendado (R)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R): **0-n veces**

- **Nota:** Repita este campo utilizando los distintos atributos de fuente según se considere.

..

Esquema de metadatos
--------------------

dc.source

Traducción al español
---------------------

Fuente/Origen del recurso 

Forma de Descripción Normalizada (RDA / RCAA2)
-----------------------------------------------
**RDA (Recursos: descripción y acceso):** Revise la forma adecuada para ingresar la información de la fuente con su debida puntuación:

- **Fuente (Texto Libre):** Ingrese la fuente principal de donde se tomo el recurso. Ej: Documentos CEDE. 
- **Fuente URL:** Utilice cuando el mismo recurso de información haya sido publicado,  se encuentra disponible en otro sistema de información en Internet **(URL)** y este haya sido la fuente del cual se toma el documento para publicarlo en el sistema de información local. 

Propiedades, atributos y especificadores de campo
-------------------------------------------------


Propiedad Fuente (Source) (R, 0-n):
+++++++++++++++++++++++++++++++++++

Utilice la información de la fuente (origen) como valor.


Relaciones con otros campos
---------------------------

- Para la gestión de **referencias bibliográficas (bibliografía)** del recurso se recomienda utilizar el campo **dc.relation.references (dcterms.references).**
- Si la fuente del recurso descrito es el resultado de la digitalización de originales utilice el campo **dc.source,** de lo contrario, utilice el campo: **dc.relatedIdentifier.**
- Opcionalmente, se pueden agregar metadatos sobre la ubicación actual y el número de llamada de la publicación digitalizada.
- No confundir con el campo Identificador de recurso **(resource.Identifier),** ni con el campo **identificador del recurso relacionado (relatedIdentifier).**
- Cuando se esté describiendo un recurso de información del tipo analítico, los datos del documento anfitrión deben ser descritos en los campos **“oaire.citation.”** 
- Las citas bibliográficas también se pueden describir utilizando exclusivamente un identificador normalizado a través del uso del campo **identificador del recurso relacionado (relatedIdentifier)** con el atributo **tipo de relación (relationType)** que contenga el valor “Cites”. 

.. code-block:: xml
	:linenos:

	<relatedIdentifier relatedIdentifierType="DOI"relationType="Cites">10.4232/10.ASEAS-5.2-1 </relatedIdentifier>

Restricciones
-------------

No aplica

Ejemplos y ayudas
-----------------

Ayudas
++++++

- **Fuente:** Coloque la fuente principal de donde se tomo el recurso. Ej: Cuadernos de Economía. 
- **Fuente URL (Directrices OpenAire):** https://openaire-guidelines-for-literature-repository-managers.readthedocs.io/en/v4.0.0/index.html 

Ejemplo en XML  (Interoperabilidad OAI-PMH)
+++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc.source>Cuadernos de ecología volumen 4 (2001)</dc.source>

.. code-block:: xml
   :linenos:

   <dc.source>Escultura del Museo Nacional de Colombia</dc.source>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <dc:source>Ecology  Letters (1461023X)  vol.4 (2001)</dc:source>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="dc">
      <element name="source">
         <element name="spa">
                 <field name="value">ABColombia, Corporación SISMA Mujer y The U.S. Office en Colombia (USOC) (2013). Colombia: Women, conflict – related sexual violence and the peace process. Recuperado de https://www.christianaid.org.uk/images/ABColombia-conflict-relatedsexual-violence-report.pdf</field>
       </element> 
     </element> 
   </element> 

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="source" lang="spa">Arias, A. (2008). Multiculturalismo y Derechos Indígenas. El caso mexicano. México D.F: Comisión Nacional de los Derechos Humanos.</dim:field>


Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

El campo **Fuente** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+--------------------------------------+
| Esquema de Metadatos | Campo Relacionado                    |
+======================+======================================+
| dc                   | * dc.source                          |
+----------------------+--------------------------------------+
| dcterms              | * dcterms.source                     |
+----------------------+--------------------------------------+
| lom                  | lom.source                           |
+----------------------+--------------------------------------+
| marcxml              | field:504                            |
+----------------------+--------------------------------------+

Niveles semánticos
------------------

No aplica.

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

+----------------------------------------+-----------------------+---------------+-----------------------------------------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores | Nota de alcance                                           |
+========================================+=======================+===============+===========================================================+
| OpenAire                               | dc.source             |               | Texto libre que contiene la Fuente principal del recurso. |
+----------------------------------------+-----------------------+---------------+-----------------------------------------------------------+


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

Se recomienda específicamente crear los nuevos atributos/especificadores de campo de título según la codificación propuesta.

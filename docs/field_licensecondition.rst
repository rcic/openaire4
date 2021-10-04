.. _aire:licenseCondition:

License Condition (Condición de la licencia) (MA)
================================================

``oaire:licenseCondition``

Definición y alcance del campo
------------------------------
Información sobre los derechos de la licencia. Está información deberá contener los derechos de autor y de propiedad intelectual definidos por la institución, de igual forma derechos de uso y reutilización del recurso. 
Se recomienda se haga claridad entre la autorización dada por el autor del recurso de información a la institución que publica el recurso en el Repositorio y la autorización/licencia de uso brindada por la institución que gestiona el Repositorio institucional a todos los usuarios del mismo. Para el primer caso, se recomienda que se genere un documento anexo al recurso de información y no se gestione como un campo de metadatos.

Pueden utilizarse las licencias de Creative Commons. 

Niveles de persistencia (M/MA/R/O)
----------------------------------
Obligatorio cuando sea aplicable (MA)

Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R): 1-n veces

Esquema de metadatos
------------------------------
oaire:licenseCondition

Traducción al español
---------------------
Condición de la licencia - derechos de autor

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
Revise la forma adecuada para ingresar la condición de licencia con su debida puntuación:

	- Este campo puede contener  un texto en el cual se hace una declaración de gestión de derechos para acceder o utilizar el objeto o una referencia
	- Es preferible hacer referencia a una URL que contiene el texto/condiciones de la licencia. 
	- Cuando se utiliza el modelo de licenciamiento provisto por la organización “Creative Commons”, existen URI que identifica de manera unívoca cada uno de sus modelos de licencia en las diferentes jurisdicciones.
	- Se pueden utilizar conjuntamente en un mismo ítem los campos de  Copyright y Creative Commons bajo la premisa que “Las licencias Creative Commons te ayudan a mantener el derecho de autor o copyright, pero a la vez permiten ciertas excepciones con respecto a él, bajo ciertas condiciones“[#]_


Propiedades, atributos y especificadores de campo
-------------------------------------------------

Propiedad Principal Condiciones de licencia (licenseCondition ) (MA, 0-n): 
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Utilice el nombre de la licencia como valor.

	- **Atributo: URI (uri) (MA, 1):** La URI proporciona la ubicación donde se puede leer la licencia. Con las licencias **“Creative Commons”,** el tipo de licencia se puede reconocer directamente en el nombre de la URL relacionada.

	- **Atributo: Fecha de inicio (startDate) (MA, 1):** Este atributo indica la fecha en que la licencia entra en vigor.  La mejor práctica recomendada para codificar el valor de la fecha según la norma ISO 8601 [W3CDTF] que sigue el formato AAAA-MM-DD.


Relaciones con otros campos
---------------------------

	- Cuando el  valor de la Fecha de inicio **(startDate)**  es omitido, se toma como fecha de inicio de la validez de la licencia la información que se presenta en los campos Fecha de creación **(dc.date.created)** y Fecha de publicación **(dc.date.issued)** en estricto orden de prioridad.

Restricciones
-------------
No aplica

Ejemplos y ayudas
-----------------

Ayudas
++++++

	- **URI:** Coloque la URI de la licencia que tendrá el recurso:
   	        --Ej: http://creativecommons.org/licenses/by-nc-nd/2.5/co/
	- **Licencia Uso:** Texto asociado al tipo de licencia de uso. 
	        --Ej: “Atribución-NoComercial-SinDerivadas 2.5 Colombia (CC BY-NC-ND 2.5 CO)”
	- **Licencia Autorización:** Coloque el texto que la institución previamente definió según las tipologías documentales definidas. 
	        --Ej: “EL AUTOR, manifiesta que la obra recurso/objeto de la presente autorización es original y la realizó sin violar o usurpar derechos de autor de terceros, por lo tanto la obra es de exclusiva autoría y tiene la titularidad sobre la misma. PARÁGRAFO: En caso de presentarse cualquier reclamación por parte de un tercero en cuanto a los derechos de autor sobre la obra en cuestión, EL AUTOR, asumirá toda la responsabilidad, y saldrá en defensa de los derechos aquí autorizados.”

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:rights>Copyright Universidad Católica de Colombia 2016</dc:rights>
   <dc:rights>info:eu-repo/semantics/openAccess</dc:rights>
   <dc:rights>http://creativecommons.org/licenses/by-nc/4.0/</dc:rights>

**Esquema DataCite/oaire/oai_openaire**

.. code-block:: xml
   :linenos:

   <oaire:licenseCondition startDate="2019-02-01" uri="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial</oaire:licenseCondition>

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="rights">
     <element name="spa">
       <field name="value">Copyright Universidad Católica de Colombia 2016</field>
     </element> 
	 <element name="creativecommons">
         <element name="spa">
           <field name="value">Attribution 4.0 International (CC BY 4.0)</field>
         </element>
	</element>	
    <element name="uri">
          <element name="spa">
            <field name="value">http://creativecommons.org/licenses/by-nc/4.0</field>
          </element>
	</element>
   </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

    <dim:field mdschema="dc" element="rights" qualifier="uri" lang="spa">http://creativecommons.org/licenses/by-nc/4.0/</dim:field>
    <dim:field mdschema="dc" element="rights" qualifier="creativecommons" lang="spa">Attribution 4.0 International (CC BY 4.0)</dim:field>



Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

El campo Condición de la licencia **(oaire:licenseCondition)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+-------------------+
| Esquema de Metadatos | Campo Relacionado |
+======================+===================+
| dc                   | dc.rights         |
+----------------------+-------------------+
| dcterms              | dcterms.rights    |
+----------------------+-------------------+
| marcxml              | field: 540 / 542  |
+----------------------+-------------------+


Niveles semánticos
------------------

No Aplica

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

+-----------------------+---------------------+----------------------------------------------------------------------------+
| Campo Elemento DSPACE | Calificadores       | Nota de alcance                                                            |
+=======================+=====================+============================================================================+
| dc.rights             |                     | Texto general de licencia/Copyright                                        |
+-----------------------+---------------------+----------------------------------------------------------------------------+
| dc.rights             |* "creativecommons"  | Texto indicador del tipo de licencia utilizado                             |
|                       |* "licence"          | Para Creative Commons utilice el texto normalizado provisto                |
|                       |                     | * Attribution 4.0 International (CC BY 4.0)                                |
|                       |                     | * Atribución-NoComercial-SinDerivadas 2.5 Colombia (CC BY-NC-ND 2.5 CO)    |
|                       |                     |                                                                            |
+-----------------------+---------------------+----------------------------------------------------------------------------+
| dc.rights             |* uri                | URL a un documento de Licencia/Copyright.                                  |
|                       |                     | *Incluye URL de Creative Commons                                           |
|                       |                     | http://creativecommons.org/licenses/by-nc/4.0                              |
+-----------------------+---------------------+----------------------------------------------------------------------------+

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

	- Se recomienda específicamente crear los nuevos atributos/especificadores de campo de **licenceCondition** según la codificación propuesta.
	- Se recomienda utilizar conjuntamente una licencia de uso en "texto" para Humanos y una licencia en "URI/URL" para Máquinas.



.. [#] https://co.creativecommons.org/?page_id=672

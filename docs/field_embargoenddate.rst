.. _dci:dateEmbargo:

Date (Fecha asociadas) (M)
==========================

``datacite:date``

Definición y alcance del campo
------------------------------
Este campo contiene un grupo de fechas asociadas a la creación, edición, publicación, embargo y acceso al recurso de información (Fechas asociada al evento durante todo el ciclo de vida del recurso).

..

Normalmente, la fecha estará asociada con la disponibilidad del recurso. La mejor práctica es codificar el valor de la fecha con el perfil que define `ISO 8601 <https://www.iso.org/iso-8601-date-and-time-format.html>`_ [W3CDTF] con formato AAAA-MM-DD.

..

En caso de recursos de información que se encuentren bajo período de embargo,  se deben registrar la fecha de disponibilidad del mismo con el compromiso de proporcionar acceso al documento completo a partir del momento de su liberación  (para productos de información que aplique).


Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio (M) para fechas de publicación.

..

Obligatorio cuando sea aplicable (MA) cuando existan periodos de embargo ó restricciones de acceso.

..

Opcional (O) otro tipo de  fechas cuando se encuentren presentes en el recurso de información.


Niveles de ocurrencia (R / NR)
------------------------------
Para fechas de publicación: No Repetible (R): **1 ocurrencia**

..

Para periodos de embargo: No Repetible (R): **2 ocurrencias** (Fechas de inicio y finalización del embargo)

Esquema de metadatos
--------------------
datacite:date

..

**Nota:** Este campo se ha adaptado del esquema de metadatos DATACITE MetadataKernel versión 4.1 (http://doi.org/10.5438/0014), el cual es utilizado ampliamente para la gestión de documentos y datos.

Traducción al español
---------------------
Fechas Asociadas:

- Fecha de publicación 
- Fecha de Disponibilidad/Acceso
- Fecha de Aceptación

Forma de Descripción Normalizada (RDA / RCAA2/ ISBD)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar la fecha en la forma estipulada:

	- **Fecha de publicación completa:**  Información relacionada con la publicación, impresión, distribución, emisión y puesta en circulación del recurso. Debe ingresarse con las reglas de codificación de la W3C / `ISO 8601 <https://www.iso.org/iso-8601-date-and-time-format.html>`_ para fechas y horas (AAAA-MM-DD) (por ejemplo: 1997-07-16)
	
		**Notas:** 
			- AAAA [año de cuatro dígitos] deber ser  **Obligatorio**.
			- MM [el mes de dos dígitos (01 = enero, 02 = febrero, 03 = marzo, etc.)] es **Opcional**.
			- DD [el día del mes de dos dígitos (01 a 31)] es **Opcional**.

	- **Campo de fecha - Fecha de publicación:** Normalmente, los sistemas de repositorio tienen más de un campo de fecha que sirve para diferentes propósitos. Por ejemplo: Fecha de creación, publicación, modificación, promoción, emisión, etc. Preferiblemente, en la perspectiva de los usuarios finales, la fecha más lógica y significativa será la fecha de publicación (dc.date.issued). **YYYY-MM-DD** (Por ejemplo: 2015-05-15)

	- **Fecha de publicación no disponible o no identificada:** Si no hay una fecha de publicación disponible o identificada, use cualquier otra fecha disponible o una aproximación a la fecha de publicación del recurso según su contenido. No colocar fechas que incluyan signos ó símbolos (Por ejemplo: 200?, 19??). No es adecuado dejar el campo sin ninguna fecha ya que para efectos de recuperación es un campo clave que aproxima la cantidad de recursos por periodos de tiempo. Cabe resaltar que en el caso que no se tenga la fecha exacta, no hay necesidad de colocar el mes ni el día, tan solo con el año el recurso no se verá afectado. YYYY (por ejemplo: 2018)

	- **Adiciones de marca de datos:** En ocasiones, existen fechas difusas o borrosas en los recursos, se recomienda no dejar el campo de fecha de publicación en blanco (acerque el periodo de fecha del recurso en vez de utilizar una periodo cronológico) y en simultaneo utilizar cicho periodo cronológico (Por Ejemplo: “Siglo XX” - “17th century”) para expresar éste periodo temporal en el campo (**dc:coverage**).  

	**Nota:** Dado que no hay un estándar para fechas difusas o no identificadas para periodos cronológicos o términos como "Renacimiento" o "Siglo XVII", simplemente estos resultados no aparecerán en las consultas realizadas en el campo de fecha.


Propiedades, atributos y especificadores de campo
-------------------------------------------------

Clase Principal Fechas (dates) (M, 1): 
++++++++++++++++++++++++++++++++++++++

Entidad que agrupa todas las fechas relacionadas con el recurso durante su ciclo de vida.

	- **Sub-Propiedad: Fecha (date) (M, 1-n):** Entidad que identifica cada uno de las fechas relacionadas con el recurso durante su ciclo de vida.
		  
		- **Atributo: Tipo de Fecha (dateType) (M, 1):**  En el tipo de fecha elija del vocabulario de **tipo de fecha** y utilice el término controlado para indicar el tipo de fecha asociado al recurso según el vocabulario propuesto:

		+-------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
		| Vocabulario Normalizado | Descripción del Atributo                                                                                                                                                                                                                                                                                                                                         | Dominio de Vocabulario |
		+=========================+==================================================================================================================================================================================================================================================================================================================================================================+========================+
		| Accepted                | Fecha en la cual fue aceptado el recurso de información y es incluido en el sistema de información. No confundir con la fecha que fue recibido el recurso. En el ámbito que haya embargo (restricción de acceso), este atributo indica la fecha de inicio de la restricción.                                                                                     | datacite               |
		+-------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
		| Available               | Fecha en la cual está disponible el recurso de información para consulta/acceso público. Generalmente está asociado con la fecha de publicación del recurso en el sistema de información cuando no se haya hecho una publicación previa. En el ámbito que haya embargo (restricción de acceso), este atributo indica la fecha de finalización de la restricción. | datacite               |
		+-------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
		| Copyrighted             | La fecha específica y documentada en la que el recurso recibe un estado con derechos de autor, si corresponde.                                                                                                                                                                                                                                                   | datacite               |
		+-------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
		| Collected               | La fecha o rango de fechas en que se recolectó/cosechó el contenido del recurso. Aplica para recursos de información recolectado/cosechado por agregadores OAI-PMH.                                                                                                                                                                                              | datacite               |
		+-------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
		| Created                 | Fecha de creación o fabricación del contenido intelectual si es diferente de la fecha.de publicación.                                                                                                                                                                                                                                                            | datacite               |
		+-------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
		| Issued                  | Fecha de publicación del recurso de información. Generalmente está asociado con la fecha de disponibilidad del recurso en el sistema de información cuando no se haya hecho una publicación previa del mismo.                                                                                                                                                    | datacite               |
		+-------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
		| Submitted               | Fecha el la cual fue enviado el recurso al sistema de información y es recibido formalmente para inicio de su gestión (Workflow) si aplica.                                                                                                                                                                                                                      | datacite               |
		+-------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
		| Updated                 | La última vez que se actualizó ó modificó el recurso de información a través de cualquiera de las interfaces ofrecidas por el sistema de información                                                                                                                                                                                                             | redcol                 |
		+-------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
		| Valid                   | La fecha o el intervalo de fechas durante el cual el conjunto de datos o el recurso es válido para su uso.                                                                                                                                                                                                                                                       | datacite               |
		+-------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
		| Withdrawn               | La fecha en que se elimina el recurso.                                                                                                                                                                                                                                                                                                                           | datacite               |
		+-------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
		| Other                   | Otro tipo de fechas no especificadas en el vocabulario                                                                                                                                                                                                                                                                                                           | datacite               |
		+-------------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+





Relaciones con otros campos
---------------------------

	- No debe confundirse la fecha de embargo del recurso de información **Embargo Period Date (datacite:date)** con la fecha de publicación del recurso **Publication Date (dc.date.issued)** incluidos sus especificadores de campo.
	- No debe confundirse la fecha de creación del recurso (**dc.date.created**) con la fecha de publicación del mismo **Publication Date (dc.date.issued)**.
	- No debe confundirse la fecha de disponibilidad del recurso en accceso completo (Full-Text Access  **dc.date.available**) en el repositorio con la fecha de publicación del mismo **Publication Date (dc.date.issued)**.


Restricciones
-------------

	- Si no hay ninguna fecha de publicación disponible, se recomienda utilizar una fecha estimada. Dado que es mejor utilizar una fecha estimada que ninguna, se pueden utilizar la fecha de impresión, la de aceptación del trabajo, la fecha en que se coloca disponible el recurso para descarga/consulta, etc.
	- En el ámbito que haya embargo (restricción de acceso), se recomienda especificar las dos fechas (**Accepted, Available**) con sus respectivos atributos que indican inicio y fin de la restricción.
	- Cuando el campo asociado a los derechos de acceso (M) se establezca con el valor provisto por COAR **embargoed access** / <http://purl.org/coar/access_right/c_f1cf>. Es obligatorio la inclusión de la fecha de inicio y finalización del período de embargo.


Ejemplos y ayudas
-----------------

Ayudas
++++++

	- **Fecha de publicación:**   datacite:date  dataType= “Issued”     - 2019-03-20
	- **Fecha de aceptación:**     datacite:date  dataType=“Accepted”   - 2019-02-01
	- **Fecha de disponibilidad:** datacite:date  dataType=“Available”  - 2010-04-25
	- **Fecha de creación:**       datacite:date  dataType=“Created”    - 1977-07-11

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   	<dc:date>2017-02-10T22:11:00Z</dc:date>
   	<dc:date>2017-02-10T22:11:00Z</dc:date>
   	<dc:date>2017</dc:date>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   	<datacite:dates>
  		<datacite:date dateType="Accepted">2011-12-01</datacite:date>
  		<datacite:date dateType="Available">2012-12-01</datacite:date>
  		<datacite:date dateType="Issued">2010-12-25</datacite:date>
	</datacite:dates>


**Esquema xoai**

.. code-block:: xml
   :linenos:

   	<element name="date">
		<element name="accessioned">
			<element name="none">
				<field name="value">2017-02-10T22:11:00Z</field>
			</element>
		</element>
		<element name="available">
			<element name="none">
				<field name="value">2017-02-10T22:11:00Z</field>
			</element>
		</element>
		<element name="issued">
			<element name="none">
				<field name="value">2017</field>
			</element>
		</element>
	</element>

**Esquema dim**

.. code-block:: xml
   :linenos:

    <dim:field mdschema="dc" element="date" qualifier="accessioned">2017-02-10T22:11:00Z</dim:field>
	<dim:field mdschema="dc" element="date" qualifier="available">2017-02-10T22:11:00Z</dim:field>
	<dim:field mdschema="dc" element="date" qualifier="issued">2017</dim:field>

Niveles de aplicación para  productos de investigación de MinCiencias
---------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias.

Relaciones con otros modelos de metadatos
-----------------------------------------
El campo Fecha de publicación **(datacite:date)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

..

+----------------------+------------------------------------------------+
| Esquema de Metadatos | Campo Relacionado                              |
+======================+================================================+
| dc                   | * dc.date                                      |
|                      | * dc.date.issued                               |
+----------------------+------------------------------------------------+
| dcterms              | dcterms.date                                   |
+----------------------+------------------------------------------------+
| lom                  | lom.meta-metadatos.date                        |
+----------------------+------------------------------------------------+
| marcxml              | field:008 (00-05,06,07-10,11-14) 046, 260, 264 |
+----------------------+------------------------------------------------+

..


Niveles semánticos
------------------

No aplica.

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores | Nota de alcance                                                                                 |
+========================================+=======================+===============+=================================================================================================+
| Fecha de publicación                   | dc.date               | issued        |                                                                                                 |
+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------------+
| Fecha de disponibilidad                | dc.date               | available     | Utilice este campo para registrar la fecha de finalización de embargo                           |
+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------------+
| Fecha de aceptación                    | dc.date               | accepted      | Para indicar el inicio de un período de embargo, utilice Enviado o Aceptado, según corresponda. |
+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------------+
| Fecha de envío                         | dc.date               | submitted     |                                                                                                 |
+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------------+
| Fecha de creación                      | dc.date               | created       |                                                                                                 |
+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------------+
| Fecha de Recolección                   | dc.date               | collected     |                                                                                                 |
+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------------+
| Fecha de actualización                 | dc.date               | updated       |                                                                                                 |
+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------------+
| Fecha de validez                       | dc.date               | valid         |                                                                                                 |
+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------------+
| Fecha de descarte                      | dc.date               | withdrawn     |                                                                                                 |
+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------------+
| Otras fechas relacionadas              | dc.date               | other         |                                                                                                 |
+----------------------------------------+-----------------------+---------------+-------------------------------------------------------------------------------------------------+


Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

- Se recomienda específicamente crear los nuevos atributos/especificadores del campo de fecha según la codificación propuesta.

- En versiones previas de otras directrices se utilizaba es esquema info:eu-repo/date/EmbargoEnd/[YYYY-MM-DD] el cual debe ser sustituido por el uso de las nuevas propiedades y atributos.

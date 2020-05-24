.. _dc.language:

Language (Idioma) (MA)
======================

``dc:language``

Definición y alcance del campo
------------------------------
Lenguaje del contenido del recurso de investigación, caracterizado por un código normalizado de tres caracteres.  

Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio si aplica (MA)

Niveles de ocurrencia (R / NR)
------------------------------------------------
Repetible (R): **0-n veces**.

- Repita este campo utilizando otros códigos de idioma según se considere.


Esquema de metadatos
------------------------------
dc:language

- **Nota:** Este campo se ha adaptado del esquema de metadatos DUBLIN CORE (http://dublincore.org/schemas/), e introducido de DRIVER Guidelines - elementos del idioma versión 2.


Traducción al español
---------------------
Idioma

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar los códigos referentes al idioma. Existen múltiples vocabularios para normalizar los idiomas como se muestra a continuación:

+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+
| ETF BCP 47                                                                                    | Registro de subetiquetas de idioma de IANA. Ver en: https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry |
+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+
| ISO 639-x, donde x puede ser 1,2 o 3. Mejor práctica: usamos ISO 639-3 y al hacerlo seguimos: | http://www.sil.org/iso639-3/                                                                                                           |
+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+
| Códigos MARC para idioma                                                                      | https://www.loc.gov/marc/languages/language_code.html#s                                                                                |
+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+

**NOTA:** 

	- Para el caso de este conjunto de directrices, se recomienda utilizar específicamente el vocabulario propuesto por la norma ISO 639-3


Propiedades, atributos y especificadores de campo
-------------------------------------------------

	- **Propiedad Principal Idioma (language) (MA, 0-n):** Entidad que identifica cada uno de los idiomas relacionadas con el recurso durante su ciclo de vida. Utilice el término controlado para indicar el tipo de fecha asociado al recurso según el vocabulario propuesto (Norma ISO 639-3 [#]_):

Relaciones con otros campos
---------------------------

	- No confundir el uso del campo Idioma, con el campo País/Lugar geográfico que se utiliza en el campo “dc.coverage”.
	- No confundir el campo Idioma (dc.language) con los atributos de Idioma (xml:lang) utilizados por otros campos de metadatos. Sin embargo se recomienda que éstos últimos también se encuentren codificados con el mismo vocabulario ISO 639-3. 

Restricciones
-------------
No aplica


Ejemplos y ayudas
------------------

Ayudas 
++++++

- Idiomas

	+--------+------------+
	| Código | Idioma     |
	+========+============+
	| spa    | Spanish    |
	+--------+------------+
	| eng    | English    |
	+--------+------------+
	| por    | portuguese |
	+--------+------------+
	| fre    | french     |
	+--------+------------+
	| ger    | Germanic   |
	+--------+------------+

Ejemplo en XML  (Interoperabilidad OAI-PMH)
+++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc:language>eng</dc:language>
   <dc:language>spa</dc:language>
   <dc:language>ita</dc:language>
   <dc:language>nld/dut</dc:language>
   <dc:language>dut</dc:language>
   <dc:language>nl</dc:language>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <dc:language>spa</dc:language>


**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="language">
    	<element name="iso">
          <element name="spa">
             <field name="value">spa</field>
          </element>
     	</element>
   </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema="dc" element="language" qualifier="iso" lang="spa">spa</dim:field>

Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------
El campo **idioma (dc.lenguaje)** es utilizado por los siguientes esquemas:

+----------------------+-------------------+
| Esquema de Metadatos | Campo Relacionado |
+======================+===================+
| marcxml              | field:041         |
+----------------------+-------------------+


Niveles semánticos
------------------
No aplica

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

+----------------------------------------+-----------------------+---------------+-----------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores | Nota de alcance |
+========================================+=======================+===============+=================+
| Idioma                                 | dc.language           | iso           | Norma ISO 639-3 |
+----------------------------------------+-----------------------+---------------+-----------------+

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------
No aplica
 
.. [#] https://iso639-3.sil.org/sites/iso639-3/files/downloads/iso-639-3.tab

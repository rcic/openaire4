.. _dc.language:

Language (Idioma) (MA)
======================

``dc.language``

Definición y alcance del campo
------------------------------
Lenguaje del contenido del recurso de investigación, caracterizado por un código normalizado de tres caracteres.  

Niveles de persistencia (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR)
------------------------------------------------
Repetible (R): **1-n veces**.

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

Revise la forma adecuada para ingresar los códigos referentes al idioma. Tome los valores de una de las siguientes listas:

+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+
| ETF BCP 47                                                                                    | Registro de subetiquetas de idioma de IANA. Ver en: https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry |
+===============================================================================================+========================================================================================================================================+
| ISO 639-x, donde x puede ser 1,2 o 3. Mejor práctica: usamos ISO 639-3 y al hacerlo seguimos: | http://www.sil.org/iso639-3/                                                                                                           |
+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+
| Códigos MARC para idioma                                                                      | https://www.loc.gov/marc/languages/language_code.html#s                                                                                |
+-----------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------+


Propiedades, atributos y especificadores de campo
-------------------------------------------------
No aplica

Relaciones con otros campos
---------------------------
No aplica

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

   <dc.language>eng</dc.language>
   <dc.language>spa</dc.language>
   <dc.language>ita</dc.language>
   <dc.language>nld/dut</dc.language>
   <dc.language>dut</dc.language>
   <dc.language>nl</dc.language>

**Esquema DataCite**

.. code-block:: xml
   :linenos:


**Esquema xoai**

.. code-block:: xml
   :linenos:

**Esquema dim**

.. code-block:: xml
   :linenos:

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

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
No aplica

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------
No aplica
 

.. _dc.language:

Idioma (MA)
============

``dc.language``

Definición y alcance del campo
------------------------------
Lenguaje del contenido del recurso de investigación. 

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
No repetible (NR)

Campo con esquema de metadatos
------------------------------
dc:language 

Traducción al español
---------------------
Idioma

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Revise la forma adecuada para ingresar los códigos referentes al idioma:

=====  ============
spa    Spanish     
eng    English     
por    portuguese  
fre    french      
ger    Germanic    
=====  ============

Consulte más códigos de idioma en la siguiente lista: https://www.loc.gov/marc/languages/language_code.html#s


Valores permitidos (Vocabularios Controlados)
---------------------------------------------
IETF BCP 47, ISO 639-3

Relaciones con otros campos
---------------------------

Restricciones
-------------


Ejemplos
--------

.. code-block:: xml
   :linenos:


   <dc.language>eng</dc.language>
   <dc.language>spa</dc.language>
   <dc.language>ita</dc.language>
   <dc.language>nld/dut</dc.language>
   <dc.language>dut</dc.language>
   <dc.language>nl</dc.language>

.. _DRIVER Guidelines v2 element language: https://wiki.surfnet.nl/display/DRIVERguidelines/Language

Atributos de campo
------------------
IETF BCP 47, ISO 639-3

Especificadores de campo
------------------------

Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear en Dspace los siguientes campos:

- dc:language

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------
OpenAIRE 3: dc.language 

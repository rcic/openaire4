.. _dci:identifier:

Resource Identifier (Identificador primario) (M)
================================================

``datacite:identifier``

Definición y alcance del campo
------------------------------
Identificador Primario. Este campo contiene una cadena de texto que referencia de manera inequívoca al recurso dentro de un contexto determinado. También hace referencia el número de identificación del proyecto ante los entes financiadores.

La mejor práctica recomendada es identificar el recurso por medio de una cadena o número que se ajuste a un sistema de identificación formal y normalizado. Los sistemas de identificación formales incluyen:


- El identificador uniforme de recursos (URI)
- El localizador uniforme de recursos (URL)
- El identificador digital de objetos (DOI)
- El nombre de recurso uniforme provisto por las Bibliotecas Nacionales (URN:NBN)
- El Identificador ARK
- También puede ser una URL directa o una URL de redirección, como PURL, HANDLE u otros mecanismos de resolución internacional.

**Notas:**

- La resolución del identificador utilizado debe permitir dirigirse de manera unívoca al registro digital o una página de salto intermediaria que al final conlleve al registro.
- Este identificador no debe conducir al documento de texto completo asociado al registro.
- Se recomienda utilizar direcciones URL estables y persistentes.
- No confundir con Identificador alternativo (R), Identificador relacionado (R), Ubicación del archivo (MA) y Fuente (R).



Niveles de persistencia (M/MA/R/O)
----------------------------------
Obligatorio (M)

Niveles de ocurrencia (R / NR)
------------------------------
No repetible (NR).

- Campo único de **uso obligatorio**

Esquema de metadatos
--------------------
datacite:identifier

- **Nota:** Este campo se ha adaptado del esquema de metadatos DATACITE MetadataKernel versión 4.1 (http://doi.org/10.5438/0014), el cual es utilizado ampliamente para la gestión de documentos y datos. 

Traducción al español
---------------------
Identificador digital del recurso

Forma de Descripción Normalizada (RDA / RCAA2/ ISBD)
----------------------------------------------------
RDA (Recursos: descripción y acceso): Revise la forma adecuada para ingresar el identificador del recurso:

**datacite:identifier:** Ingrese alguno de los siguientes identificadores normalizados:
   - ARK
   - URI
   - URL
   - URN:NBN
   - DOI
   - PURL
   - HANDLE


Propiedades, atributos y especificadores de campo
-------------------------------------------------

- **Propiedad del Identificador Primario  (Identifier) (M, 1):** Esta propiedad permite especificar el valor del identificador que se le ha otorgado al recurso.

   - **Atributo: Tipo de identificador alternativo (identifierType) (M,1):** Este atributo permite especificar el tipo de identificador que se le ha otorgado al recurso. Se debe tener en cuenta los siguientes tipos de identificadores y su codificación normalizada según el vocabulario controlado propuesto:
   
     +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
     | Vocabulario Normalizado | Descripción del Atributo                                                                                                                                                               | Dominio de Vocabulario |
     +=========================+========================================================================================================================================================================================+========================+
     | ARK                     | Clave de recursos de archivo; URI diseñada para soportar el acceso a largo plazo a objetos de información.                                                                             | datacite               |
     +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
     | DOI                     | Identificador de Objeto Digital. Código alfanumérico que sirva para identificar de forma única un documento digital.                                                                   | datacite               |
     +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
     | HANDLE                  | Es un identificador persistente, es decir, un sistema de especificación para nombres e identificación de servicios.                                                                    | datacite               |
     +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
     | PURL                    | Localizador de recursos uniforme y persistente, se utiliza para referenciar un determinado recurso que cambia de dirección a lo largo del tiempo desde una misma dirección.            | datacite               |
     +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
     | URI                     | Identificador uniforme de recursos                                                                                                                                                     | datacite               |
     +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
     | URL                     | Localizador Uniforme de Recursos, es la dirección específica que se le asigna a cada uno de los recursos disponibles en la red con el fin de localizarlos e identificarlos fácilmente. | datacite               |
     +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
     | URN                     | Nombre del recurso uniforme, permite identificar recursos en la web pero no indica exactamente dónde se encuentra el recurso.                                                          | datacite               |
     +-------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------------+
     



Relaciones con otros campos
---------------------------

- No debe confundirse el Identificador Primario **(datacite:Identifier)** del recurso con el  identificador relacionado **(datacite:relatedIdentifier)** del mismo.
- No debe confundirse el Identificador Primario **(datacite:Identifier)** del recurso con el  identificador Alternativo **(datacite:alternateIdentifier)** del mismo.
- No debe confundirse el Identificador Primario **(datacite:Identifier)** del recurso con el  campo **dc.relation** que permite **relacionar una versión del recurso con otra.**
- No debe confundirse el Identificador Primario **(datacite:Identifier)** del recurso con el  campo **dc.identifier.citation** que permite almacenar la cita única del recurso en un formato de citación específico.
- No debe confundirse el Identificador Primario **(datacite:Identifier)** del recurso con el  campo **dc.identifier.bibliographicCitation (dcterms.bibliographicCitation)** que en DSPACE es utilizado como (dc.identifier.citation) y que contiene la cita bibliográfica que permite identificar el recurso de origen.

Restricciones
-------------

- Campo de metadatos de uso único.
- Debe utilizarse Identificadores que permitan dirigirse (uso de sistemas de resolución) de manera unívoca al registro digital o una página de salto intermediaria que al final conlleve al registro.
- No debe ser utilizado para almacenar identificadores que no permitan hacer una correcta resolución.
- No utilizar este campo para almacenar estos tipos de identificadores (que no permiten sistema de resolución univoco): ISBN, ISSN, E-ISSN,  PMID, UPC, Signaturas Topográficas, Identificadores locales, etc.


Ejemplos y ayudas
-----------------

Ayudas
++++++

- **Identificador Primario:** Identificador del recurso, puede ser una cadena alfanumérica que sea única dentro de su dominio o emisión. 

      - Ej (URL): https://repositorio.uptc.edu.co/handle/001/1698
      - Ej (DOI): https://doi.org/10.1002/anie.201601750 
      - Ej (Handle): http://hdl.handle.net/10272/16239 
      - Ej (PURL): https://purl.org/metabiblioteca/home 
      - Ej (URN): urn:nbn:nl:ui:13-123456789

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

      <dc:identifier>http://hdl.handle.net/10272/16239</dc:identifier>
      <dc:identifier>10.1002/anie.201601750</dc:identifier>

**Esquema DataCite**

.. code-block:: xml
   :linenos:

   <datacite:identifier identifierType="Handle">http://hdl.handle.net/1234/5628</datacite:identifier>

   <datacite:identifier identifierType="HANDLE">http://hdl.handle.net/10272/16239</datacite:identifier>

**Esquema xoai**

.. code-block:: xml
   :linenos:

      <element name="identifier">
      <element name="handle">
         <element name="none">
         <field name="value">http://hdl.handle.net/10272/16239</field>
         </element>
      </element>
      </element>

.. code-block:: xml
   :linenos:

      <element name="identifier">
      <element name="doi">
      <element name="none">
         <field name="value">10.1002/anie.201601750</field>
      </element>
      </element>
      </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

      <dim:field mdschema="dc" element="identifier" qualifier="uri">http://hdl.handle.net/10272/16239</dim:field>
      <dim:field mdschema="dc" element="identifier" qualifier="doi">10.1002/anie.201601750</dim:field>


Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------
El campo Identificador Primario **(datacite:Identifier)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+---------------------------+
| Esquema de Metadatos | Campo Relacionado         |
+======================+===========================+
| dc                   | * dc.identifier.doi       |
|                      | * dc.identifier.uri       |
|                      | * dc.identifier.url       |
+----------------------+---------------------------+
| dcterms              | * dcterms.identifier.doi  |
|                      | * dcterms.identifier.uri  |
|                      | * dcterms.identifier.url  |
+----------------------+---------------------------+
| marcxml              | field: 024, 856           |
+----------------------+---------------------------+

Niveles semánticos
------------------

- Este campo contempla la utilización de distintos identificadores internacionales estandarizados para la identificación de un recurso.
- Cada registro presente en estos identificadores  internacionales estandarizados es un identificador persistente.


Recomendación de campos de aplicación en DSPACE
-----------------------------------------------

Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas DSPACE basados en los siguientes elementos:

+----------------------------------------+-----------------------+---------------+-----------------+
| Vocabulario controlado OpenAire/RedCol | Campo Elemento DSPACE | Calificadores | Nota de alcance |
+========================================+=======================+===============+=================+
| Identificador Principal                | dc.identifier         | * doi         |                 |
|                                        |                       | * local       |                 |
|                                        |                       | * isbn        |                 |
|                                        |                       | * issn        |                 |
|                                        |                       | * uri         |                 |
|                                        |                       | * url         |                 |
|                                        |                       | * other       |                 |
+----------------------------------------+-----------------------+---------------+-----------------+

**Nota:**

- Cuando es utilizado el esquema de metadatos dublin core (dc), el identificador Primario será siempre la primera ocurrencia del campo dc.identifier.


Recomendaciones de migración de otras directrices de metadatos (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------------------

Se recomienda específicamente crear los nuevos atributos/especificadores del campo de identificador alternativo según la codificación propuesta.

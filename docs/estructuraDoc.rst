.. _estructuraDoc:

Estructura del Perfil de Aplicación (Campos de Metadatos)
=========================================================

El documento proporciona una descripción general de cómo configurar y utilizar el protocolo OAI-PMH para la recolección de metadatos. Los campo mínimos a trabajar en el perfil de aplicación son los siguientes: 


- **Definición y alcance del campo:** Se exponen con precisión los conceptos de los campo y se determina de forma clara y sencilla los objetivos que se quieren alcanzar en cada uno.

..

- **Niveles de requerimientos:** Son las propiedades de los metadatos definidas así:

..

  - **Obligatorio = Mandatory (M)**
    La propiedad siempre debe estar presente en los metadatos. No se permite un valor vacío para la propiedad.

..

  - **Obligatorio si es aplicable = Mandatory if Applicable (MA)**
    Cuando se puede obtener el valor de la propiedad, debe estar presente en los metadatos.

..

  - **Recomendado = Recommended (R)**
    Se recomienda el uso de la propiedad.

..

  - **Opcional = Optional (O)**
    No es importante si la propiedad se usa o no, pero si se usa puede proporcionar información complementaria sobre el recurso.

..

- **Niveles de ocurrencia:** Se especifica la repetibilidad o  no repetibilidad de cada campo según su naturaleza.

..

    - **Repetible (R)**
    - **No repetible (NR)**

..

- **Esquema de metadatos:** Determina el modelo de metadatos aplicado para la definición y utilización del campo. Estas directrices contemplan la utilización de los siguientes modelos de metadatos:

..

+-------------------------------------------------------------+---------------------+
| Modelo de Metadatos                                         | Codificación REDCOL |
+=============================================================+=====================+
| Simple DC XML Schema                                        | dc                  |
+-------------------------------------------------------------+---------------------+
| DCMI Metadata Terms Schema                                  | dcterms             |
+-------------------------------------------------------------+---------------------+
| Learning Object Metadata Schema definition (LOM)            | lom                 |
+-------------------------------------------------------------+---------------------+
| Electronic Theses and Dissertation Metadata Schema (ETD-MS) | thesis              |
+-------------------------------------------------------------+---------------------+
| DataCite Metadata Schema                                    | datacite            |
+-------------------------------------------------------------+---------------------+
| OpenAire Specification Schema                               | oaire               |
+-------------------------------------------------------------+---------------------+

..

- **Campo con esquema de metadatos:** Se detalla la estructura del campo del metadato para la descripción del recurso. 

..

- **Traducción al español:** Nombre del campo de metadato en idioma español. 

..

- **Forma de descripción normalizada:** Aquí se indica la forma correcta de la descripción del campo según la normatividad internacional aplicada. Ejemplo: RDA (Recursos : descripción y acceso) - RCAA2 (Reglas de Catalogación Angloamericanas 2).

..

- **Valores permitidos:** En los campos temáticos se deben utilizar vocabularios controlados y/o términos extraídos de tesauros.  

..

- **Relaciones con otros campos:** Aquí deben colocarse los campos a los cuales hace relación. Ejemplo: título, campos relacionados, subtítulo, título alternativo, otro título. 

..

- **Restricciones:** Información que no debe utilizarse en el campo.

..

- **Ejemplos:** Se describe la forma correcta para la descripción del campo. 

..

- **Atributos de campo:** Son los elementos que debe incluir el campo para su descripción. Ejemplo: atributos de idioma, formato, etc. 

..

- **Especificadores de campo:** Hace referencia a la sintaxis que debe tener el campo.

..

- **Niveles de aplicación para productos de investigación de Colciencias:** Se especifica a que producto de Colciencias se le aplica el campo. 

..

- **Relaciones con otros modelos de metadatos:** Se relacionan otros modelos y esquemas de metadatos que apliquen. 

..

- **Niveles semánticos:** Permiten asignar significado a la información sobre los atributos que se apliquen al campo. 

..

- **Recomendación de campos de aplicación en DSPACE:** como se describe un campo específico en el repositorio Dspace. 

..

- **Recomendaciones de migración de Modelos anteriores:** Información que se debe tener en cuenta al momento de migrar modelos y esquemas de metadatos anteriores como: BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2.0, OPENAIRE 3.0.


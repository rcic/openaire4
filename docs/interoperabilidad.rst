.. _interoperabilidad:

Interoperabilidad
=================

Un componente vital que debe ser tenido en cuenta en todas las las políticas y/o directrices de gestión de los proyectos institucionales de **Sistemas de información de investigación, Repositorios institucionales , Bibliotecas Digitales, y Sistemas de publicación monográficos/seriados es el componente de Interoperabilidad del sistema de información**, entendiendo esta como “La capacidad de un sistema de información para comunicarse y compartir datos, información, documentos y objetos digitales de forma efectiva, con uno o varios sistemas de información (siendo generalmente estos sistemas completamente heterogéneos, distribuidos y geográficamente distantes), mediante una interconexión libre, automática y transparente, sin dejar de utilizar en ningún momento la interfaz del sistema propio”(Gómez-Dueñas, 2009). De esta forma, aunque los sistemas de información sean totalmente funcionales en  el ámbito de aplicación y uso de los usuarios (Interfaces de Usuario). Para muchos proyectos, no es claro cómo estos sistemas de información se pueden articular con otros sistemas y redes de información y participar en la creación de productos y servicios distribuidos.

Hay tres elementos claves que se deben tener en cuenta como parte importante del componente de interoperabilidad en estos sistemas de Información y que actualmente presentan algunos problemas que se detallan a continuación:

	- **La estructura de los metadatos utilizados (Interoperabilidad Sintáctica):** Respecto a la estructura de los metadatos, aunque actualmente existe un consenso generalizado en la utilización del estándar Dublin Core para recursos de información Monográficos/Seriadas y el estándar LOM para Objetos de Aprendizaje (Llamados en Colombia REDA), en la práctica se evidencia que cada institución ha modificado y configurado sus distintos sistemas de información creando campos de metadatos adaptados a sus recursos de información propios y que no necesariamente están ajustados a algún estándar. Por ejemplo para almacenar la tipología documental asociada, se ha encontrado gran disparidad de campos entre los que se encuentran: “dc.type”, “dc.type.local”, “dc.type.tipologia”, “dc.type.tipolocal”, etc.  El problema de no tener claridad en la correcta gestión de estos campos “propios” se traduce básicamente en la pérdida total o parcial de estos datos al ser integrados/recolectados/cosechados por otros sistemas intermediarios y/o agregadores.  

	..

	- **La forma y valores de los contenidos (Interoperabilidad Semántica):** Respecto a la forma y valores de los contenidos presentes en los metadatos utilizados, se evidencia que el aseguramiento de la calidad en los metadatos sigue siendo un gran desafío para las instituciones que gestionan los distintos sistemas de información (Repositorios Institucionales / Bibliotecas Digitales / Portales de Revistas), esto apoyado en muchos resultados de las investigaciones presentadas para determinar el estado y calidad de los Metadatos en Colombia entre los que se destacan (Tabares Morales, 2013) y (Ruíz Jaramillo, 2015), que indican como parte de sus conclusiones que “se presenta algunos problemas de calidad de metadatos de los OAs, principalmente respecto a la completitud y coherencia de los mismos”. Dicho de otro modo, falta mejorar y normalizar aún  más los contenidos presentes en los esquemas de metadatos. Se debe tener en cuenta que para este punto, existen múltiples manuales y guías que se han publicado y presentado para normalizar metadatos como la Guía de Metadatos del Proyecto Biblioteca Digital Colombiana,  El Manual de Metadatos e Interoperabilidad del Sistema Nacional de Acceso Abierto al Conocimiento – SNAAC, la guía de Metadatos y políticas de cosecha de la Red Latinoamericana de Repositorios y Biblioteca Digitales - LAReferencia y las Directrices DRIVER 2.0 - Directrices para proveedores de contenido que han evolucionado a las Directrices OpenAIRE para gestión de repositorios documentales V3/4. Adicionalmente, la Confederation of Open Access Repositories COAR generó un conjunto de vocabularios semánticos que serán utilizados en el desarrollo de estas directrices.
	
	..

	- **Los protocolos para compartir los metadatos (y Contenidos) (Interoperabilidad Estructural):** Respecto a los protocolos para compartir los metadatos, básicamente todos los sistemas de información poseen interfaces nativas que están íntimamente ligados al uso del protocolo OAI-PMH v2 (Un  protocolo de intercambio de datos sobre el protocolo HTTP que tiene su origen en la ciudad de Nuevo México en el año de 1999 y cuya primera versión se hizo pública en enero de 2001). Sin embargo, pese a cumplir más de veinte años aún no se ha explotado todo su potencial de intercambio sobre formatos de metadatos siendo generalmente utilizado asociado al formato de metadatos más simple de todos (oai_dc), el cual solo permite compartir los quince (15) campos básicos asociados al estándar dublin core. Por fortuna, los principales sistemas de información para Repositorio y Bibliotecas Digitales (DSPACE, EPRINTS,  OJC, OMP, etc.), tienen incorporados múltiples formatos de intercambio de metadatos en su protocolo OAI-PMH brindando una mayor flexibilidad para evaluar el estado y calidad de los metadatos. Adicionalmente, se debe tener en cuenta que en los últimos años han surgido nuevos protocolos y componentes que pueden perfectamente reemplazar el uso del protocolo OAI-PMH, entre ellos tenemos ResourceSync y REST-FULL.  


.. toctree::
   :numbered:
   :maxdepth: 1
   :hidden:

   formatoMeta
   contMeta
   compAgre
   estructuraDoc


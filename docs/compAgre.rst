.. _compAgre:

Compatibilidad con otros recolectores de metadatos
==================================================

La Red Colombiana de Información Científica (RedCol) recolectará los metadatos de los distintos sistemas de información que posean las instituciones miembro (Repositorios / Bibliotecas Digitales, Sistema de Publicación, Sistemas de Investigación) que cumplan las directrices propuestas y provean los protocolos de interoperabilidad requeridos (OAI-PMH).

Adicionalmente, las instituciones miembro podrán optar por suministrar únicamente los datos de acceso de un sistema del tipo Integrador/Recolector/Agregador institucional que también sea compatible con estas directrices. Para este caso, es importante conocer la procedencia de los proveedores de contenido original que serán recolectados por los el sistema de información y que deben ser codificados por RedCol, siguiendo las `políticas <http://www.openarchives.org/OAI/2.0/guidelines-provenance.htm>`_ de OAI-PMH para la interoperabilidad (Utilizando el campo **“provenance”** en los metadatos recolectados).

NOTA: No confundir el campo dc.description.provenance que viene incluido dentro del registro de metadatos con el campo OAI:provenance que se indica como un complemente del campo **“record”,** el cual es independiente el modelo de metadatos utilizado durante la cosecha a través el protocolo OAI-PMH  del repositorio/biblioteca digital.

A continuación, se muestra un ejemplo de las etiquetas XML que deben venir acompañando a cada registro de metadatos que se recolecta a través de un sistema intermediario para su codificación:


.. code-block:: xml
   :linenos:

   <record>
   <header> … </header>
   <metadata> … </metadata>

   <about>
   <provenance xmlns="http://www.openarchives.org/OAI/2.0/provenance"
   xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
   xsi:schemaLocation="http://www.openarchives.org/OAI/2.0/provenance
   http://www.openarchives.org/OAI/2.0/provenance.xsd">
     <originDescription altered="true" harvestDate="2012-09-17T14:58:36Z">
       <baseURL>https://repositorio.MinCiencias.gov.co/oai/request</baseURL>
       <identifier>oai:repositorio.MinCiencias.gov.co:1874/218065</identifier>
       <datestamp>2012-01-19T12:38:56Z</datestamp>
       <metadataNamespace>
         http://www.openarchives.org/OAI/2.0/oai_dc/
       </metadataNamespace>
     </originDescription>
   </provenance>
   </about>
   </record>


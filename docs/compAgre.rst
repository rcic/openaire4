.. _compAgre:

Compatibilidad de los agregadores
=================================

Además de los repositorios institucionales y de investigación, están los agregadores que también pueden ser compatibles con estas directrices. Para este caso, es importante conocer la procedencia de los proveedores de contenido original que serán recolectados por los agregadores y que deben ser codificados por OpenAIRE, siguiendo las políticas de OAI-PMH para la interoperabilidad. A continuación, se muestra un ejemplo para su codificación:

.. code-block:: xml
   :linenos:

    <about>
      <provenance xmlns="http://www.openarchives.org/OAI/2.0/provenance"
      xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xsi:schemaLocation="http://www.openarchives.org/OAI/2.0/provenance
      http://www.openarchives.org/OAI/2.0/provenance.xsd">
        <originDescription altered="true" harvestDate="2012-09-17T14:58:36Z">
          <baseURL>http://dspace.library.uu.nl:8080/dspace-oai/request</baseURL>
          <identifier>oai:dspace.library.uu.nl:1874/218065</identifier>
          <datestamp>2012-01-19T12:38:56Z</datestamp>
          <metadataNamespace>
            http://www.openarchives.org/OAI/2.0/oai_dc/
          </metadataNamespace>
        </originDescription>
      </provenance>
    </about>
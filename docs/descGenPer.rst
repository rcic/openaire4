.. _descGenPer:

Perfil de Aplicación de los metadatos 
======================================

El perfil de aplicación es una descripción detallada de los campos de metadatos recomendados para su implementación en repositorios institucionales de investigación. Para el caso de este conjunto de directrices se han creado los siguientes campos de elementos con su correspondiente descripción detallada:

.. tabularcolumns:: |\Y{0.3}|\Y{0.4}|\Y{0.3}|

========================================== =================================== ========================================================================================
Campo-OpenAIRE                             Elemento Metadata                   Refinamiento por vocabulario
========================================== =================================== ========================================================================================
:ref:`dci:title`                           datacite:title                      * Idioma: `ISO 639-3`_
                                                                               * Tipo de Título: :ref:`title type <vocab:titletype_titletype>`
:ref:`dci:creator`                         datacite:creator                     * Tipo de Autor: :ref:`name type <vocab:nametype_nametype>`
                                                                                * Tipo de Identificador: nameIdentifierScheme  
                                                                                * Esquema de Identificador: schemeURI  
:ref:`dci:contributor`                     datacite:contributor                * Tipo de Colaborador: :ref:`name type <vocab:nametype_nametype>`
                                                                               * Tipo de Identificador: nameIdentifierScheme  
                                                                               * Esquema de Identificador: schemeURI               
:ref:`aire:fundingReference`               oaire:fundingReference              :ref:`funderIdentifier type <vocab:funderIdentifiertype_identifiertype>`
:ref:`dci:alternativeIdentifier`           datacite:alternateIdentifier        :ref:`alternateIdentifier type <vocab:alternateIdentifiertype_identifiertype>`
:ref:`dci:relatedIdentifier`               datacite:relatedIdentifier          | :ref:`relatedIdentifier type <vocab:relatedIdentifiertype_identifiertype>`
                                                                               | :ref:`relation type <vocab:relationtype_relationtype>`
                                                                               | :ref:`resourcetype general <vocab:resourcetypegeneral_resourcetypegeneral>`
:ref:`dci:dateEmbargo`                     datacite:date                       :ref:`date type <vocab:datetype_datetype>`
:ref:`dc.language`                         dc.language                         `IETF BCP 47`_, `ISO 639-3`_
:ref:`dc.publisher`                        dc.publisher
:ref:`aire:resourceType`                   oaire:resourceType                  `COAR Resource Type Vocabulary`_
:ref:`aire:version`                        oaire:version                       `COAR Version Vocabulary`_
:ref:`dc.description`                      dc.description
:ref:`dc.format`                           dc.format                           :ref:`format type <vocab:formattype_formattype>`
:ref:`dci:identifier`                      datacite:identifier                 :ref:`identifier type <vocab:identifiertype_identifiertype>`
:ref:`dci:accessrights`                    datacite:rights                     `COAR Access Right Vocabulary`_
:ref:`dc.source`                           dc:source
:ref:`dci:subject`                         datacite:subject              
:ref:`aire:licenseCondition`               oaire:licenseCondition
:ref:`dc.coverage`                         dc.coverage
:ref:`dci:size`                            datacite:size
:ref:`dci:geolocation`                     datacite:geoLocation
:ref:`aire:file`                           oaire:file                          `COAR Access Right Vocabulary`_
:ref:`aire:citationTitle`                  oaire:citationTitle 	
:ref:`aire:citationVolume`                 oaire:citationVolume
:ref:`aire:citationIssue`                  oaire:citationIssue
:ref:`aire:citationStartPage`              oaire:citationStartPage
:ref:`aire:citationEndPage`                oaire:citationEndPage
:ref:`aire:citationEdition`                oaire:citationEdition

:ref:`aire:citationConferencePlace`        oaire:citationConferencePlace
:ref:`aire:citationConferenceDate`         oaire:citationConferenceDate
:ref:`dct:audience`                        dcterms:audience                     :ref:`audience type <vocab:audiencetype_audiencetype>`
:ref:`thesis.degree`                       * thesis.degree.name
                                           * thesis.degree.level
                                           * thesis.degree.discipline
                                           * thesis.degree.grantor
========================================== =================================== ========================================================================================


.. _COAR Resource Type Vocabulary: http://vocabularies.coar-repositories.org/documentation/resource_types/
.. _COAR Access Right Vocabulary: http://vocabularies.coar-repositories.org/documentation/access_rights/
.. _COAR Version Vocabulary: http://vocabularies.coar-repositories.org/documentation/version_types/
.. _IETF BCP 47: http://tools.ietf.org/rfc/bcp/bcp47.txt
.. _ISO 639-3: https://iso639-3.sil.org/ 

.. toctree::
   :numbered:
   :maxdepth: 1
   :hidden:

   field_title
   field_creator
   field_contributor
   field_projectid
   field_resourceidentifier
   field_alternativeidentifier
   field_relatedidentifier
   field_embargoenddate
   field_language
   field_publisher
   field_publicationtype
   field_resourceversion
   field_description
   field_format
   field_accessrights
   field_source
   field_subject
   field_licensecondition
   field_coverage
   field_size
   field_geolocation
   field_filelocation
   field_citationtitle
   field_citationvolume
   field_citationissue
   field_citationstartpage
   field_citationendpage
   field_citationedition
   field_citationconferenceplace
   field_citationconferencedate
   field_audience
   field_thesis


.. _WebDewey: http://dewey.org/webdewey/login/login.html


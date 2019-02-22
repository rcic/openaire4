.. _dci:contribuidor:

Contribuidor (MA)
=================

``datacite:contribuidor``

Cardinalidad
~~~~~~~~~~~~

*Obligatoria si aplica*

*Ocurrencia: 0-n*

Definición y instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

La institución o persona responsable de recolectar, administrar, distribuir o contribuir de otra manera al desarrollo del recurso.

**No confundir con**

* :ref:`dc:editor`
* :ref:`dci:autor`
* :ref:`aire:referenciaFinanciación`

**Observaciones**

* adaptado desde `DataCite MetadataKernel`_ v4.1

Propiedad de contribuidor (MA, 0-n)
----------------------------------

.. _dci:contributor_contributorType:

Atributo de tipoContribuidor (M)
--------------------------------

El tipo de contribuidor del recurso (ocurrencia: 1). Obligatorio si se utiliza *contribuidor*.

.. include:: vocabularies/contributortype.rst

.. _dci:contributor_contributorName:

Subpropiedad nombreContribuidor (M)
-----------------------------------

El nombre del contribuidor (ocurrencia: 1). Obligatorio si se utiliza *Contribuidor*.

.. _dci:contributor_nameType:

Atributo tipoNombre (R)
***********************

El tipo de nombre (ocurrencia: 0-1).

.. include:: vocabularies/nametype.rst

.. _dci:contributor_familyName:

Subpropiedad nombreFamilia (O)
------------------------------

El apellido del contribuidor (ocurrencia: 0-1).

.. _dci:contributor_givenName:

Subpropiedad nombreDado (O)
---------------------------

El primer o nombre personal del contribuidor (ocurrencia: 0-1).


.. _dci:contributor_nameIdentifier:

Subpropiedad identificadorNombre (R)
------------------------------------

Identifica de forma única a una persona física o jurídica, de acuerdo con varios esquemas (occurrence: 0-n).

.. _dci:contributor_nameIdentifierScheme:

Atributo esquemaIdentificadorNombre (M)
***************************************

El nombre de los esquemas de identificador de nombre (ocurrencia: 1). Obligatoria si *identificadorNombre* es usada.

.. _dci:contributor_schemeURI:

Atributo URIesquema (R)
***********************

La URI de los esquemas de identificador de nombre (ocurrencia: 0-1).

.. _dci:contributor_affiliation:

Subpropiedad de afiliación (R)
------------------------------

La afiliación organizacional o institucional del contribuidor.

Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:

   <datacite:contributors>
	   <datacite:contributor>
	     <datacite:contributorName>Evans, R. J.</datacite:contributorName>
	   <datacite:contributor>
	   <datacite:contributor>
	     <datacite:contributorName>International Human Genome Sequencing Consortium</datacite:contributorName>
	   </datacite:contributor>
   </datacite:contributors>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
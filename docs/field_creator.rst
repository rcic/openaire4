.. _dci:autor:

Autor (M)
===========

``datacite:autor``

Cardinalidad
~~~~~~~~~~~~

*Obligatoria*

*Ocurrencia: 1-n*

Definición y instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Los autores de la publicación en orden de prioridad. Puede ser un nombre corporativo / institucional o personal.

**No confundir con**

* :ref:`dci:contribuidor`
* :ref:`dc:editor`

**Observaciones**

* adaptado desde `DataCite MetadataKernel`_ v4.1

Propiedades de autor (M, 1-n)
-----------------------------

.. _dci:autor_nombreAutor:

Subpropiedad nombreAutor (M)
----------------------------

El nombre del autor (ocurrencia: 1). El formato debe ser: familiar, dado. Los nombres no romanos pueden ser transcritos de acuerdo con el
`ALA-LC <http://www.loc.gov/catdir/cpso/roman.html>`_ esquemas.

.. _dci:autor_nombreTipo:

Atributo nombreTipo (R)
***********************

El tipo de nombre (ocurrencia: 0-1).

.. include:: vocabularies/nametype.rst

.. _dci:creator_givenName:

Subpropiedad nombreDado (R)
---------------------------

El primer o nombre personal del autor.

.. _dci:creator_familyName:

Subpropiedad nombreFamilia (R)
------------------------------

El apellido del autor.

.. _dci:creator_nameIdentifier:

Subpropiedad identificadorNombre (R)
------------------------------------

Identifica de forma única a una persona física o jurídica, de acuerdo con varios esquemas (ocurrencias: 0-n).
El formato depende del esquema.

.. note:: 
   OpenAIRE recomienda incluir un identificadorNombre, como ORCID o ISNI, si está disponible.


.. _dci:creator_nameIdentifier_nameIdentifierScheme:

Atributo esquemaIdentificadorNombre (M)
***************************************

El nombre de los esquemas de identificador de nombre (ocurrencia: 1).
Obligatorio si se usa identificadorNombre.

.. _dci:creator_nameIdentifier_schemeURI:

Atributo URIesquema (R)
***********************

La URI de los esquemas de identificador de nombre (ocurrencia: 0-1).

.. _dci:creator_affiliation:

Subpropiedad de afiliación (R)
------------------------------

La afiliación organizacional o institucional del autor (ocurrencia: 0-n).

Ejemplo
~~~~~~~
.. code-block:: xml
   :linenos:

   <datacite:creators>
     <datacite:creator>
       <datacite:creatorName>Evans, R.J.</datacite:creatorName>
       <datacite:affiliation>Institute of Science and Technology</datacite:affiliation>
       <datacite:nameIdentifier nameIdentifierScheme="ORCID"
                       schemeURI="http://orcid.org">
         1234-1234-1234-1234
       </datacite:nameIdentifier>
     </datacite:creator>
   </datacite:creators>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
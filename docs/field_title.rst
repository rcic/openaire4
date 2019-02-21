.. _dci:título:

.. _dci:título_título:

Título (M)
=========

``datacite:título``

Cardinalidad
~~~~~~~~~~~~

*Obligatoria*

*Ocurrencia: 1-n*

Definición y instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Un nombre o título por el cual se conoce un recurso.

**Valores permitidos, ejemplos, otras restricciones**

Texto libre.

**Observaciones**

* adaptado desde `DataCite MetadataKernel`_ v4.1

Propiedades de título (M, 1-n)
------------------------------

Utilice el nombre del título como valor. Repita esta propiedad para diferentes tipos de títulos o idiomas de títulos.

Lenguaje de atributos (O)
-------------------------

El idioma del título (ocurrencia: 0-1)

Use el atributo ``xml:lang`` para indicar el idioma del título. El valor del atributo debe elegirse de IETF BCP 47, el `IANA Language Subtag Registry <http://www.iana.org/assignments/language-subtag-registry>`_.


Atributo título tipo (O)
------------------------

El tipo de Título (occurrences: 0-1).

**Valores permitidos, ejemplos, otras restricciones**

.. include:: vocabularies/titletype.rst


Ejemplo
~~~~~~~
.. code-block:: xml
   :linenos:

    <datacite:title xml:lang="en-US">
     National Institute for Environmental Studies and Center
     for Climate System Research Japan
    </datacite:title>
    <datacite:title xml:lang="en-US" titleType="Subtitle">A survey</datacite:title>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
.. _dci:geolocation:

Ubicación geográfica (O)
========================

``datacite:geoLocation``

Nombre del campo
----------------

Campo normalizado:
~~~~~~~~~~~~~~~~~~
geoLocation

Campo con esquema de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
datacite:geoLocation

Traducción al español:
~~~~~~~~~~~~~~~~~~~~~~
Ubicación geográfica

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Opcional (O)

Niveles de Ocurrencia (R/NR - Cantidad Veces)
---------------------------------------------
Repetible ( R)

Definición y Alcance del campo
------------------------------
Lugar donde se recuperaron los datos del recurso. Repita el campo si el recurso cuenta con ubicaciones diferentes.

Forma de Descripción Normalizada (RDA/RCAA2)
-----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
datacite:geoLocation

Relaciones con otros campos
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Restricciones
~~~~~~~~~~~~~

Ejemplos
~~~~~~~~

.. code-block:: xml
   :linenos:

   	<datacite:geoLocations>
   	<datacite:geoLocation>
    	<datacite:geoLocationPlace>Oceano Atlántico</datacite:geoLocationPlace>
    	<datacite:geoLocationPoint>
             <datacite:pointLongitude>31.233</datacite:pointLongitude>
        	     <datacite:pointLatitude>-67.302</datacite:pointLatitude>
    	</datacite:geoLocationPoint>
    <datacite:geoLocationBox>
	<datacite:westBoundLongitude>-71.032</datacite:westBoundLongitude>
             <datacite:eastBoundLongitude>-68.211</datacite:eastBoundLongitude>
             <datacite:southBoundLongitude>41.090</datacite:southBoundLongitude>
             <datacite:northBoundLongitude>42.893</datacite:northBoundLongitude>
    </datacite:geoLocationBox>
 	</datacite:geoLocation>
	</datacite:geoLocations>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

Atributos de Campo
------------------

Especificadores de Campo
------------------------

Niveles de Aplicación - Productos de Colciencias
------------------------------------------------
Se aplica a todos los productos de Colciencias.

Observaciones del Campo
-----------------------

Adaptado de
~~~~~~~~~~~

Relaciones con otros modelos de metadatos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Niveles Semánticos
~~~~~~~~~~~~~~~~~~

Recomendación de Campos de aplicación en DSPACE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LAREFERENCIA, OPENAIRE2, OPENAIRE3)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Otras Observaciones
~~~~~~~~~~~~~~~~~~~

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
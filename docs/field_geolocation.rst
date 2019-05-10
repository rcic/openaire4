.. _dci:geolocation:

Ubicación geográfica (O)
========================

``datacite:geoLocation``

Definición y alcance del campo
------------------------------
Lugar donde se recuperaron los datos del recurso. Repita el campo si el recurso cuenta con ubicaciones diferentes.

Niveles de requerimientos (M/MA/R/O)
------------------------------------
Opcional (O)

Niveles de ocurrencia (R / NR -  Cantidad Veces)
------------------------------------------------
Repetible (R)

Campo con esquema de metadatos
------------------------------
datacite:geoLocation

Traducción al español
---------------------
Ubicación geográfica

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

Valores permitidos (Vocabularios Controlados)
---------------------------------------------
datacite:geoLocation

Relaciones con otros campos
---------------------------

Restricciones
-------------

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


Atributos de campo
------------------

Especificadores de campo
------------------------

- datacite:pointLongitude
- datacite:pointLatitude   
- datacite:geoLocationBox
- datacite:westBoundLongitude
- datacite:eastBoundLongitude
- datacite:southBoundLongitude         
- datacite:northBoundLongitude


Niveles de aplicación para productos de investigación de Colciencias
--------------------------------------------------------------------
Se aplica a todos los productos de Colciencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

Niveles semánticos
------------------

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear los siguientes campos en Dspace:

- datacite:geoLocation
- datacite:pointLongitude
- datacite:pointLatitude   
- datacite:geoLocationBox
- datacite:westBoundLongitude
- datacite:eastBoundLongitude
- datacite:southBoundLongitude         
- datacite:northBoundLongitude


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

.. _dci:geolocation:

Geo Location (Ubicación geográfica) (O)
=======================================

``datacite:geoLocation``

Definición y alcance del campo
------------------------------
Este campo se utiliza para describir los lugares geográficos donde se llevaron a cabo las investigaciones o el lugar de referencia dentro del recurso (Región espacial o lugar con nombre donde se recopilaron los datos o sobre los cuales se enfocaron los datos.) ó lugar de publicación del recurso. Está información delimitará a cada producto o recurso de investigación y se podrán obtener con precisión la cantidad de investigaciones realizadas en un área geográfica delimitada.

Niveles de persistencia (M/MA/R/O)
------------------------------------
Opcional (O)

Niveles de ocurrencia (R / NR)
------------------------------
Repetible (R): 0-n veces. Repita el campo si el recurso cuenta con ubicaciones diferentes.

Esquema de metadatos
--------------------
datacite:geoLocation

Traducción al español
---------------------
Ubicación geográfica

Forma de Descripción Normalizada (RDA / RCAA2)
----------------------------------------------
RDA (Recursos: descripción y acceso)

  - Cuando describa coordenadas geográficas, se recomienda utilizar las coordenadas codificadas según el modelo **WGS 84 (Sistema geodésico mundial).** Este modelo usa solo números decimales para las coordenadas. Las longitudes son -180 a 180 (0 es Greenwich, los números negativos son al oeste, los números positivos son al este), las latitudes son -90 a 90 (0 es el ecuador; los números negativos son al sur, los números positivos al norte).
  - Un cuadro (box/geoLocationBox)  está definido por dos puntos geográficos. Esquina inferior izquierda (normalmente sur oeste), esquina superior derecha (normalmente noreste). Cada punto está definido por su longitud y latitud.


Propiedades, atributos y especificadores de campo
-------------------------------------------------

Clase Principal Ubicaciones Geográficas (geoLocations) (O, 0-n): 
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Describa todas las posibles regiones espaciales o lugares con nombre donde se recopilaron los datos o sobre los cuales se enfocaron los datos.

Propiedad: Ubicación Geográfica (geoLocation) (O, 0-n): 
+++++++++++++++++++++++++++++++++++++++++++++++++++++++

Describa cada una de las posibles ubicaciones geográficas asociadas. Repita esta propiedad para indicar varias ubicaciones diferentes.

  - Sub-Propiedad: Lugar Geográfico (geoLocationPlace) (O, 0-n) : Descripción de una ubicación geográfica

  - Sub-Propiedad: Punto Geográfico (geoLocationPoint) (O, 0-n) : Un punto de ubicación en el espacio. Un punto contiene un solo par de latitud-longitud.

      - Sub-Propiedad: Punto Longitud (pointLongitude) (M, 1) : Dimensión longitudinal del punto.

      - Sub-Propiedad: Punto Latitud (pointLatitude) (M, 1) : Dimensión latitudinal del punto.
  
  - Sub-Propiedad: Punto Geográfico (geoLocationBox) (O, 0-n) : Los límites espaciales de un lugar o cuadro.
    
      - Sub-Propiedad: Punto Longitud (westBoundLongitude) (M, 1) : Coordenada (Longitud) de la  Esquina Superior Izquierda.

      - Sub-Propiedad: Punto Latitud (northBoundLatitude) (M, 1) : Coordenada (Latitud) de la Esquina Superior Izquierda. 

      - Sub-Propiedad: Punto Longitud (eastBoundLongitude) (M, 1) : Coordenada (Longitud) de la Esquina Inferior Derecha. 

      - Sub-Propiedad: Punto Latitud (southBoundLatitude) (M, 1) : Coordenada (Latitud) de la  Esquina Inferior Derecha.

  - Sub-Propiedad: Polígono Geográfico (geoLocationPolygon) (O, 0-n) : Un área de polígono dibujado, definida por un conjunto de puntos y líneas que conectan los puntos en una cadena cerrada.

      - Sub-Propiedad: Punto Polígono (polygonPoint) (M, 4-n) : Un punto de ubicación en un polígono.
        
        - Sub-Propiedad: Punto Longitud (pointLongitude) (M, 1) : Dimensión longitudinal del punto.
        
        - Sub-Propiedad: Punto Latitud (pointLatitude) (M, 1) : Dimensión latitudinal del punto.
          
      - Sub-Propiedad: Punto dentro de un Polígono (inPolygonPoint ) (M, 4-n) : Para cualquier área delimitada que sea más grande que la mitad de la tierra, defina un punto (aleatorio) en el interior.
      
        - Sub-Propiedad: Punto Longitud (pointLongitude) (M, 1) : Dimensión longitudinal del punto.

        - Sub-Propiedad: Punto Latitud (pointLatitude) (M, 1) : Dimensión latitudinal del punto. 

Relaciones con otros campos
---------------------------

    - El campo datacite:geoLocation está relacionado con el campo dc.coverage.spatial

Restricciones
-------------

Ninguna

Ejemplos y ayudas
-----------------

Ayudas
++++++

  - **Ej: dc.geoLocation.geoLocationPlace:**  Frente a Banco Gordo  
  - **Ej: dc.geoLocation.geoLocationPoint** -109.4566667 23.14166667
  - **Ej: dc.geoLocation.geoLocationBox** -111.9816376 27.91061913 -111.98134240 27.91141073
  - **Ej: datacite.geolocation.geolocationPlace** Jasper N.P. (N. Bdry.)

Ejemplo en XML (Interoperabilidad OAI-PMH)
++++++++++++++++++++++++++++++++++++++++++

**Esquema oai_dc**

.. code-block:: xml
   :linenos:

   <dc.coverage>Límite noroeste de la Cuenca de Guaymas</dc.coverage>

**Esquema DataCite**

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

**Esquema xoai**

.. code-block:: xml
   :linenos:

   <element name="datacite">
     <element name="geoLocationBox">
           <element name="westBoundLongitude">
                   <element name="en_US">
                        <field name="value">23.04</field>
                   </element>
           </element>
           <element name="eastBoundLongitude">
                   <element name="en_US">
                        <field name="value">-82.75</field>
                   </element>
           </element>
           <element name="southBoundLatitude">
                   <element name="en_US">
                        <field name="value">22.60</field>
                   </element>
           </element>
           <element name="northBoundLatitude">
                   <element name="en_US">
                        <field name="value">-82.24</field>
                   </element>
           </element>
   </element>
   </element>

**Esquema dim**

.. code-block:: xml
   :linenos:

   <dim:field mdschema ="datacite" element ="geoLocationPoint" qualifier ="pointLongitude">31.233</dim:field>
   <dim:field mdschema ="datacite" element ="geoLocationPoint" qualifier ="pointLatitude">-67.302</dim:field>

Niveles de aplicación para productos de investigación de MinCiencias
--------------------------------------------------------------------
Se aplica a todos los productos de MinCiencias. 

Relaciones con otros modelos de metadatos
-----------------------------------------

El campo ubicación geográfica **(datacite:geoLocation)** es utilizado por los siguientes esquemas de metadatos y puede intercambiarse su uso de manera indistinta mientras se conserven sus distintos niveles de atributos y especificadores de campo:

+----------------------+--------------------------+
| Esquema de Metadatos | Campo Relacionado        |
+======================+==========================+
| dc                   | dc.publisher (city)      |
+----------------------+--------------------------+
| dcterms              | dcterms.publisher (city) |
+----------------------+--------------------------+
| marcxml              | field: 260$a / 264$a     |
+----------------------+--------------------------+

Niveles semánticos
------------------
No aplica

Recomendación de campos de aplicación en DSPACE
-----------------------------------------------
Se recomienda crear/modificar el componente de registro de metadatos (y sus correspondientes hojas de entrada de datos) de los sistemas **DSPACE** basados en los siguientes elementos:

+----------------------+-----------------------------+-----------------------+-----------------+
| Esquema de Metadatos | Campo Elemento DSPACE       | Calificadores         | Nota de alcance |
+======================+=============================+=======================+=================+
| DataCite             | datacite.geoLocationPlace   |                       |                 |
+----------------------+-----------------------------+-----------------------+-----------------+
| DataCite             | datacite.geoLocationPoint   |                       |                 |
+----------------------+-----------------------------+-----------------------+-----------------+
|                      |                             | pointLongitude        |                 |
+----------------------+-----------------------------+-----------------------+-----------------+
|                      |                             | pointLatitude         |                 |
+----------------------+-----------------------------+-----------------------+-----------------+
| DataCite             | datacite.geoLocationBox     |                       |                 |
+----------------------+-----------------------------+-----------------------+-----------------+
|                      |                             | westBoundLongitude    |                 |
+----------------------+-----------------------------+-----------------------+-----------------+
|                      |                             | eastBoundLongitude    |                 |
+----------------------+-----------------------------+-----------------------+-----------------+
|                      |                             | southBoundLongitude   |                 |
+----------------------+-----------------------------+-----------------------+-----------------+
|                      |                             | northBoundLongitude   |                 |
+----------------------+-----------------------------+-----------------------+-----------------+
| DataCite             | datacite.geoLocationPolygon |                       |                 |
+----------------------+-----------------------------+-----------------------+-----------------+
|                      |                             | polygonPointLatitude  |                 |
+----------------------+-----------------------------+-----------------------+-----------------+
|                      |                             | polygonPointLongitude |                 |
+----------------------+-----------------------------+-----------------------+-----------------+


Recomendaciones de migración de Modelos anteriores (BDCOL, SNAAC, LA REFERENCIA, OPENAIRE 2, OPENAIRE 3)
--------------------------------------------------------------------------------------------------------

  - Se recomienda específicamente crear los nuevos atributos/especificadores de campo de tamaño según la codificación propuesta.

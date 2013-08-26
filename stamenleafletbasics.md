+<!DOCTYPE html>
+<html>
+    <head>
+        <title>Bike Valet Map</title>
+        <script type="text/javascript" src="http://leaflet.cloudmade.com/dist/leaflet.js"></script>
+        <link rel="stylesheet" href="http://leaflet.cloudmade.com/dist/leaflet.css" />
+        <!--[if lte IE 8]><link rel="stylesheet" href="http://leaflet.cloudmade.com/dist/leaflet.ie.css" /><![endif]-->
+        
+        <script type="text/javascript" src="../js/tile.stamen.js?v1.2.3"></script>
+        <script type="text/javascript">
+            function initialize() {
+                var layers = ["toner"];
+              
+                    var layer = layers[0];
+                    var map = new L.Map(layer, {
+                                        center: new L.LatLng(37.8, -122.4),
+                                        zoom: 10
+                                        });
+                    map.addLayer(new L.StamenTileLayer(layer));
+                
+            }
+            </script>
+        <style type="text/css">
+            .map {
+                width: 600px;
+                height: 320px;
+                margin: 0 0 1em 0;
+            }
+            </style>
+    </head>
+    <body onload="initialize()">
+        <div id="toner" class="map"></div>
+        <div id="terrain" class="map"></div>
+        <div id="watercolor" class="map"></div>
+    </body>
+</html>

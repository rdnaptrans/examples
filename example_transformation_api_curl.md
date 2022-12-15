# Calling Transformation API from command line with cURL

#### GeoJSON in-line
<tt>curl --location --request POST https://api.transformation.nsgi.nl/v1/transform --header "X-Api-Key: <strong><em>put_your_own_key_here</em></strong>" --header "Accept-Crs: <strong>EPSG:7931</strong>" --header "Content-Crs: <strong>EPSG:7415</strong>" --header "Content-Type: application/json" --data "{ \"data\": { \"type\": \"MultiPoint\", \"coordinates\": [ <strong>[ 155000.000, 463000.000, 100.000 ], [ 155000.000, 463000.000 ]</strong> ] }, \"acceptDeviationLongLineSegments\": <strong>0.001</strong>}"</tt>

#### GeoJSON in file
<tt>curl --location --request POST https://api.transformation.nsgi.nl/v1/transform --header "X-Api-Key: <strong><em>put_your_own_key_here</em></strong>" --header "Accept-Crs: <strong>EPSG:7931</strong>" --header "Content-Crs: <strong>EPSG:7415</strong>" --header "Content-Type: application/json" --data @<strong>input.json</strong></tt>

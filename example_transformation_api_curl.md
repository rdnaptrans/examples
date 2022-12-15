Calling Transformation-API form command line with cURL

curl --location --request POST https://api.transformation.nsgi.nl/v1/transform --header "X-Api-Key: put_your_own_key_here" --header "Accept-Crs: EPSG:7931" --header "Content-Crs: EPSG:7415" --header "Content-Type: application/json" --data-raw "{ \"data\": { \"type\": \"MultiPoint\", \"coordinates\": [ [ 155000.000, 463000.000, 100.000 ], [ 155000.000, 463000.000 ] ] },\"acceptDeviationLongLineSegments\": 0.001}"

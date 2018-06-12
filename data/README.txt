**General info 
According to the Inspection Centres 2018 file; 
Zimbabwe is composed of 10 Provinces , 126 districts and 210 constituency
also 89 Local authority

**GET lat lon for a way by the node ID
https://www.openstreetmap.org/api/0.6/way/275461128/full

**Overpass 
http://overpass-turbo.eu/#

**basic overpass querry : 
[out:json];
// gather results
(
  node["amenity"="university"]({{bbox}});
  way["amenity"="university"]({{bbox}});
  relation["amenity"="university"]({{bbox}});
);
// print results
out body;
>;
out skel qt;

**List of AMenty to filter with :
https://wiki.openstreetmap.org/wiki/Key:amenity

** Zimbabwe statistics
http://www.zimstat.co.zw/

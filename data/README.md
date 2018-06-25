<h1>First interaction with data</h1>
<h4>Related websites Ressources :</h4> 

* Election Instance <br/>
http://zec.gov.zw
* Zimbabwe statistics <br/>
http://www.zimstat.co.zw/
* Election Ressource center <br/>
https://erczim.org/
* Vote's watch <br/>
http://www.votewatch263.org.zw/
* Election Support Network <br/>
http://www.zesn.org.zw/

<h4>General Shapes info :</h4> 
According to the Inspection Centres 2018 file;
Zimbabwe is composed of 10 Provinces , 63 districts and 210 constituency
also 89 Local authority
each province has a set of warrds arround 1200 ward in total

<h4>Getting data from Open Street Map</h4>

* get lat lon for a way by the node ID: <br/> https://www.openstreetmap.org/api/0.6/way/275461128/full

* Overpass Link: <br/>
http://overpass-turbo.eu/#

* List of Amenty to filter with :
https://wiki.openstreetmap.org/wiki/Key:amenity

* Basic overpass querry : 
~~~~
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
~~~~
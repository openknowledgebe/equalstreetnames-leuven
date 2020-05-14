/**
 * Get all the relevant relations in Brussels Region.
 */
[out:json][timeout:300];
( area["admin_level"="8"]["ref:INS"="24062"]["wikidata"="Q118958"]; )->.a;
(
    relation["type"="associatedStreet"](area.a);
    relation["type"="street"](area.a);
    relation["type"="multipolygon"]["place"]["name"](area.a);
    relation["type"="multipolygon"]["highway"]["name"](area.a);
);
out body;
>;
out skel qt;
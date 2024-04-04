
# AdministrativeBoundary Feature (Schema)

`ogc.bbr.template.AdministrativeBoundaryFeature` *v1.0*

Defines a specific interoperability profile of the AdministrativeBoundary for OGC API Feature schemas and Inspire data model

[*Status*](http://www.opengis.net/def/status): Under development

## Description


## AdministrativeBoundary Inspire Data Model Profile for OGC API

This specification defines the specific requirements of the AdministrativeBoundary Information Model.
Administrative Boundary is defined like a line of demarcation between administrative units.

- [INSPIRE Administrative Boundary](https://inspire.ec.europa.eu/featureconcept/AdministrativeBoundary)
- [OGC-API IDE CATALONIA AdministrativeBoundary](https://geoserveis.ide.cat/servei/catalunya/inspire/ogc/features/collections/inspire:AU.AdministrativeBoundary/)

![Model](./assets/model.png)

## Key features of this profile:
- a schema for the AdministrativeBoundary element with the Inspire data model
- a JSON-LD context for this result schema
- JSON-LD context elements defining namespaces for the values
## Examples

### Example of AdministrativeBoundary Feature
#### json
```json

{
    "@context": {
      "mynamespace": "http://example.org/ns1/"
    },
    "id": "AU.AdministrativeBoundary.ID.AU.linia.1",
    "type": "Feature",
    "geometry": {
      "type": "LineString",
      "coordinates": [
        [
          -111.67183507997295,
          40.056709946862874
        ],
        [
          -111.71,
          40.156709946862874
        ]
      ]
    },
    "properties": {
        "localid": "ID.AU.linia.1",
        "country": "ES",
        "nationallevel": "4th order",
        "legalstatus": "agreed",
        "technicalstatus": "edgeMatched",
        "administrativeunit1": "080018",
        "administrativeunit2": "080543",
        "beginlifespanversion": "2017-07-26",
        "namespace": "Catalunya.AU",
        "versionid": "20230511"
    }
  }
  
```

#### jsonld
```jsonld
{
  "@context": [
    "http://localhost:9090/register/build-local/annotated/bbr/template/AdministrativeBoundaryFeature/context.jsonld",
    {
      "mynamespace": "http://example.org/ns1/"
    }
  ],
  "id": "AU.AdministrativeBoundary.ID.AU.linia.1",
  "type": "Feature",
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        -111.67183507997295,
        40.056709946862874
      ],
      [
        -111.71,
        40.156709946862875
      ]
    ]
  },
  "properties": {
    "localid": "ID.AU.linia.1",
    "country": "ES",
    "nationallevel": "4th order",
    "legalstatus": "agreed",
    "technicalstatus": "edgeMatched",
    "administrativeunit1": "080018",
    "administrativeunit2": "080543",
    "beginlifespanversion": "2017-07-26",
    "namespace": "Catalunya.AU",
    "versionid": "20230511"
  }
}
```

#### ttl
```ttl
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<http://example.com/features/AU.AdministrativeBoundary.ID.AU.linia.1> a geojson:Feature ;
    geojson:geometry [ a geojson:LineString ;
            geojson:coordinates ( ( -1.116718e+02 4.005671e+01 ) ( -1.1171e+02 4.015671e+01 ) ) ] .


```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: Example of a simple GeoJSON Feature AdministrativeBoundary with Inspire
  Model
$defs:
  MyFeature:
    allOf:
    - $ref: https://opengeospatial.github.io/bblocks/annotated-schemas/geo/features/feature/schema.yaml
    - properties:
        properties:
          $ref: http://localhost:9090/register/build-local/annotated/bbr/template/AdministrativeBoundary/schema.yaml
anyOf:
- $ref: '#/$defs/MyFeature'

```

Links to the schema:

* YAML version: [schema.yaml](http://localhost:9090/register/build-local/annotated/bbr/template/AdministrativeBoundaryFeature/schema.json)
* JSON version: [schema.json](http://localhost:9090/register/build-local/annotated/bbr/template/AdministrativeBoundaryFeature/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "type": "@type",
    "id": "@id",
    "properties": "@nest",
    "geometry": {
      "@context": {
        "coordinates": {
          "@container": "@list",
          "@id": "geojson:coordinates"
        }
      },
      "@id": "geojson:geometry"
    },
    "bbox": {
      "@container": "@list",
      "@id": "geojson:bbox"
    },
    "Feature": "geojson:Feature",
    "FeatureCollection": "geojson:FeatureCollection",
    "GeometryCollection": "geojson:GeometryCollection",
    "LineString": "geojson:LineString",
    "MultiLineString": "geojson:MultiLineString",
    "MultiPoint": "geojson:MultiPoint",
    "MultiPolygon": "geojson:MultiPolygon",
    "Point": "geojson:Point",
    "Polygon": "geojson:Polygon",
    "features": {
      "@container": "@set",
      "@id": "geojson:features"
    },
    "links": {
      "@context": {
        "href": {
          "@type": "@id",
          "@id": "oa:hasTarget"
        },
        "rel": {
          "@context": {
            "@base": "http://www.iana.org/assignments/relation/"
          },
          "@id": "http://www.iana.org/assignments/relation",
          "@type": "@id"
        },
        "type": "dct:type",
        "hreflang": "dct:language",
        "title": "rdfs:label",
        "length": "dct:extent"
      },
      "@id": "rdfs:seeAlso"
    },
    "geojson": "https://purl.org/geojson/vocab#",
    "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
    "oa": "http://www.w3.org/ns/oa#",
    "dct": "http://purl.org/dc/terms/",
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](http://localhost:9090/register/build-local/annotated/bbr/template/AdministrativeBoundaryFeature/context.jsonld)

## Sources

* [OGC API - Features, Part 1, 7.16.2: Feature Response](https://docs.ogc.org/is/17-069r3/17-069r3.html#_response_7)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/MayteToscano/bblock-template](https://github.com/MayteToscano/bblock-template)
* Path: `_sources/AdministrativeBoundaryFeature`


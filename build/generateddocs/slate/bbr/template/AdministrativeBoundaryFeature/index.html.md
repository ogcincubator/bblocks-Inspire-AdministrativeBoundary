---
title: AdministrativeBoundary Feature (Schema)

language_tabs:
  - json: JSON
  - jsonld: JSON-LD
  - turtle: RDF/Turtle

toc_footers:
  - Version 1.0
  - <a href='#'>AdministrativeBoundary Feature</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: AdministrativeBoundary Feature (Schema)
---


# AdministrativeBoundary Feature `ogc.bbr.template.AdministrativeBoundaryFeature`

Defines a specific interoperability profile of the AdministrativeBoundary for OGC API Feature schemas and Inspire data model

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="success">
This building block is <strong><a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/blob/main/build/tests/bbr/template/AdministrativeBoundaryFeature/" target="_blank">valid</a></strong>
</aside>

# Description


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
# Examples

## Example of AdministrativeBoundary Feature



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

<blockquote class="lang-specific json">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/tests/bbr/template/AdministrativeBoundaryFeature/example_1_1.json">Open in new window</a>
    <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=json&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-Inspire-AdministrativeBoundary%2Fbuild%2Ftests%2Fbbr%2Ftemplate%2FAdministrativeBoundaryFeature%2Fexample_1_1.json&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on JSON Viewer</a></p>
</blockquote>




```jsonld
{
  "@context": [
    "https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/AdministrativeBoundaryFeature/context.jsonld",
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

<blockquote class="lang-specific jsonld">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/tests/bbr/template/AdministrativeBoundaryFeature/example_1_1.jsonld">Open in new window</a>
    <a target="_blank" href="https://json-ld.org/playground/#json-ld=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-Inspire-AdministrativeBoundary%2Fbuild%2Ftests%2Fbbr%2Ftemplate%2FAdministrativeBoundaryFeature%2Fexample_1_1.jsonld">View on JSON-LD Playground</a>
</blockquote>




```turtle
@prefix geojson: <https://purl.org/geojson/vocab#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<http://example.com/features/AU.AdministrativeBoundary.ID.AU.linia.1> a geojson:Feature ;
    geojson:geometry [ a geojson:LineString ;
            geojson:coordinates ( ( -1.116718e+02 4.005671e+01 ) ( -1.1171e+02 4.015671e+01 ) ) ] .


```

<blockquote class="lang-specific turtle">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/tests/bbr/template/AdministrativeBoundaryFeature/example_1_1.ttl">Open in new window</a>
</blockquote>



# JSON Schema

```yaml--schema
$schema: https://json-schema.org/draft/2020-12/schema
description: Example of a simple GeoJSON Feature AdministrativeBoundary with Inspire
  Model
$defs:
  MyFeature:
    allOf:
    - $ref: https://opengeospatial.github.io/bblocks/annotated-schemas/geo/features/feature/schema.yaml
    - properties:
        properties:
          $ref: https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/AdministrativeBoundary/schema.yaml
anyOf:
- $ref: '#/$defs/MyFeature'

```

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-Inspire-AdministrativeBoundary%2Fbuild%2Fannotated%2Fbbr%2Ftemplate%2FAdministrativeBoundaryFeature%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/AdministrativeBoundaryFeature/schema.yaml" target="_blank">https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/AdministrativeBoundaryFeature/schema.yaml</a>
* JSON version: <a href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/AdministrativeBoundaryFeature/schema.json" target="_blank">https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/AdministrativeBoundaryFeature/schema.json</a>


# JSON-LD Context

```json--ldContext
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

> <a target="_blank" href="https://json-ld.org/playground/#json-ld=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-Inspire-AdministrativeBoundary%2Fbuild%2Fannotated%2Fbbr%2Ftemplate%2FAdministrativeBoundaryFeature%2Fcontext.jsonld">View on JSON-LD Playground</a>

You can find the full JSON-LD context here:
<a href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/AdministrativeBoundaryFeature/context.jsonld" target="_blank">https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/AdministrativeBoundaryFeature/context.jsonld</a>

# References

* [OGC API - Features, Part 1, 7.16.2: Feature Response](https://docs.ogc.org/is/17-069r3/17-069r3.html#_response_7)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary" target="_blank">https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary</a>
* Path:
<code><a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/blob/HEAD/_sources/AdministrativeBoundaryFeature" target="_blank">_sources/AdministrativeBoundaryFeature</a></code>


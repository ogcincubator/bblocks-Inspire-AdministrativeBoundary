
# AdministrativeBoundary (Schema)

`ogc.bbr.template.AdministrativeBoundary` *v0.1*

Defines a specific interoperability profile of the AdministrativeBoundary dataset with the Inspire data model

[*Status*](http://www.opengis.net/def/status): Under development

## Description


## AdministrativeBoundary Inspire Data Model Profile for OGC API

This specification defines the specific requirements of the AdministrativeBoundary Information Model.
Administrative Boundary is defined like a line of demarcation between administrative units.

- [INSPIRE Administrative Boundary](https://inspire.ec.europa.eu/featureconcept/AdministrativeBoundary)
- [OGC-API IDE CATALONIA AdministrativeBoundary](https://geoserveis.ide.cat/servei/catalunya/inspire/ogc/features/collections/inspire:AU.AdministrativeBoundary/)

## Key features of this profile:
- a schema for the AdministrativeBoundary element with the Inspire data model
- a JSON-LD context for this result schema
- JSON-LD context elements defining namespaces for the values
## Examples

### Example of AdministrativeBoundary API
#### json
```json
{
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
  
```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: A line of demarcation between administrative units.
type: object
properties:
  localid:
    type: string
    pattern: ^ID\.AU\.linia\.\d+$
  country:
    type: string
    enum:
    - ES
  allOf:
    $ref: https://raw.githubusercontent.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/main/build/annotated/bbr/template/TechnicalStatusValue/schema.yaml
  administrativeunit1:
    type: string
  administrativeunit2:
    type: string
  beginlifespanversion:
    type: string
    format: date-time
  namespace:
    type: string
  versionid:
    type: string
required:
- localid
- country
- nationallevel
- legalstatus
- technicalstatus
- administrativeunit1
- administrativeunit2
- beginlifespanversion
- namespace
- versionid

```

Links to the schema:

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/main/build/annotated/bbr/template/AdministrativeBoundary/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/main/build/annotated/bbr/template/AdministrativeBoundary/schema.yaml)

## Sources

* [INSPIRE registry](https://inspire.ec.europa.eu/featureconcept/AdministrativeBoundary)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary](https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary)
* Path: `_sources/AdministrativeBoundary`



# TechnicalStatusValue (Schema)

`ogc.bbr.template.TechnicalStatusValue` *v0.1*

enumeration

[*Status*](http://www.opengis.net/def/status): Under development

## Description


## Enumeration TechnicalStatusValue
Description of the technical status of administrative boundaries.
## Values TechnicalStatusValue
| Status      | Description                                                                                   |
|-------------|-----------------------------------------------------------------------------------------------|
| edgeMatched      | The boundaries of neighbouring administrative units have the same set of coordinates |
| notEdgeMatched   | The boundaries of neighbouring administrative units do not have the same set of coordinates |

 
## Examples

### Example of TechnicalStatusValue Enumeration
#### json
```json
{
  "technicalstatus": "edgeMatched"
}
```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: Schemas for TechnicalStatusValue
type: object
properties:
  technicalstatus:
    description: Description of the technical status of administrative boundaries.
    type: string
    oneOf:
    - const: edgeMatched
      descripcion: The boundaries of neighbouring administrative units have the same
        set of coordinates
    - const: notEdgeMatched
      descripcion: The boundaries of neighbouring administrative units do not have
        the same set of coordinates
required:
- technicalstatus

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/TechnicalStatusValue/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/TechnicalStatusValue/schema.yaml)

## Sources

* [INSPIRE registry](https://inspire.ec.europa.eu/featureconcept/AdministrativeBoundary)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary](https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary)
* Path: `_sources/TechnicalStatusValue`



# LegalStatusValue (Schema)

`ogc.bbr.template.LegalStatusValue` *v0.1*

enumeration

[*Status*](http://www.opengis.net/def/status): Under development

## Description


## Enumeration LegalStatusValue
Description of the legal status of administrative boundaries.
## Values LegalStatusValue
| Status      | Description                                                                                   |
|-------------|-----------------------------------------------------------------------------------------------|
| agreed      | The edge-matched boundary has been agreed between neighbouring administrative units and is stable now |
| notAgreed   | The edge-matched boundary has not yet been agreed between neighbouring administrative units and could be changed |

## Examples

### Example of LegalStatusValue Enumeration
#### json
```json
{
  "legalstatus":  "agreed"
}


```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: Schemas for LegalStatusValue
type: object
properties:
  legalstatus:
    description: Description of the legal status of administrative boundaries.
    type: string
    oneOf:
    - const: agreed
      descripcion: agreed
    - const: notAgreed
      descripcion: notAgreed
required:
- legalstatus

```

Links to the schema:

* YAML version: [schema.yaml](http://localhost:9090/register/build-local/annotated/bbr/template/LegalStatusValue/schema.json)
* JSON version: [schema.json](http://localhost:9090/register/build-local/annotated/bbr/template/LegalStatusValue/schema.yaml)

## Sources

* [INSPIRE registry](https://inspire.ec.europa.eu/featureconcept/AdministrativeBoundary)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/MayteToscano/bblock-template](https://github.com/MayteToscano/bblock-template)
* Path: `_sources/LegalStatusValue`


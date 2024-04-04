
# AdministrativeHierarchyLevel (Schema)

`ogc.bbr.template.AdministrativeHierarchyLevel` *v0.1*

codelist

[*Status*](http://www.opengis.net/def/status): Under development

## Description


## Codelist AdministrativeHierarchyLevel  

Levels of administration in the national administrative hierarchy. This code list reflects the level in the hierarchical pyramid of the administrative structures, which is based on geometric aggregation of territories and does not necessarily describe the subordination between the related administrative authorities.
## Values AdministrativeHierarchyLevel
| Order    | Description                                            |
|----------|--------------------------------------------------------|
| 1st order| Highest level in the national administrative hierarchy |
| 2nd order| 2nd level in the national administrative hierarchy     |
| 3rd order| 3rd level in the national administrative hierarchy     |
| 4th order| 4th level in the national administrative hierarchy     |
| 5th order| 5th level in the national administrative hierarchy     |
| 6th order| 6th level in the national administrative hierarchy     |

## Examples

### Example of AdministrativeHierarchyLevel Codelist
#### json
```json
{
  "nationallevel": "1st order"
}
```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: Schemas for AdministrativeBoundary
type: object
properties:
  nationallevel:
    description: Levels of administration in the national administrative hierarchy.
      This code list reflects the level in the hierarchical pyramid of the administrative
      structures, which is based on geometric aggregation of territories and does
      not necessarily describe the subordination between the related administrative
      authorities.
    type: string
    oneOf:
    - const: 1st order
      descripcion: Highest level in the national administrative hierarchy
    - const: 2nd order
      descripcion: 2nd level in the national administrative hierarchy
    - const: 3rd order
      descripcion: 3rd level in the national administrative hierarchy
    - const: 4th order
      descripcion: 4th level in the national administrative hierarchy
    - const: 5th order
      descripcion: 5th level in the national administrative hierarchyr
    - const: 6th order
      descripcion: 6th level in the national administrative hierarchy
required:
- nationallevel

```

Links to the schema:

* YAML version: [schema.yaml](https://raw.githubusercontent.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/main/build/annotated/bbr/template/AdministrativeHierarchyLevel/schema.json)
* JSON version: [schema.json](https://raw.githubusercontent.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/main/build/annotated/bbr/template/AdministrativeHierarchyLevel/schema.yaml)

## Sources

* [INSPIRE registry](https://inspire.ec.europa.eu/featureconcept/AdministrativeBoundary)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary](https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary)
* Path: `_sources/AdministrativeHierarchyLevel`


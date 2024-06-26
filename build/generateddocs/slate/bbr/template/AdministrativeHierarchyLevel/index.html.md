---
title: AdministrativeHierarchyLevel (Schema)


toc_footers:
  - Version 0.1
  - <a href='#'>AdministrativeHierarchyLevel</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: AdministrativeHierarchyLevel (Schema)
---


# AdministrativeHierarchyLevel `ogc.bbr.template.AdministrativeHierarchyLevel`

codelist

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="success">
This building block is <strong><a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/blob/main/build/tests/bbr/template/AdministrativeHierarchyLevel/" target="_blank">valid</a></strong>
</aside>

# Description


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

# Examples

## Example of AdministrativeHierarchyLevel Codelist



```json
{
  "nationallevel": "1st order"
}
```

<blockquote class="lang-specific json">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/tests/bbr/template/AdministrativeHierarchyLevel/example_1_1.json">Open in new window</a>
    <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=json&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-Inspire-AdministrativeBoundary%2Fbuild%2Ftests%2Fbbr%2Ftemplate%2FAdministrativeHierarchyLevel%2Fexample_1_1.json&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on JSON Viewer</a></p>
</blockquote>



# JSON Schema

```yaml--schema
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

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-Inspire-AdministrativeBoundary%2Fbuild%2Fannotated%2Fbbr%2Ftemplate%2FAdministrativeHierarchyLevel%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/AdministrativeHierarchyLevel/schema.yaml" target="_blank">https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/AdministrativeHierarchyLevel/schema.yaml</a>
* JSON version: <a href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/AdministrativeHierarchyLevel/schema.json" target="_blank">https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/AdministrativeHierarchyLevel/schema.json</a>

# References

* [INSPIRE registry](https://inspire.ec.europa.eu/featureconcept/AdministrativeBoundary)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary" target="_blank">https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary</a>
* Path:
<code><a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/blob/HEAD/_sources/AdministrativeHierarchyLevel" target="_blank">_sources/AdministrativeHierarchyLevel</a></code>


---
title: TechnicalStatusValue (Schema)


toc_footers:
  - Version 0.1
  - <a href='#'>TechnicalStatusValue</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: TechnicalStatusValue (Schema)
---


# TechnicalStatusValue `ogc.bbr.template.TechnicalStatusValue`

enumeration

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="success">
This building block is <strong><a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/blob/main/build/tests/bbr/template/TechnicalStatusValue/" target="_blank">valid</a></strong>
</aside>

# Description


## Enumeration TechnicalStatusValue
Description of the technical status of administrative boundaries.
## Values TechnicalStatusValue
| Status      | Description                                                                                   |
|-------------|-----------------------------------------------------------------------------------------------|
| edgeMatched      | The boundaries of neighbouring administrative units have the same set of coordinates |
| notEdgeMatched   | The boundaries of neighbouring administrative units do not have the same set of coordinates |

 
# Examples

## Example of TechnicalStatusValue Enumeration



```json
{
  "technicalstatus": "edgeMatched"
}
```

<blockquote class="lang-specific json">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/tests/bbr/template/TechnicalStatusValue/example_1_1.json">Open in new window</a>
    <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=json&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-Inspire-AdministrativeBoundary%2Fbuild%2Ftests%2Fbbr%2Ftemplate%2FTechnicalStatusValue%2Fexample_1_1.json&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on JSON Viewer</a></p>
</blockquote>



# JSON Schema

```yaml--schema
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

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-Inspire-AdministrativeBoundary%2Fbuild%2Fannotated%2Fbbr%2Ftemplate%2FTechnicalStatusValue%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/TechnicalStatusValue/schema.yaml" target="_blank">https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/TechnicalStatusValue/schema.yaml</a>
* JSON version: <a href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/TechnicalStatusValue/schema.json" target="_blank">https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/TechnicalStatusValue/schema.json</a>

# References

* [INSPIRE registry](https://inspire.ec.europa.eu/featureconcept/AdministrativeBoundary)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary" target="_blank">https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary</a>
* Path:
<code><a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/blob/HEAD/_sources/TechnicalStatusValue" target="_blank">_sources/TechnicalStatusValue</a></code>


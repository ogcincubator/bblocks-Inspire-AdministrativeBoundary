---
title: LegalStatusValue (Schema)


toc_footers:
  - Version 0.1
  - <a href='#'>LegalStatusValue</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: LegalStatusValue (Schema)
---


# LegalStatusValue `ogc.bbr.template.LegalStatusValue`

enumeration

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="success">
This building block is <strong><a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/blob/main/build/tests/bbr/template/LegalStatusValue/" target="_blank">valid</a></strong>
</aside>

# Description


## Enumeration LegalStatusValue
Description of the legal status of administrative boundaries.
## Values LegalStatusValue
| Status      | Description                                                                                   |
|-------------|-----------------------------------------------------------------------------------------------|
| agreed      | The edge-matched boundary has been agreed between neighbouring administrative units and is stable now |
| notAgreed   | The edge-matched boundary has not yet been agreed between neighbouring administrative units and could be changed |

# Examples

## Example of LegalStatusValue Enumeration



```json
{
  "legalstatus":  "agreed"
}


```

<blockquote class="lang-specific json">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/tests/bbr/template/LegalStatusValue/example_1_1.json">Open in new window</a>
    <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=json&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-Inspire-AdministrativeBoundary%2Fbuild%2Ftests%2Fbbr%2Ftemplate%2FLegalStatusValue%2Fexample_1_1.json&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on JSON Viewer</a></p>
</blockquote>



# JSON Schema

```yaml--schema
$schema: https://json-schema.org/draft/2020-12/schema
description: Schemas for LegalStatusValue
type: object
properties:
  legalstatus:
    description: Description of the legal status of administrative boundaries.
    type: string
    oneOf:
    - const: agreed
      descripcion: The edge-matched boundary has been agreed between neighbouring
        administrative units and is stable now
    - const: notAgreed
      descripcion: The edge-matched boundary has not yet been agreed between neighbouring
        administrative units and could be changed
required:
- legalstatus

```

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-Inspire-AdministrativeBoundary%2Fbuild%2Fannotated%2Fbbr%2Ftemplate%2FLegalStatusValue%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/LegalStatusValue/schema.yaml" target="_blank">https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/LegalStatusValue/schema.yaml</a>
* JSON version: <a href="https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/LegalStatusValue/schema.json" target="_blank">https://ogcincubator.github.io/bblocks-Inspire-AdministrativeBoundary/build/annotated/bbr/template/LegalStatusValue/schema.json</a>

# References

* [INSPIRE registry](https://inspire.ec.europa.eu/featureconcept/AdministrativeBoundary)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary" target="_blank">https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary</a>
* Path:
<code><a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/blob/HEAD/_sources/LegalStatusValue" target="_blank">_sources/LegalStatusValue</a></code>


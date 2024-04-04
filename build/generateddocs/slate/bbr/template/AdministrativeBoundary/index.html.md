---
title: AdministrativeBoundary (Schema)


toc_footers:
  - Version 0.1
  - <a href='#'>AdministrativeBoundary</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: AdministrativeBoundary (Schema)
---


# AdministrativeBoundary `ogc.bbr.template.AdministrativeBoundary`

Defines a specific interoperability profile of the AdministrativeBoundary dataset with the Inspire data model

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="success">
This building block is <strong><a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/blob/main/build/tests/bbr/template/AdministrativeBoundary/" target="_blank">valid</a></strong>
</aside>

# Description


## AdministrativeBoundary Inspire Data Model Profile for OGC API

This specification defines the specific requirements of the AdministrativeBoundary Information Model.
Administrative Boundary is defined like a line of demarcation between administrative units.

- [INSPIRE Administrative Boundary](https://inspire.ec.europa.eu/featureconcept/AdministrativeBoundary)
- [OGC-API IDE CATALONIA AdministrativeBoundary](https://geoserveis.ide.cat/servei/catalunya/inspire/ogc/features/collections/inspire:AU.AdministrativeBoundary/)

## Key features of this profile:
- a schema for the AdministrativeBoundary element with the Inspire data model
- a JSON-LD context for this result schema
- JSON-LD context elements defining namespaces for the values
# Examples

## Example of AdministrativeBoundary API



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

<blockquote class="lang-specific json">
  <p class="example-links">
    <a target="_blank" href="https://raw.githubusercontent.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/main/build/tests/bbr/template/AdministrativeBoundary/example_1_1.json">Open in new window</a>
    <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=json&amp;dataUrl=https%3A%2F%2Fraw.githubusercontent.com%2Fogcincubator%2Fbblocks-Inspire-AdministrativeBoundary%2Fmain%2Fbuild%2Ftests%2Fbbr%2Ftemplate%2FAdministrativeBoundary%2Fexample_1_1.json&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on JSON Viewer</a></p>
</blockquote>



# JSON Schema

```yaml--schema
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

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2Fraw.githubusercontent.com%2Fogcincubator%2Fbblocks-Inspire-AdministrativeBoundary%2Fmain%2Fbuild%2Fannotated%2Fbbr%2Ftemplate%2FAdministrativeBoundary%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://raw.githubusercontent.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/main/build/annotated/bbr/template/AdministrativeBoundary/schema.yaml" target="_blank">https://raw.githubusercontent.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/main/build/annotated/bbr/template/AdministrativeBoundary/schema.yaml</a>
* JSON version: <a href="https://raw.githubusercontent.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/main/build/annotated/bbr/template/AdministrativeBoundary/schema.json" target="_blank">https://raw.githubusercontent.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/main/build/annotated/bbr/template/AdministrativeBoundary/schema.json</a>

# References

* [INSPIRE registry](https://inspire.ec.europa.eu/featureconcept/AdministrativeBoundary)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary" target="_blank">https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary</a>
* Path:
<code><a href="https://github.com/ogcincubator/bblocks-Inspire-AdministrativeBoundary/blob/HEAD/_sources/AdministrativeBoundary" target="_blank">_sources/AdministrativeBoundary</a></code>


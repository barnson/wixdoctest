---
custom_edit_url: null
sidebar_position: 259
---
# SummaryInformation element
Properties about the package to be placed in the Summary Information Stream. These are visible from COM through the IStream interface, and these properties can be seen on the package in Explorer.

## Parents
[Package](package.md), [Module](module.md)

## Remarks
<p>You can specify any valid Windows code by by integer like 1252, or by web name like Windows-1252. See [Code pages](reference/codepage.md) for more information.</p>


## Attributes
**Codepage** (String)
  : The code page integer value or web name for summary info strings only. See remarks for more information.

**Description** (String)
  : The product full name or description.

**Keywords** (String)
  : Optional keywords for browsing.

**Manufacturer** (String)
  : The vendor releasing the package. Defaults to the Package/@Manufacturer attribute's value.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
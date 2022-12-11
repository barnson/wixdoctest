---
custom_edit_url: null
sidebar_position: 3
---
# WixLocalization element (Wxl extension)


## Children
* [String](string.md) 
* [UI](ui.md) 

## Remarks
<p>You can specify any valid Windows code page by integer like 1252, or by web name like Windows-1252 or iso-8859-1. See [Code pages](reference/codepage.md) for more information.</p>


## Attributes
**Codepage** (String)
  : Optional code page integer value or web name for the resulting database. You can also specify -1 which will not reset the database code page. See remarks for more information.

**Culture** (String)
  : Optional culture for this localization file. If the Culture attribute is not provided, the localization file is considered to be language neutral. This culture value is used to filter applicable localization files during the build. Language neutral localization files are always included.

**Language** (Integer)
  : The decimal language ID (LCID) for the culture. Used only when processed by native code using locutil.

**SummaryInformationCodepage** (String)
  : Optional code page integer value or web name for the resulting database's SummaryInformation. If not specified, the SummaryInformation codepage will be set to the same value from the Codepage attribute. If no codepage is provided, the SummaryInformation will default to the ANSI codepage. See remarks for more information.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wixloc.xsd)
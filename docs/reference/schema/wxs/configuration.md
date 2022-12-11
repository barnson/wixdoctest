---
custom_edit_url: null
sidebar_position: 44
---
# Configuration element
Defines the configurable attributes of merge module.

## Parents
[Module](module.md)

## Attributes
**ContextData** (String)
  : Specifies a semantic context for the requested data.

**DefaultValue** (String)
  : Specifies a default value for the item in this record if the merge tool declines to provide a value.

**Description** (String)
  : Description for authoring.

**DisplayName** (String)
  : Display name for authoring.

**Format** (enumeration, required)
  : Specifies the format of the data being changed. This attribute's value must be one of the following:
- *Text*
- *Key*
- *Integer*
- *Bitfield*

**HelpKeyword** (String)
  : Keyword into chm file for authoring.

**HelpLocation** (String)
  : Location of chm file for authoring.

**KeyNoOrphan** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Does not merge rule according to rules in MSI SDK.

**Name** (String, required)
  : Defines the name of the configurable item.

**NonNullable** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : If yes, null is not a valid entry.

**Type** (String)
  : Specifies the type of the data being changed.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
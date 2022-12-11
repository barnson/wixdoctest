---
custom_edit_url: null
sidebar_position: 282
---
# UpgradeFile element
Specifies files to either ignore or to specify optional data about a file.

## Parents
[UpgradeImage](upgradeimage.md)

## Children
* [SymbolPath](symbolpath.md) 

## Attributes
**AllowIgnoreOnError** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether patching this file is vital.

**File** (String, required)
  : Foreign key into the File table.

**Ignore** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'), required)
  : If yes, the file is ignored during patching, and the next two attributes are ignored.

**WholeFile** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Whether the whole file should be installed, rather than creating a binary patch.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
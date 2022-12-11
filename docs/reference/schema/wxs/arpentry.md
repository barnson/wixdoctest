---
custom_edit_url: null
sidebar_position: 10
---
# ArpEntry element
Information about the Add/Remove Programs entry that is installed by the package. ArpEntry may not be specified with DetectCondition or UninstallArguments.

## Parents
[ExePackage](exepackage.md)

## Attributes
**Id** (String, required)
  : The id of the ARP entry.

**Version** (String, required)
  : The DisplayVersion value of the ARP entry that is installed by this package. Older or missing versions cause this package to be detected as absent. Newer versions cause this package to be detected as obsolete.

**Win64** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'), required)
  : Whether the ARP entry is 64-bit.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
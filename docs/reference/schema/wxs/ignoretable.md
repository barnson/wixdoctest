---
custom_edit_url: null
sidebar_position: 106
---
# IgnoreTable element
Specifies a table from the merge module that is not merged into an .msi file. If the table already exists in an .msi file, it is not modified by the merge. The specified table can therefore contain data that is unneeded after the merge. To minimize the size of the .msm file, it is recommended that developers remove unused tables from modules intended for redistribution rather than creating IgnoreTable elements for those tables.

## Parents
[Module](module.md)

## Attributes
**Id** (String, required)
  : The name of the table in the merge module that is not to be merged into the .msi file.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
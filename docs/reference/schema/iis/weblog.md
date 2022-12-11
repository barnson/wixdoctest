---
custom_edit_url: null
sidebar_position: 14
---
# WebLog element (Iis extension)
WebLog definition.

## Parents
[Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md)

## Attributes
**Id** (String, required)
  : Identifier for the WebLog.

**Type** (enumeration, required)
  :  This attribute's value must be one of the following:
- *IIS*: Microsoft IIS Log File Format
- *NCSA*: NCSA Common Log File Format
- *none*: Disables logging.
- *ODBC*: ODBC Logging
- *W3C*: W3C Extended Log File Format


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)
---
custom_edit_url: null
sidebar_position: 43
---
# XmlConfig element (Util extension)
Adds or removes .xml file entries. If you use the XmlConfig element you must reference WixUtilExtension.dll as it contains the XmlConfig custom actions.

## Parents
[Component](../wxs/component.md), [XmlConfig](xmlconfig.md)

## Children
* [XmlConfig](xmlconfig.md) 

## Attributes
**Action** (enumeration)
  :  This attribute's value must be one of the following:
- *create*
- *delete*

**ElementId** (String)
  : The Id of another XmlConfig to add attributes to.  In this case, the 'ElementPath', 'Action', 'Node', and 'On' attributes must be omitted.

**ElementPath** (String)
  : The XPath of the parent element being modified.  Note that this is a formatted field and therefore, square brackets in the XPath must be escaped. In addition, XPaths allow backslashes to be used to escape characters, so if you intend to include literal backslashes, you must escape them as well by doubling them in this attribute. The string is formatted by MSI first, and the result is consumed as the XPath.

**File** (String, required)
  : Path of the .xml file to configure.

**Id** (String)
  : Identifier for xml file modification.

**Name** (String)
  : Name of XML node to set/add to the specified element.  Not setting this attribute causes the element's text value to be set.  Otherwise this specified the attribute name that is set.

**Node** (enumeration)
  :  This attribute's value must be one of the following:
- *element*
- *value*
- *document*

**On** (enumeration)
  :  This attribute's value must be one of the following:
- *install*
- *uninstall*

**PreserveModifiedDate** (wxs:YesNoTypeUnion)
  : Specifies wheter or not the modification should preserve the modified date.  Preserving the modified date will allow the file to be patched if no other modifications have been made.

**Sequence** (Integer)
  : Specifies the order in which the modification is to be attempted on the XML file.  It is important to ensure that new elements are created before you attempt to add an attribute to them.

**Value** (String)
  : The value to be written.  See the Formatted topic for information how to escape square brackets in the value.

**VerifyPath** (String)
  : The XPath to the element being modified.  This is required for 'delete' actions.  For 'create' actions, VerifyPath is used to decide if the element already exists. Note that this is a formatted field and therefore, square brackets in the XPath must be escaped. In addition, XPaths allow backslashes to be used to escape characters, so if you intend to include literal backslashes, you must escape them as well by doubling them in this attribute. The string is formatted by MSI first, and the result is consumed as the XPath.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)
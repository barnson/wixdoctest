---
custom_edit_url: null
sidebar_position: 44
---
# XmlFile element (Util extension)
Adds or removes .xml file entries.  If you use the XmlFile element you must reference WixUtilExtension.dll as it contains the XmlFile custom actions.

## Parents
[Component](../wxs/component.md)

## Attributes
**Action** (enumeration, required)
  : The type of modification to be made to the XML file when the component is installed. This attribute's value must be one of the following:
- *createElement*: Creates a new element under the element specified in ElementPath.  The Name attribute is required in this case and specifies the name of the new element.  The Value attribute is not necessary when createElement is specified as the action.  If the Value attribute is set, it will cause the new element's text value to be set.
- *deleteValue*: Deletes a value from the element specified in the ElementPath.  If Name is specified, the attribute with that name is deleted.  If Name is not specified, the text value of the element specified in the ElementPath is deleted.  The Value attribute is ignored if deleteValue is the action specified.
- *setValue*: Sets a value in the element specified in the ElementPath.  If Name is specified, and attribute with that name is set to the value specified in Value.  If Name is not specified, the text value of the element is set.  Value is a required attribute if setValue is the action specified.
- *bulkSetValue*: Sets all the values in the elements that match the ElementPath.  If Name is specified, attributes with that name are set to the same value specified in Value.  If Name is not specified, the text values of the elements are set.  Value is a required attribute if setBulkValue is the action specified.

**ElementPath** (String, required)
  : The XPath of the element to be modified.  Note that this is a formatted field and therefore, square brackets in the XPath must be escaped. In addition, XPaths allow backslashes to be used to escape characters, so if you intend to include literal backslashes, you must escape them as well by doubling them in this attribute. The string is formatted by MSI first, and the result is consumed as the XPath.

**File** (String, required)
  : Path of the .xml file to configure.

**Id** (String)
  : Identifier for xml file modification.

**Name** (String)
  : Name of XML node to set/add to the specified element.  Not setting this attribute causes the element's text value to be set.  Otherwise this specified the attribute name that is set.

**Permanent** (wxs:YesNoTypeUnion)
  : Specifies whether or not the modification should be removed on uninstall.  This has no effect on uninstall if the action was deleteValue.

**PreserveModifiedDate** (wxs:YesNoTypeUnion)
  : Specifies wheter or not the modification should preserve the modified date.  Preserving the modified date will allow the file to be patched if no other modifications have been made.

**SelectionLanguage** (enumeration)
  : Specify whether the DOM object should use XPath language or the old XSLPattern language (default) as the query language. This attribute's value must be one of the following:
- *XPath*
- *XSLPattern*

**Sequence** (Integer)
  : Specifies the order in which the modification is to be attempted on the XML file.  It is important to ensure that new elements are created before you attempt to add an attribute to them.

**Value** (String)
  : The value to be written.  See the Formatted topic for information how to escape square brackets in the value.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)
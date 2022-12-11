---
custom_edit_url: null
sidebar_position: 9
---
# ComPlusMethod element (Complus extension)
Represents a method for an interface.

## Parents
[ComPlusInterface](complusinterface.md)

## Children
* [ComPlusRoleForMethod](complusroleformethod.md) 

## Attributes
**AutoComplete** (wxs:YesNoTypeUnion)
  : 

**Description** (String)
  : 

**Id** (String, required)
  : Identifier for the element.

**Index** (xs:int)
  : Dispatch id of the method. If this attribute is not set a value must be provided for the Name attribute.

**Name** (String)
  : Name of the method. If this attribute is not set a value must be provided for the Index attribute.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)
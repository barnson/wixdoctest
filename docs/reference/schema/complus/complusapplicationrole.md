---
custom_edit_url: null
sidebar_position: 2
---
# ComPlusApplicationRole element (Complus extension)
Defines an application role. If this element is a descendent of a Component element, the application role will be created in association with this component. If the element is a child of any of the Fragment, Module, or Package elements it is considered to be a locater, referencing an existing application role.

## Parents
[Component](../wxs/component.md), [Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md), [ComPlusApplication](complusapplication.md)

## Children
* [ComPlusGroupInApplicationRole](complusgroupinapplicationrole.md) 
* [ComPlusUserInApplicationRole](complususerinapplicationrole.md) 

## Attributes
**Application** (String)
  : If the element is not a child of a ComPlusApplication element, this attribute should be provided with the id of a ComPlusApplication element representing the application the role belongs to.

**Description** (String)
  : 

**Id** (String, required)
  : Identifier for the element.

**Name** (String, required)
  : Name of the application role.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)
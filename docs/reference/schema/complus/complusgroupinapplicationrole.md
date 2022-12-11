---
custom_edit_url: null
sidebar_position: 6
---
# ComPlusGroupInApplicationRole element (Complus extension)
This element represents a security group membership in an application role. When the parent component of this element is installed, the user will be added to the associated application role. This element must be a descendent of a Component element; it can not be a child of a ComPlusApplicationRole locater element. To reference a locater element use the ApplicationRole attribute.

## Parents
[Component](../wxs/component.md), [ComPlusApplicationRole](complusapplicationrole.md)

## Attributes
**ApplicationRole** (String)
  : If the element is not a child of a ComPlusApplicationRole element, this attribute should be provided with the id of a ComPlusApplicationRole element representing the application role the user is to be added to.

**Group** (String, required)
  : Foreign key into the Group table.

**Id** (String, required)
  : Identifier for the element.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)
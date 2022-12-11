---
custom_edit_url: null
sidebar_position: 15
---
# ComPlusRoleForMethod element (Complus extension)
Represents a role assignment to a COM+ method.

## Parents
[Component](../wxs/component.md), [ComPlusMethod](complusmethod.md)

## Attributes
**ApplicationRole** (String, required)
  : Id of the ComPlusApplicationRole element representing the role that shall be granted access to the method.

**Id** (String, required)
  : Identifier for the element.

**Method** (String)
  : If the element is not a child of a ComPlusMethod element, this attribute should be provided with the id of a ComPlusMethod element representing the method the role is to be added to.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)
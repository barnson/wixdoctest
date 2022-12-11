---
custom_edit_url: null
sidebar_position: 13
---
# ComPlusRoleForComponent element (Complus extension)
Represents a role assignment to a COM+ component.

## Parents
[Component](../wxs/component.md), [ComPlusComponent](compluscomponent.md)

## Attributes
**ApplicationRole** (String, required)
  : Id of the ComPlusApplicationRole element representing the role that shall be granted access to the component.

**Component** (String)
  : If the element is not a child of a ComPlusComponent element, this attribute should be provided with the id of a ComPlusComponent element representing the component the role is to be added to.

**Id** (String, required)
  : Identifier for the element.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)
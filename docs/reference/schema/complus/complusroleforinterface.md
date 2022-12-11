---
custom_edit_url: null
sidebar_position: 14
---
# ComPlusRoleForInterface element (Complus extension)
Represents a role assignment to an interface.

## Parents
[Component](../wxs/component.md), [ComPlusInterface](complusinterface.md)

## Attributes
**ApplicationRole** (String, required)
  : Id of the ComPlusApplicationRole element representing the role that shall be granted access to the interface.

**Id** (String, required)
  : Identifier for the element.

**Interface** (String)
  : If the element is not a child of a ComPlusInterface element, this attribute should be provided with the id of a ComPlusInterface element representing the interface the role is to be added to.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)
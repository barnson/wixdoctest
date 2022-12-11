---
custom_edit_url: null
sidebar_position: 188
---
# Publish element


## Windows Installer references
[ControlEvent Table](https://docs.microsoft.com/en-us/windows/win32/msi/controlevent-table)

## Parents
[Control](control.md), [UI](ui.md)

## Attributes
**Control** (String)
  : The parent Control for this Publish element, should only be specified when this element is a child of the UI element.

**Dialog** (String)
  : The parent Dialog for this Publish element, should only be specified when this element is a child of the UI element. This attribute will create a reference to the specified Dialog, so an additional DialogRef is not necessary.

**Event** (String)
  : Set this attribute's value to one of the standard control events to trigger that event. Either this attribute or the Property attribute must be set, but not both at the same time.

**Order** (String)
  : This attribute should only need to be set if this element is nested under a UI element in order to control the order in which this publish event will be started. If this element is nested under a Control element, the default value will be one greater than any previous Publish element's order (the first element's default value is 1). If this element is nested under a UI element, the default value is always 1 (it does not get a default value based on any previous Publish elements).

**Property** (String)
  : Set this attribute's value to a property name to set that property. Either this attribute or the Event attribute must be set, but not both at the same time.

**Value** (String)
  : If the Property attribute is specified, set the value of this attribute to the new value for the property. To set a property to null, do not set this attribute (the ControlEvent Argument column will be set to '{}'). Otherwise, this attribute's value should be the argument for the event specified in the Event attribute. If the event doesn't take an attribute, a common value to use is "0".


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
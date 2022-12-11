---
custom_edit_url: null
sidebar_position: 35
---
# RestartResource element (Util extension)
Registers a resource with the Restart Manager.

## Parents
[Component](../wxs/component.md), [Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md)

## Attributes
**Id** (String)
  : The unique identifier for this resource. A unique identifier will be generated automatically if not specified.

**Path** (String)
  : The full path to the process module to register with the Restart Manager. This can be a formatted value that resolves to a full path.

**ProcessName** (String)
  : The name of a process to register with the Restart Manager. This can be a formatted value that resolves to a process name.

**ServiceName** (String)
  : The name of a Windows service to register with the Restart Manager. This can be a formatted value that resolves to a service name.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)
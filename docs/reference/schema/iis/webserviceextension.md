---
custom_edit_url: null
sidebar_position: 16
---
# WebServiceExtension element (Iis extension)
The WebServiceExtension property is used by the Web server to determine whether a Web service extension is permitted to run.

## Parents
[Component](../wxs/component.md)

## Attributes
**Allow** (wxs:YesNoTypeUnion, required)
  : Indicates if the extension is allowed or denied.

**Description** (String)
  : Description of the extension.

**File** (String, required)
  : Usually a Property that resolves to short file name path

**Group** (String)
  : String used to identify groups of extensions.

**Id** (String)
  : Identifier for the web service extension. Used within the MSI package only. If the Id is not specified, it will be generated.

**UIDeletable** (wxs:YesNoTypeUnion)
  : Indicates if the UI is allowed to delete the extension from the list of not.  Default: Not deletable.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)
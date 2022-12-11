---
custom_edit_url: null
sidebar_position: 20
---
# InternetShortcut element (Util extension)
Creates a shortcut to a URL.

## Parents
[Component](../wxs/component.md)

## Attributes
**Directory** (String)
  : Identifier reference to Directory element where shortcut is to be created. This attribute's value defaults to the parent Component directory.

**IconFile** (String)
  : Icon file that should be displayed. Note that this is a formatted field, so you can use [#fileId] syntax to refer to a file being installed (using the file: protocol).

**IconIndex** (Integer)
  : Index of the icon being referenced.

**Id** (String)
  : Unique identifier in your installation package for this Internet shortcut.

**Name** (String, required)
  : The name of the shortcut file, which is visible to the user. (The .lnk extension is added automatically and by default, is not shown to the user.)

**Target** (String, required)
  : URL that should be opened when the user selects the shortcut. Windows opens the URL in the appropriate handler for the protocol specified in the URL. Note that this is a formatted field, so you can use [#fileId] syntax to refer to a file being installed (using the file: protocol).

**Type** (enumeration)
  : Which type of shortcut should be created. This attribute's value must be one of the following:
- *url*: Creates .url files using IUniformResourceLocatorW.
- *link*: Creates .lnk files using IShellLinkW (default).


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)
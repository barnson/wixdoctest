---
custom_edit_url: null
sidebar_position: 64
---
# Dialog element
Defines a dialog box in the Dialog Table.

## Windows Installer references
[Control Table](https://docs.microsoft.com/en-us/windows/win32/msi/control-table), [ComboBox Table](https://docs.microsoft.com/en-us/windows/win32/msi/combobox-table), [Dialog Table](https://docs.microsoft.com/en-us/windows/win32/msi/dialog-table), [ListBox Table](https://docs.microsoft.com/en-us/windows/win32/msi/listbox-table), [ListView Table](https://docs.microsoft.com/en-us/windows/win32/msi/listview-table), [RadioButton Table](https://docs.microsoft.com/en-us/windows/win32/msi/radiobutton-table)

## Parents
[UI](ui.md)

## Children
* [Control](control.md) : Control elements belonging to this dialog.

## Attributes
**CustomPalette** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Used to specify if pictures in the dialog box are rendered with a custom palette.

**ErrorDialog** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies this dialog as an error dialog.

**Height** (Integer, required)
  : The height of the dialog box in dialog units.

**Hidden** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Used to hide the dialog.

**Id** (String, required)
  : Unique identifier for the dialog.

**KeepModeless** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Keep modeless dialogs alive when this dialog is created through DoAction.

**LeftScroll** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Used to align the scroll bar on the left.

**Modeless** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Used to set the dialog as modeless.

**NoMinimize** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Used to specify if the dialog can be minimized.

**RightAligned** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Align text on the right.

**RightToLeft** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Used to specify if the text in the dialog should be displayed in right to left reading order.

**SystemModal** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Used to set the dialog as system modal.

**Title** (String)
  : The title of the dialog box.

**TrackDiskSpace** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Have the dialog periodically call the installer to check if available disk space has changed.

**Width** (Integer, required)
  : The width of the dialog box in dialog units.

**X** (Integer)
  : Horizontal placement of the dialog box as a percentage of screen width. The default value is 50.

**Y** (Integer)
  : Vertical placement of the dialog box as a percentage of screen height. The default value is 50.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
---
custom_edit_url: null
sidebar_position: 130
---
# ListItem element
The value (and optional text) associated with an item in a ComboBox, ListBox, or ListView.

## Windows Installer references
[ComboBox Table](https://docs.microsoft.com/en-us/windows/win32/msi/combobox-table), [ListBox Table](https://docs.microsoft.com/en-us/windows/win32/msi/listbox-table), [ListView Table](https://docs.microsoft.com/en-us/windows/win32/msi/listview-table)

## Parents
[ListBox](listbox.md), [ComboBox](combobox.md), [ListView](listview.md)

## Attributes
**Icon** (String)
  : The identifier of the Binary (not Icon) element containing the icon to associate with this item. This value is only valid when nested under a ListView element.

**Text** (String)
  : The localizable, visible text to be assigned to the item. If not specified, this will default to the value of the Value attribute.

**Value** (String, required)
  : The value assigned to the associated ComboBox, ListBox, or ListView property if this item is selected.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
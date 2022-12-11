---
custom_edit_url: null
sidebar_position: 192
---
# RadioButton element
Text or Icon plus Value that is assigned to the Property of the parent Control (RadioButtonGroup).

## Windows Installer references
[RadioButton Table](https://docs.microsoft.com/en-us/windows/win32/msi/radiobutton-table), [Control Table](https://docs.microsoft.com/en-us/windows/win32/msi/control-table), [Dialog Table](https://docs.microsoft.com/en-us/windows/win32/msi/dialog-table)

## Parents
[RadioButtonGroup](radiobuttongroup.md)

## Attributes
**Bitmap** (String)
  : This attribute defines the bitmap displayed with the radio button. The value of the attribute creates a reference to a Binary element that represents the bitmap. This attribute is mutually exclusive with the Icon and Text attributes.

**Height** ([LocalizableInteger](localizableinteger.md 'Values of this type must be an integer or a localization variable with the format `!(loc.Variable)` where `Variable` is the name of the localization variable.'), required)
  : 

**Help** (String)
  : 

**Icon** (String)
  : This attribute defines the icon displayed with the radio button. The value of the attribute creates a reference to a Binary element that represents the icon. This attribute is mutually exclusive with the Bitmap and Text attributes.

**Text** (String)
  : Text displayed with the radio button. This attribute is mutually exclusive with the Bitmap and Icon attributes.

**ToolTip** (String)
  : 

**Value** (String, required)
  : Value assigned to the associated control Property when this radio button is selected.

**Width** ([LocalizableInteger](localizableinteger.md 'Values of this type must be an integer or a localization variable with the format `!(loc.Variable)` where `Variable` is the name of the localization variable.'), required)
  : 

**X** ([LocalizableInteger](localizableinteger.md 'Values of this type must be an integer or a localization variable with the format `!(loc.Variable)` where `Variable` is the name of the localization variable.'), required)
  : 

**Y** ([LocalizableInteger](localizableinteger.md 'Values of this type must be an integer or a localization variable with the format `!(loc.Variable)` where `Variable` is the name of the localization variable.'), required)
  : 


## See also
[RadioButtonGroup](radiobuttongroup.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
---
custom_edit_url: null
sidebar_position: 48
---
# Control element
Contains the controls that appear on each dialog.

## Windows Installer references
[Control Table](https://docs.microsoft.com/en-us/windows/win32/msi/control-table), [ComboBox Table](https://docs.microsoft.com/en-us/windows/win32/msi/combobox-table), [Dialog Table](https://docs.microsoft.com/en-us/windows/win32/msi/dialog-table), [ListBox Table](https://docs.microsoft.com/en-us/windows/win32/msi/listbox-table), [ListView Table](https://docs.microsoft.com/en-us/windows/win32/msi/listview-table), [RadioButton Table](https://docs.microsoft.com/en-us/windows/win32/msi/radiobutton-table)

## Parents
[Billboard](billboard.md), [Dialog](dialog.md)

## Children
* [Binary](binary.md) (no more than 1) : Icon referenced in icon column of row
* [ComboBox](combobox.md) 
* [ListBox](listbox.md) 
* [ListView](listview.md) 
* [Property](property.md) (no more than 1) : Property table entry for the Property table column associated with this control
* [Publish](publish.md) 
* [RadioButtonGroup](radiobuttongroup.md) 
* [Subscribe](subscribe.md) 
* [Text](text.md) (no more than 1) : alternative to Text attribute when CDATA is needed to escape XML delimiters

## Attributes
**Bitmap** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for RadioButton and PushButton Controls.

**Cancel** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to "yes" to cause this Control to be invoked by the escape key.

**CDROM** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Volume and Directory Controls.

**CheckBoxPropertyRef** (String)
  : This attribute is only valid for CheckBox controls. The value is the name of a Property that was already used as the Property for another CheckBox control. The Property attribute cannot be specified. The attribute exists to support multiple checkboxes on different dialogs being tied to the same property.

**CheckBoxValue** (String)
  : This attribute is only valid for CheckBox Controls. When set, the linked Property will be set to this value when the check box is checked.

**ComboList** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for ComboBox Controls.

**Default** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to "yes" to cause this Control to be invoked by the return key.

**DefaultCondition** ()
  : When the condition expression evaluates to true, set the Control as the default.

**DisableCondition** ()
  : When the condition expression evaluates to true, disable the Control.

**Disabled** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to "yes" to cause the Control to be disabled.

**ElevationShield** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for PushButton controls. Set this attribute to "yes" to add the User Account Control (UAC) elevation icon (shield icon) to the PushButton control. If this attribute's value is "yes" and the installation is not yet running with elevated privileges, the pushbutton control is created using the User Account Control (UAC) elevation icon (shield icon). If this attribute's value is "yes" and the installation is already running with elevated privileges, the pushbutton control is created using the other icon attributes. Otherwise, the pushbutton control is created using the other icon attributes.

**EnableCondition** ()
  : When the condition expression evaluates to true, enable the Control.

**Fixed** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Volume and Directory Controls.

**FixedSize** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for RadioButton, PushButton, and Icon Controls.

**Floppy** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Volume and Directory Controls.

**FormatSize** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Text Controls.

**HasBorder** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for RadioButton Controls.

**Height** ([LocalizableInteger](localizableinteger.md 'Values of this type must be an integer or a localization variable with the format `!(loc.Variable)` where `Variable` is the name of the localization variable.'), required)
  : Height of the rectangular boundary of the control. This must be a non-negative number.

**Help** (String)
  : This attribute is reserved for future use. There is no need to use this until Windows Installer uses it for something.

**Hidden** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to "yes" to cause the Control to be hidden.

**HideCondition** ()
  : When the condition expression evaluates to true, hide the Control.

**Icon** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for RadioButton and PushButton Controls.

**IconSize** (enumeration)
  : This attribute is only valid for RadioButton, PushButton, and Icon Controls. This attribute's value must be one of the following:
- *16*
- *32*
- *48*

**Id** (String, required)
  : Combined with the Dialog Id to make up the primary key of the Control table.

**Image** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for RadioButton, PushButton, and Icon Controls.

**Indirect** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether the value displayed or changed by this control is referenced indirectly. If this bit is set, the control displays or changes the value of the property that has the identifier listed in the Property column of the Control table.

**Integer** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to "yes" to cause the linked Property value for the Control to be treated as an integer. Otherwise, the Property will be treated as a string.

**LeftScroll** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to "yes" to cause the scroll bar to display on the left side of the Control.

**Multiline** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Edit Controls.

**NoPrefix** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Text Controls.

**NoWrap** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Text Controls.

**Password** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Edit Controls.

**ProgressBlocks** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for ProgressBar Controls.

**Property** (String)
  : The name of a defined property to be linked to this control. This column is required for active controls.

**PushLike** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for RadioButton and Checkbox Controls.

**RAMDisk** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Volume and Directory Controls.

**Remote** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Volume and Directory Controls.

**Removable** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Volume and Directory Controls.

**RightAligned** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to "yes" to cause the Control to be right aligned.

**RightToLeft** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to "yes" to cause the Control to display from right to left.

**ShowCondition** ()
  : When the condition expression evaluates to true, show the Control.

**ShowRollbackCost** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for VolumeCostList Controls.

**Sorted** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for ListBox, ListView, and ComboBox Controls. Set the value of this attribute to "yes" to have entries appear in the order specified under the Control. If the attribute value is "no" or absent the entries in the control will appear in alphabetical order.

**Sunken** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to "yes" to cause the Control to be sunken.

**TabSkip** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute to "yes" to cause this Control to be skipped in the tab sequence.

**Text** (String)
  : A localizable string used to set the initial text contained in a control. This attribute can contain a formatted string that is processed at install time to insert the values of properties using [PropertyName] syntax. Also supported are environment variables, file installation paths, and component installation directories; see Formatted for details.

**ToolTip** (String)
  : The string used for the Tooltip.

**Transparent** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Text Controls.

**Type** (String, required)
  : The type of the control. Could be one of the following: Billboard, Bitmap, CheckBox, ComboBox, DirectoryCombo, DirectoryList, Edit, GroupBox, Hyperlink, Icon, Line, ListBox, ListView, MaskedEdit, PathEdit, ProgressBar, PushButton, RadioButtonGroup, ScrollableText, SelectionTree, Text, VolumeCostList, VolumeSelectCombo

**UserLanguage** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : This attribute is only valid for Text Controls.

**Width** ([LocalizableInteger](localizableinteger.md 'Values of this type must be an integer or a localization variable with the format `!(loc.Variable)` where `Variable` is the name of the localization variable.'), required)
  : Width of the rectangular boundary of the control. This must be a non-negative number.

**X** ([LocalizableInteger](localizableinteger.md 'Values of this type must be an integer or a localization variable with the format `!(loc.Variable)` where `Variable` is the name of the localization variable.'), required)
  : Horizontal coordinate of the upper-left corner of the rectangular boundary of the control. This must be a non-negative number.

**Y** ([LocalizableInteger](localizableinteger.md 'Values of this type must be an integer or a localization variable with the format `!(loc.Variable)` where `Variable` is the name of the localization variable.'), required)
  : Vertical coordinate of the upper-left corner of the rectangular boundary of the control. This must be a non-negative number.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
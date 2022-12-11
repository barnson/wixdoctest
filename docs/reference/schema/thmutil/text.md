---
custom_edit_url: null
sidebar_position: 36
---
# Text element (Thmutil extension)
Defines text for the parent control based on an optional condition. If multiple Text elements are given for one control, the conditions should be mutually exclusive (when multiple conditions are true, the behavior is undefined and may be changed at any time). If none of the conditions of a control's Text elements are true, then it uses the text of the Text element without the Condition attribute.

## Parents
[Button](button.md), [Checkbox](checkbox.md), [CommandLink](commandlink.md), [Hyperlink](hyperlink.md), [Hypertext](hypertext.md), [Label](label.md), [RadioButton](radiobutton.md), [Richedit](richedit.md)

## Attributes
**Condition** (String)
  : The condition that determines when the parent control will use this text.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/thmutil.xsd)
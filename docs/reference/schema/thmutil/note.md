---
custom_edit_url: null
sidebar_position: 25
---
# Note element (Thmutil extension)
Defines note text for a command link control based on an optional condition. If multiple Note elements are given for one control, the conditions should be mutually exclusive (when multiple conditions are true, the behavior is undefined and may be changed at any time). If none of the conditions of a control's Note elements are true, then it uses the text of the Note element without the Condition attribute.

## Parents
[CommandLink](commandlink.md)

## Attributes
**Condition** (String)
  : The condition that determines when the parent control will use this note text.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/thmutil.xsd)
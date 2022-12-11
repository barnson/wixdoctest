---
custom_edit_url: null
sidebar_position: 9
---
# ChangePageAction element (Thmutil extension)
When the button is pressed, the specified page is shown.

## Parents
[Button](button.md), [CommandLink](commandlink.md)

## Attributes
**Cancel** (enumeration)
  : When set to 'yes', none of the variable changes made on the current page are saved. This attribute's value must be one of the following:
- *no*
- *yes*

**Condition** (String)
  : The condition that determines if the parent control will execute this action.

**Page** (String, required)
  : The Name of the Page to show.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/thmutil.xsd)
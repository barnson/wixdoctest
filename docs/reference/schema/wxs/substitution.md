---
custom_edit_url: null
sidebar_position: 258
---
# Substitution element
Specifies the configurable fields of a module database and provides a template for the configuration of each field.

## Parents
[Module](module.md)

## Attributes
**Column** (String, required)
  : Specifies the target column in the row named in the Row column.

**Row** (String, required)
  : Specifies the primary keys of the target row in the table named in the Table column. If multiple keys, separated by semicolons.

**Table** (String, required)
  : Specifies the name of the table being modified in the module database.

**Value** (String)
  : Provides a formatting template for the data being substituted into the target field specified by Table, Row, and Column.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
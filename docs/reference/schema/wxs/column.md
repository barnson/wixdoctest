---
custom_edit_url: null
sidebar_position: 34
---
# Column element
Column definition for a Custom Table

## Parents
[CustomTable](customtable.md)

## Attributes
**Category** (enumeration)
  : Category of this column. This attribute must be specified with a value of 'Binary' if the Type attribute's value is 'binary'. This attribute's value must be one of the following:
- *text*
- *upperCase*
- *lowerCase*
- *integer*
- *doubleInteger*
- *timeDate*
- *identifier*
- *property*
- *filename*
- *wildCardFilename*
- *path*
- *paths*
- *anyPath*
- *defaultDir*
- *regPath*
- *formatted*
- *formattedSddl*
- *template*
- *condition*
- *guid*
- *version*
- *language*
- *binary*
- *customSource*
- *cabinet*
- *shortcut*

**Description** (String)
  : Description of this column.

**Id** (String, required)
  : Identifier for the column.

**KeyColumn** (Integer)
  : Column in the table in KeyTable attribute.

**KeyTable** (String)
  : Table in which this column is an external key. Can be semicolon delimited.

**Localizable** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Whether this column can be localized.

**MaxValue** (xs:long)
  : Maximum value for a numeric value, date or version in this column.

**MinValue** (xs:long)
  : Minimum value for a numeric value, date or version in this column.

**Modularize** (enumeration)
  : How this column should be modularized, if at all. This attribute's value must be one of the following:
- *none*: Column should not be modularized. This is the default value.
- *column*: Column should be modularized.
- *condition*: Column is a condition and should be modularized.
- *icon*: When the column is an primary or foreign key to the Icon table it should be modularized special.
- *property*: Any Properties in the column should be modularized.
- *semicolonDelimited*: Semi-colon list of keys, all of which need to be modularized.

**Nullable** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Whether this column can be left null.

**PrimaryKey** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Whether this column is a primary key.

**Set** (String)
  : Semicolon delimited list of permissible values.

**Type** (enumeration, required)
  : The type of this column. This attribute's value must be one of the following:
- *binary*: Column contains a path to a file that will be inserted into the column as a binary object. If this value is set, the Category attribute must also be set with a value of 'Binary' to pass ICE validation.
- *int*: Column contains an integer or datetime value (the MinValue and MaxValue attributes should also be set).
- *string*: Column contains a non-localizable string value.

**Width** (Integer)
  : Width of this column.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
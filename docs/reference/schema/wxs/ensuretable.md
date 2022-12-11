---
custom_edit_url: null
sidebar_position: 79
---
# EnsureTable element
Use this element to ensure that a table appears in the installer database, even if its empty.

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md)

## Remarks
This element is particularly useful for two problems that may occur while merging merge modules:
<ol><li>
        The first likely problem is that in order to properly merge you need to have certain
        tables present prior to merging. Using this element is one way to ensure those tables
        are present prior to the merging.
    </li><li>
        The other common problem is that a merge module has incorrect validation information
        about some tables. By ensuring these tables prior to merging, you can avoid this
        problem because the correct validation information will go into the installer database
        before the merge module has a chance to set it incorrectly.
    </li></ol>

## Attributes
**Id** (String, required)
  : The name of the table.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
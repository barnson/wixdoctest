---
custom_edit_url: null
sidebar_position: 13
---
# WebFilter element (Iis extension)
IIs Filter for a Component or Web Site

## Parents
[Component](../wxs/component.md), [WebSite](website.md)

## Attributes
**Description** (String)
  : Description of the filter.

**Flags** (Integer)
  : Sets the MD_FILTER_FLAGS metabase key for the filter. This must be an integer. See MSDN 'FilterFlags' documentation for more details.

**Id** (String)
  : The unique Id for the web filter. If the Id is not specified, it will be generated.

**LoadOrder** (String)
  : The legal values are "first", "last", or a number. If a number is specified, it must be greater than 0.

**Name** (String, required)
  : The name of the filter to be used in IIS.

**Path** (String, required)
  : The path of the filter executable file. This should usually be a value like '[!FileId]', where 'FileId' is the file identifier of the filter executable file.

**WebSite** (String)
  : Specifies the parent website for this filter (if there is one). If this is a global filter, then this attribute should not be specified.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)
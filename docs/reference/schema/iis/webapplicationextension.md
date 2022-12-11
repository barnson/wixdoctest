---
custom_edit_url: null
sidebar_position: 8
---
# WebApplicationExtension element (Iis extension)
Extension for WebApplication

## Parents
[WebApplication](webapplication.md)

## Attributes
**CheckPath** (wxs:YesNoTypeUnion)
  : 

**Executable** (String, required)
  : Usually a Property that resolves to short file name path.

**Extension** (String)
  : Extension being registered. Do not prefix with a '.' (e.g. you should use "html", not ".html"). To register for all extensions, use Extension="*". To register a wildcard application map (which handles all requests, even those for directories or files with no extension) omit the Extension attribute completely.

**Script** (wxs:YesNoTypeUnion)
  : 

**Verbs** (String)
  : 


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)
---
custom_edit_url: null
sidebar_position: 3
---
# DotNetCoreSearch element (Netfx extension)
Searches for the specified .NET installed on the computer.

## Parents
[Bundle](../wxs/bundle.md), [Fragment](../wxs/fragment.md)

## Attributes
**After** (String)
  : Id of the search that this one should come after.

**Condition** (String)
  : Condition for evaluating the search. If this evaluates to false, the search is not executed at all.

**Id** (String)
  : Identifier for the search. If the Id is not specified, one will be generated.

**MajorVersion** (Integer)
  : Major version of .NET. For example, "6".

**Platform** (enumeration)
  : The platform to search for. This attribute's value must be one of the following:
- *arm64*
- *x64*
- *x86*

**RuntimeType** (enumeration)
  : The .NET runtime to search for. This attribute's value must be one of the following:
- *aspnet*
- *core*
- *desktop*

**Variable** (String, required)
  : Name of the variable in which to place the result of the search.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/netfx.xsd)
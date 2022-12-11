---
custom_edit_url: null
sidebar_position: 7
---
# WebApplication element (Iis extension)
Defines properties for a web application. These properties can be used for more than one application defined in a web site or vroot, by defining this element in a common location and referring to it by setting the WebApplication attribute of the WebSite and WebVirtualDir elements.

## Parents
[Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md), [WebVirtualDir](webvirtualdir.md), [WebDir](webdir.md), [WebSite](website.md)

## Children
* [WebApplicationExtension](webapplicationextension.md) 

## Attributes
**AllowSessions** (wxs:YesNoDefaultTypeUnion)
  : Sets the Enable Session State option. When enabled, you can set the session timeout using the SessionTimeout attribute.

**Buffer** (wxs:YesNoDefaultTypeUnion)
  : Sets the option that enables response buffering in the application, which allows ASP script to set response headers anywhere in the script.

**ClientDebugging** (wxs:YesNoDefaultTypeUnion)
  : Enable ASP client-side script debugging.

**DefaultScript** (enumeration)
  : Sets the default script language for the site. This attribute's value must be one of the following:
- *VBScript*
- *JScript*

**Id** (String)
  : Identifier for the web application. If the Id is not specified, it will be generated.

**Isolation** (enumeration)
  : Sets the application isolation level for this application for pre-IIS 6 applications. This attribute's value must be one of the following:
- *low*: Means the application executes within the IIS process.
- *medium*: Executes pooled in a separate process.
- *high*: Means execution alone in a separate process.

**Name** (String, required)
  : Sets the name of this application.

**ParentPaths** (wxs:YesNoDefaultTypeUnion)
  : Sets the parent paths option, which allows a client to use relative paths to reach parent directories from this application.

**ScriptTimeout** (Integer)
  : Sets the timeout value in seconds for executing ASP scripts.

**ServerDebugging** (wxs:YesNoDefaultTypeUnion)
  : Enable ASP server-side script debugging.

**SessionTimeout** (Integer)
  : Sets the timeout value for sessions in minutes.

**WebAppPool** (String)
  : References the Id attribute of a WebAppPool element to use as the application pool for this application in IIS 6 applications.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)
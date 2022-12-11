---
custom_edit_url: null
sidebar_position: 12
---
# WebError element (Iis extension)
Custom Web Errors used by WebSites and Virtual Directories.

## Parents
[WebVirtualDir](webvirtualdir.md), [WebSite](website.md)

## Remarks
You can only use error code and sub code combinations which are supported by IIS.  Attempting to set a custom error for
an error code and sub code combination that is not supported by IIS (in the default list of error codes) will result in
an installation failure.


## Attributes
**ErrorCode** (Integer, required)
  : HTTP 1.1 error code.

**File** (String)
  : File to be sent to the client for this error code and sub code.  This can be formatted.  For example: [#FileId].

**SubCode** (Integer, required)
  : Error sub code.  Set to 0 to get the wild card "*".

**URL** (String)
  : URL to be sent to the client for this error code and sub code.  This can be formatted.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)
---
custom_edit_url: null
sidebar_position: 2
---
# UrlAce element (Http extension)
The security principal and which rights to assign to them for the URL reservation.

## Parents
[UrlReservation](urlreservation.md)

## Attributes
**Id** (String)
  : Unique ID of this URL ACE. If this attribute is not specified, an identifier will be generated automatically.

**Rights** (enumeration)
  : Rights for this ACE. Default is "all". This attribute's value must be one of the following:
- *register*
- *delegate*
- *all*

**SecurityPrincipal** (String)
  : The security principal for this ACE. When the UrlReservation is under a ServiceInstall element, this defaults to "NT SERVICE\ServiceInstallName". This may be either a SID or an account name in a format that [LookupAccountName](https://learn.microsoft.com/en-us/windows/win32/api/winbase/nf-winbase-lookupaccountnamea) supports. When using a SID, an asterisk must be prepended.  For example, "*S-1-5-18".


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/http.xsd)
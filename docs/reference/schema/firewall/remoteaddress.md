---
custom_edit_url: null
sidebar_position: 2
---
# RemoteAddress element (Firewall extension)
A remote address to which the port or program can listen. Address formats vary based on the version of Windows and Windows Firewall the program is being installed on. For Windows XP SP2 and Windows Server 2003 SP1, see [RemoteAddresses Property](https://learn.microsoft.com/en-us/windows/win32/api/netfw/nf-netfw-inetfwauthorizedapplication-get_remoteaddresses). For Windows Vista and Windows Server 2008, see [RemoteAddresses Property](https://learn.microsoft.com/en-us/windows/win32/api/netfw/nf-netfw-inetfwrule-get_remoteaddresses).

## Parents
[FirewallException](firewallexception.md)

## Attributes
**Value** (String, required)
  : A remote address.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/firewall.xsd)
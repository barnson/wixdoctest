---
custom_edit_url: null
sidebar_position: 1
---
# FirewallException element (Firewall extension)
Registers an exception for a program or a specific port and protocol in the Windows Firewall on Windows XP SP2, Windows Server 2003 SP1, and later. For more information about the Windows Firewall, see [About Windows Firewall API](https://learn.microsoft.com/en-us/previous-versions/windows/desktop/ics/about-windows-firewall).

## Parents
[Component](../wxs/component.md), [File](../wxs/file.md)

## Children
* [RemoteAddress](remoteaddress.md) 

## Attributes
**Description** (String)
  : Description for this firewall rule displayed in Windows Firewall manager.

**File** (String)
  : Identifier of a file to be granted access to all incoming ports and protocols. If you use File, you cannot also use Program.  If you use File and also Port or Protocol in the same FirewallException element, the exception will fail to install on Windows XP and Windows Server 2003. IgnoreFailure="yes" can be used to ignore the resulting failure, but the exception will not be added.

**Id** (String)
  : Unique ID of this firewall exception. If the Id is not specified, one will be generated.

**IgnoreFailure** (wxs:YesNoTypeUnion)
  : If "yes", failures to register this firewall exception will be silently ignored. If "no" (the default), failures will cause rollback.

**Name** (String, required)
  : Name of this firewall exception, visible to the user in the firewall control panel.

**Outbound** (wxs:YesNoTypeUnion)
  : If "yes", registers an outbound firewall rule. The default is "no".

**Port** (String)
  : Port to allow through the firewall for this exception.  If you use Port and also File or Program in the same FirewallException element, the exception will fail to install on Windows XP and Windows Server 2003. IgnoreFailure="yes" can be used to ignore the resulting failure, but the exception will not be added.

**Profile** (enumeration)
  : Profile type for this firewall exception. Default is "all". This attribute's value must be one of the following:
- *domain*
- *private*
- *public*
- *all*

**Program** (String)
  : Path to a target program to be granted access to all incoming ports and protocols. Note that this is a formatted field, so you can use [#fileId] syntax to refer to a file being installed. If you use Program, you cannot also use File.  If you use Program and also Port or Protocol in the same FirewallException element, the exception will fail to install on Windows XP and Windows Server 2003. IgnoreFailure="yes" can be used to ignore the resulting failure, but the exception will not be added.

**Protocol** (enumeration)
  : IP protocol used for this firewall exception. If Port is defined, "tcp" is assumed if the protocol is not specified.  If you use Protocol and also File or Program in the same FirewallException element, the exception will fail to install on Windows XP and Windows Server 2003. IgnoreFailure="yes" can be used to ignore the resulting failure, but the exception will not be added. This attribute's value must be one of the following:
- *tcp*
- *udp*

**Scope** (enumeration)
  : The scope of this firewall exception, which indicates whether incoming connections can come from any computer including those on the Internet or only those on the local network subnet. To more precisely specify allowed remote address, specify a custom scope using RemoteAddress child elements. This attribute's value must be one of the following:
- *any*
- *localSubnet*


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/firewall.xsd)
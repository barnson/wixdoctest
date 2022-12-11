---
custom_edit_url: null
sidebar_position: 7
---
# AppId element
Application ID containing DCOM information for the associated application GUID. If this element is nested under a Fragment, Module, or Package element, it must be advertised.

## Windows Installer references
[AppId Table](https://docs.microsoft.com/en-us/windows/win32/msi/appid-table), [Registry Table](https://docs.microsoft.com/en-us/windows/win32/msi/registry-table)

## Parents
[Package](package.md), [Module](module.md), [Fragment](fragment.md), [File](file.md), [TypeLib](typelib.md), [Component](component.md)

## Children
* [Class](class.md) 

## Remarks
When being used in unadvertised mode, the attributes in the AppId element correspond to registry keys
as follows (values that can be specified in authoring are in bold):
<dl><dt>Id</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\AppID\{'{'}**Id**{'}'}]<br /></dd><dt>Specific Example</dt><dd>
                [HKCR\AppID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}]<br /></dd></dl></dd><dt>ActivateAtStorage</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\AppID\{'{'}**Id**{'}'}]<br />
                ActivateAtStorage="**ActivateAtStorage**"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\AppID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}]<br />
                ActivateAtStorage="**Y**"
            </dd></dl></dd><dt>Description</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\AppID\{'{'}**Id**{'}'}]<br />
                @="**Description**"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\AppID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}]<br />
                @="**My AppId Description**"
            </dd></dl></dd><dt>DllSurrogate</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\AppID\{'{'}**Id**{'}'}]<br />
                DllSurrogate="**DllSurrogate**"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\AppID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}]<br />
                DllSurrogate="**C:\surrogate.exe**"
            </dd></dl></dd><dt>LocalService</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\AppID\{'{'}**Id**{'}'}]<br />
                LocalService="**LocalService**"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\AppID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}]<br />
                LocalService="**MyServiceName**"
            </dd></dl></dd><dt>RemoteServerName</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\AppID\{'{'}**Id**{'}'}]<br />
                RemoteServerName="**RemoteServerName**"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\AppID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}]<br />
                RemoteServerName="**MyRemoteServer**"
            </dd></dl></dd><dt>RunAsInteractiveUser</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\AppID\{'{'}**Id**{'}'}]<br />
                RunAs="**RunAsInteractiveUser**"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\AppID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}]<br />
                RunAs="**Interactive User**"
            </dd></dl></dd><dt>ServiceParameters</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\AppID\{'{'}**Id**{'}'}]<br />
                ServiceParameters="**ServiceParameters**"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\AppID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}]<br />
                ServiceParameters="**-param**"
            </dd></dl></dd></dl>

## Attributes
**ActivateAtStorage** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this value to 'yes' to configure the client to activate on the same system as persistent storage.

**Advertise** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this value to 'yes' in order to create a normal AppId table row. Set this value to 'no' in order to generate Registry rows that perform similar registration (without the often problematic Windows Installer advertising behavior).

**Description** (String)
  : Set this value to the description of the AppId. It can only be specified when the AppId is not being advertised.

**DllSurrogate** (String)
  : Set this value to specify that the class is a DLL that is to be activated in a surrogate EXE process, and the surrogate process to be used is the path of a surrogate EXE file specified by the value.

**Id** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : Set this value to the AppID GUID that corresponds to the named executable.

**LocalService** (String)
  : Set this value to the name of a service to allow the object to be installed as a Win32 service.

**RemoteServerName** (String)
  : Set this value to the name of the remote server to configure the client to request the object be run at a particular machine whenever an activation function is called for which a COSERVERINFO structure is not specified.

**RunAsInteractiveUser** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this value to 'yes' to configure a class to run under the identity of the user currently logged on and connected to the interactive desktop when activated by a remote client without being written as a Win32 service.

**ServiceParameters** (String)
  : Set this value to the parameters to be passed to a LocalService on invocation.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
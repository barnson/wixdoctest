---
custom_edit_url: null
sidebar_position: 33
---
# Class element
COM Class registration for parent Component.

## Windows Installer references
[Class Table](https://docs.microsoft.com/en-us/windows/win32/msi/class-table), [ProgId Table](https://docs.microsoft.com/en-us/windows/win32/msi/progid-table), [Registry Table](https://docs.microsoft.com/en-us/windows/win32/msi/registry-table), [AppId Table](https://docs.microsoft.com/en-us/windows/win32/msi/appid-table)

## Parents
[File](file.md), [TypeLib](typelib.md), [AppId](appid.md), [Component](component.md)

## Children
* [FileTypeMask](filetypemask.md) 
* [Interface](interface.md) 
* [ProgId](progid.md) : A ProgId associated with Class must be a child element of the Class element

## Remarks
When being used in unadvertised mode, the attributes in the Class element correspond to registry keys
as follows (values that can be specified in authoring are in bold):
<dl><dt>Id/Context/Server</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\CLSID\{'{'}**Id**{'}'}\**Context1**]<br />
                @="[!**Server**]"<br />
                [HKCR\CLSID\{'{'}**Id**{'}'}\**Context2**]<br />
                @="[!**Server**]"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\**LocalServer**]<br />
                @="[!**comserv.dll**]"<br />
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\**LocalServer32**]<br />
                @="[!**comserv.dll**]"
            </dd></dl></dd><dt>Id/Context/ForeignServer</dt><dd><dl><dt>In General</dt><dd>
              [HKCR\CLSID\{'{'}**Id**{'}'}\**Context1**]<br />
              @="**ForeignServer**"<br />
              [HKCR\CLSID\{'{'}**Id**{'}'}\**Context2**]<br />
              @="**ForeignServer**"
            </dd><dt>Specific Example</dt><dd>
              [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\**LocalServer**]<br />
              @="**mscoree.dll**"<br />
              [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\**LocalServer32**]<br />
              @="**mscoree.dll**"
            </dd></dl></dd><dt>AppId</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\CLSID\{'{'}**Id**{'}'}]<br />
                AppId="{'{'}**AppId**{'}'}"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}]<br />
                AppId="{'{'}**00000000-89AB-0000-0123-000000000000**{'}'}"
            </dd></dl></dd><dt>Argument</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\CLSID\{'{'}**Id**{'}'}\**Context**]<br />
                @="[!**Server**] **Argument**"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\**LocalServer32**]<br />
                @="[!**comserv.dll**] **/arg1 /arg2 /arg3**"<br /></dd></dl></dd><dt>Control</dt><dd><dl><dt>In General</dt><dd>
                Value "yes" specified:<br />
                [HKCR\CLSID\{'{'}**Id**{'}'}\Control]
            </dd><dt>Specific Example</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\Control]
            </dd></dl></dd><dt>Description</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\CLSID\{'{'}**Id**{'}'}]<br />
                @="**Description**"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}]<br />
                @="**Description of Example COM Component**"
            </dd></dl></dd><dt>Handler</dt><dd><dl><dt>In General</dt><dd>
                Value "1" specified:<br />
                [HKCR\CLSID\{'{'}**Id**{'}'}\InprocHandler]<br />
                @="ole.dll"<br />
                Value "2" specified:<br />
                [HKCR\CLSID\{'{'}**Id**{'}'}\InprocHandler32]<br />
                @="ole32.dll"<br />
                Value "3" specified:<br />
                [HKCR\CLSID\{'{'}**Id**{'}'}\InprocHandler]<br />
                @="ole.dll"<br />
                [HKCR\CLSID\{'{'}**Id**{'}'}\InprocHandler32]<br />
                @="ole32.dll"<br />
                Other value specified:<br />
                [HKCR\CLSID\{'{'}**Id**{'}'}\InprocHandler32]<br />
                @="**Handler**"
            </dd><dt>Specific Example (for other value)</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\InprocHandler32]<br />
                @="**handler.dll**"
            </dd></dl></dd><dt>Icon/IconIndex</dt><dd>This is not currently handled properly.</dd><dt>Insertable</dt><dd><dl><dt>In General</dt><dd>
                Value "no" specified:<br />
                [HKCR\CLSID\{'{'}**Id**{'}'}\NotInsertable]<br />
                Value "yes" specified:<br />
                [HKCR\CLSID\{'{'}**Id**{'}'}\Insertable]
            </dd><dt>Specific Example</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\Insertable]
            </dd></dl></dd><dt>Programmable</dt><dd><dl><dt>In General</dt><dd>
                Value "yes" specified:<br />
                [HKCR\CLSID\{'{'}**Id**{'}'}\Programmable]
            </dd><dt>Specific Example</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\Programmable]
            </dd></dl></dd><dt>RelativePath</dt><dd>Unsupported. Please contribute this back to WiX if you know.</dd><dt>SafeForInitializing</dt><dd><dl><dt>In General</dt><dd>
                Value "yes" specified:<br />
                [HKCR\CLSID\{'{'}**Id**{'}'}\Implemented Categories\{'{'}7DD95802-9882-11CF-9FA9-00AA006C42C4{'}'}]
            </dd><dt>Specific Example</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\Implemented Categories\{'{'}7DD95802-9882-11CF-9FA9-00AA006C42C4{'}'}]
            </dd></dl></dd><dt>SafeForScripting</dt><dd><dl><dt>In General</dt><dd>
                Value "yes" specified:<br />
                [HKCR\CLSID\{'{'}**Id**{'}'}\Implemented Categories\{'{'}7DD95801-9882-11CF-9FA9-00AA006C42C4{'}'}]
            </dd><dt>Specific Example</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\Implemented Categories\{'{'}7DD95801-9882-11CF-9FA9-00AA006C42C4{'}'}]
            </dd></dl></dd><dt>ThreadingModel</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\CLSID\{'{'}**Id**{'}'}\**Context**]<br />
                ThreadingModel="**ThreadingModel**"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\**LocalServer32**]<br />
                ThreadingModel="**Apartment**"
            </dd></dl></dd><dt>TypeLibId (from parent TypeLib/@Id)</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\CLSID\{'{'}**Id**{'}'}\TypeLib]<br />
                @="{'{'}**TypeLibId**{'}'}"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\TypeLib]<br />
                @="{'{'}**11111111-89AB-1111-0123-111111111111**{'}'}"
            </dd></dl></dd><dt>Version</dt><dd><dl><dt>In General</dt><dd>
                [HKCR\CLSID\{'{'}**Id**{'}'}\Version]<br />
                @="**Version**"
            </dd><dt>Specific Example</dt><dd>
                [HKCR\CLSID\{'{'}**01234567-89AB-CDEF-0123-456789ABCDEF**{'}'}\Version]<br />
                @="**1.0.0.0**"
            </dd></dl></dd></dl>

## Attributes
**Advertise** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this value to "yes" in order to create a normal Class table row. Set this value to "no" in order to generate Registry rows that perform similar registration (without the often problematic Windows Installer advertising behavior).

**AppId** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'))
  : This attribute is only allowed when a Class is advertised. Using this attribute will reference an Application ID containing DCOM information for the associated application GUID. The value must correspond to an AppId/@Id of an AppId element nested under a Fragment, Module, or Package element. To associate an AppId with a non-advertised class, nest the class within a parent AppId element.

**Argument** (String)
  : This column is optional only when the Context column is set to "LocalServer" or "LocalServer32" server context. The text is registered as the argument against the OLE server and is used by OLE for invoking the server. Note that the resolution of properties in the Argument field is limited. A property formatted as [Property] in this field can only be resolved if the property already has the intended value when the component owning the class is installed. For example, for the argument "[#MyDoc.doc]" to resolve to the correct value, the same process must be installing the file MyDoc.doc and the component that owns the class.

**Context** ()
  : The server context(s) for this COM server. This attribute is optional for VB6 libraries that are marked "PublicNotCreateable". Class elements marked Advertised must specify at least one server context. It is most common for there to be a single value for the Context attribute.

**Control** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Set this attribute's value to 'yes' to identify an object as an ActiveX Control. The default value is 'no'.

**Description** (String)
  : Localized description associated with the Class ID and Program ID.

**ForeignServer** (String)
  : May only be specified if the value of the Advertise attribute is "no" and Server has not been specified. In addition, it may only be used when the Class element is directly under the Component element. The value can be that of an registry type (REG_SZ). This attribute should be used to specify foreign servers, such as mscoree.dll if needed.

**Handler** (String)
  : The default inproc handler. May be optionally provided only for Context = LocalServer or LocalServer32. Value of "1" creates a 16-bit InprocHandler (appearing as the InprocHandler value). Value of "2" creates a 32-bit InprocHandler (appearing as the InprocHandler32 value). Value of "3" creates 16-bit as well as 32-bit InprocHandlers. A non-numeric value is treated as a system file that serves as the 32-bit InprocHandler (appearing as the InprocHandler32 value).

**Icon** (String)
  : The file providing the icon associated with this CLSID. Reference to an Icon element (should match the Id attribute of an Icon element). This is currently not supported if the value of the Advertise attribute is "no".

**IconIndex** (Integer)
  : Icon index into the icon file.

**Id** ([Guid](guid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF" or "{01234567-89AB-CDEF-0123-456789ABCDEF}". Also allows "PUT-GUID-HERE" for use in examples.'), required)
  : The Class identifier (CLSID) of a COM server.

**Insertable** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies the CLSID may be insertable.

**Programmable** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies the CLSID may be programmable.

**RelativePath** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : When the value is "yes", the bare file name can be used for COM servers. The installer registers the file name only instead of the complete path. This enables the server in the current directory to take precedence and allows multiple copies of the same component.

**SafeForInitializing** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : May only be specified if the value of the Advertise attribute is "no".

**SafeForScripting** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : May only be specified if the value of the Advertise attribute is "no".

**Server** (String)
  : May only be specified if the value of the Advertise attribute is "no" and the ForeignServer attribute is not specified. File Id of the COM server file. If this element is nested under a File element, this value defaults to the value of the parent File/@Id.

**ShortPath** ([YesNoTypeUnion](yesnotype.md 'Values of this type will either be "yes"/"true" or "no"/"false".'))
  : Specifies whether or not to use the short path for the COM server. This can only apply when Advertise is set to 'no'. The default is 'no' meaning that it will use the long file name for the COM server.

**ThreadingModel** (enumeration)
  : Threading model for the CLSID. This attribute's value must be one of the following:
- *apartment*
- *free*
- *both*
- *neutral*
- *single*
- *rental*

**Version** (String)
  : Version for the CLSID.


## See also
[AppId](appid.md)

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
---
custom_edit_url: null
sidebar_position: 3
---
# ComPlusAssembly element (Complus extension)
Represents a DLL or assembly to be registered with COM+. If this element is a child of a ComPlusApplication element, the assembly will be registered in this application. Other ways the Application attribute must be set to an application. The element must be a descendent of a Component element, it can not be a child of a ComPlusApplication locator element.

## Parents
[Component](../wxs/component.md), [ComPlusApplication](complusapplication.md)

## Children
* [ComPlusAssemblyDependency](complusassemblydependency.md) 
* [ComPlusComponent](compluscomponent.md) 

## Remarks
<p>
  When installing a native assembly, all components
  contained in the assembly must be represented as ComPlusComponent elements
  under this element. Any component not listed will not be removed during
  uninstall.
</p>

<p>
  The fields DllPath, TlbPath and PSDllPath are formatted
  fields that should contain file paths to there respective file types. A typical
  value for DllPath for example, should be something like “[#MyAssembly_dll]”,
  where “MyAssembly_dll” is the key of the dll file in the File table.
</p>

<p>
  <b>Warning</b>: The assembly name provided in the AssemblyName
  attribute must be a fully specified assembly name, if a partial name is
  provided a random assembly matching the partial name will be selected.
</p>


## Attributes
**Application** (String)
  : If the element is not a child of a ComPlusApplication element, this attribute should be provided with the id of a ComPlusApplication element representing the application the assembly is to be registered in. This attribute can be omitted for a .NET assembly even if the application is not a child of a ComPlusApplication element.

**AssemblyName** (String)
  : The name of the assembly used to identify the assembly in the GAC. This attribute can be provided only if DllPathFromGAC is set to “yes”.

**DllPath** (String)
  : The path to locate the assembly DLL during registration. This attribute should be provided if DllPathFromGAC is not set to “yes”.

**DllPathFromGAC** (wxs:YesNoTypeUnion)
  : Indicates that the DLL path should be extracted from the GAC instead for being provided in the DllPath attribute. If this attribute is set to “yes”, the name of the assembly can be provided using the AssemblyName attribute. Or, if this AssemblyName attribute is missing, the name will be extracted from the MsiAssemblyName table using the id of the parent Component element.

**EventClass** (wxs:YesNoTypeUnion)
  : Indicates that the assembly is to be installed as an event class DLL. This attribute is only valid for native assemblies. The assembly will be installed with the COM+ catalog’s InstallEventClass() function.

**Id** (String, required)
  : Identifier for the element.

**PSDllPath** (String)
  : An optional path to an external proxy/stub DLL for the assembly.

**RegisterInCommit** (wxs:YesNoTypeUnion)
  : Indicates that the assembly should be installed in the commit custom action instead of the normal deferred custom action. This is necessary when installing .NET assemblies to the GAC in the same installation, as the assemblies are not visible in the GAC until after the InstallFinalize action has run.

**TlbPath** (String)
  : An optional path to an external type lib for the assembly. This attribute must be provided if the Type attribute is set to “.net”.

**Type** (enumeration, required)
  :  This attribute's value must be one of the following:
- *native*
- *.net*


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)
---
custom_edit_url: null
sidebar_position: 4
---
# ComPlusAssemblyDependency element (Complus extension)
Defines a dependency between two assemblies. This element affects the order in which assembles are registered. Any assemblies referenced by this element are guarantied to be registered before, and unregistered after, the assembly referenced by the parent ComPlusAssembly element.

## Parents
[ComPlusAssembly](complusassembly.md)

## Remarks
It is only necessary to explicitly specify dependencies between
assemblies contained in the same package (MSI or MSM). Assemblies merged in to a
package from a merge module will always be installed before any assemblies
specified in the base package. Assemblies merged in from different merge
modules are sequenced using the ModuleDependency MSI table. It is not possible
to have cross dependencies between merge modules or have an assembly in a merge
module depend on an assembly in the base package.


## Attributes
**RequiredAssembly** (String, required)
  : Reference to the id of the assembly required by the parent ComPlusAssembly element.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)
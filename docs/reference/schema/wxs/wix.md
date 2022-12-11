---
custom_edit_url: null
sidebar_position: 289
---
# Wix element
This is the top-level container element for every wxs file. Among the possible children, the Bundle, Package, Module, Patch, and PatchCreation elements are analogous to the main function in a C program. There can only be one of these present when linking occurs. Package compiles into an msi file, Module compiles into an msm file, PatchCreation compiles into a pcp file. The Fragment element is an atomic unit which ultimately links into either a Package, Module, or PatchCreation. The Fragment can either be completely included or excluded during linking.

## Children
* [Bundle](bundle.md) 
* [Fragment](fragment.md) 
* [Module](module.md) 
* [Package](package.md) 
* [Patch](patch.md) 
* [PatchCreation](patchcreation.md) 

## Attributes
**RequiredVersion** ([VersionType](versiontype.md 'Values of this type will look like: "x.x.x.x" where x is an integer from 0 to 65534.'))
  : Required version of the WiX toolset to compile this input file.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
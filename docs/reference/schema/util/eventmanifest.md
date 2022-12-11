---
custom_edit_url: null
sidebar_position: 9
---
# EventManifest element (Util extension)
Used to install Event Manifests.

## Parents
[File](../wxs/file.md)

## Attributes
**MessageFile** (String)
  : The message file (including path) of all the providers in the event manifest. Often the message file path cannot be determined until setup time. Put your MessageFile here and the messageFileName attribute of the all the providers in the manifest will be updated with the path before it is registered.

**ParameterFile** (String)
  : The parameter file (including path) of all the providers in the event manifest. Often the parameter file path cannot be determined until setup time. Put your ParameterFile here and the parameterFileName attribute of the all the providers in the manifest will be updated with the path before it is registered.

**ResourceFile** (String)
  : The resource file (including path) of all the providers in the event manifest. Often the resource file path cannot be determined until setup time. Put your ResourceFile here and the resourceFileName attribute of the all the providers in the manifest will be updated with the path before it is registered.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/util.xsd)
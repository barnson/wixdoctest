---
custom_edit_url: null
toc_max_heading_level: 2
---
# FeatureInstallation Class
Represents an instance of a feature of an installed product.
## Properties
| Property | Description |
| ------ | ----------- |
| [FeatureName](#featurename) | Gets the name of the feature. |
| [Parent](#parent) | Gets the parent of the feature, or null if the feature has no parent (it is a root feature). |
| [State](#state) | Gets the installed state of the feature. |
| [Usage](#usage) | Gets the usage metrics for the feature. |
`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## FeatureName Property {#featurename}
Gets the name of the feature.
### Declaration
```cs
public string FeatureName { get; set; } 
```
## Parent Property {#parent}
Gets the parent of the feature, or null if the feature has no parent (it is a root feature).
### Declaration
```cs
public FeatureInstallation Parent { get; set; } 
```
### Remarks
Invocation of this property may be slightly costly for products with many features, because it involves an enumeration of all the features in the product.
## State Property {#state}
Gets the installed state of the feature.
### Declaration
```cs
public InstallState State { get; set; } 
```
### Remarks
Win32 MSI API: [MsiQueryFeatureState](http://msdn.microsoft.com/library/en-us/msi/setup/msiqueryfeaturestate.asp) 

## Usage Property {#usage}
Gets the usage metrics for the feature.
### Declaration
```cs
public FeatureInstallation+UsageData Usage { get; set; } 
```
### Remarks
If no usage metrics are recorded, the «see P:WixToolset.Dtf.WindowsInstaller.FeatureInstallation.UsageData.UseCount» value is 0.
Win32 MSI API: [MsiGetFeatureUsage](http://msdn.microsoft.com/library/en-us/msi/setup/msigetfeatureusage.asp) 


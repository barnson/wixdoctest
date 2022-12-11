---
custom_edit_url: null
toc_max_heading_level: 2
---
# FeatureInfoCollection Class
Accessor for information about features within the context of an installation session.
## Methods
| Method | Description |
| ------ | ----------- |
| [Contains(feature)](#contains_feature) | Checks if the collection contains a feature. |
| [CopyTo(array, arrayIndex)](#copyto_array_arrayindex) | Copies the features into an array. |
| [GetEnumerator()](#getenumerator_nop) | Enumerates the features in the collection. |
## Properties
| Property | Description |
| ------ | ----------- |
| [Count](#count) | Gets the number of features defined for the product. |
| [Item](#item) | Gets information about a feature within the context of an installation session. |
`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Contains(feature) Method {#contains_feature}
Checks if the collection contains a feature.
### Declaration
```cs
public bool Contains(
  string feature
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| feature | string | name of the feature |
### Return value
`bool` true if the feature is in the collection, else false
## CopyTo(array, arrayIndex) Method {#copyto_array_arrayindex}
Copies the features into an array.
### Declaration
```cs
public void CopyTo(
  FeatureInfo[] array,
  int arrayIndex
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| array | FeatureInfo[] | array that receives the features |
| arrayIndex | int | offset into the array |
## GetEnumerator() Method {#getenumerator_nop}
Enumerates the features in the collection.
### Declaration
```cs
public IEnumerator<WixToolset.Dtf.WindowsInstaller.FeatureInfo> GetEnumerator
```
### Return value
`IEnumerator<WixToolset.Dtf.WindowsInstaller.FeatureInfo>` an enumerator over all features in the collection
## Count Property {#count}
Gets the number of features defined for the product.
### Declaration
```cs
public int Count { get; set; } 
```
## Item Property {#item}
Gets information about a feature within the context of an installation session.
### Declaration
```cs
public FeatureInfo Item[
  string feature
] { get; set; } 
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| feature | string | name of the feature |

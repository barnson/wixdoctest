---
custom_edit_url: null
sidebar_position: 1
---
# ComPlusApplication element (Complus extension)
Defines a COM+ application. If this element is a descendent of a Component element, the application will be created in association with this component. If the element is a child of any of the Fragment, Module, or Package elements it is considered to be a locater, referencing an existing application.  If the element is a child of a ComPlusPartition element, or have its Partition attribute set, the application will be installed under the referenced partition.

## Parents
[Component](../wxs/component.md), [Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md), [ComPlusPartition](compluspartition.md)

## Children
* [ComPlusApplicationRole](complusapplicationrole.md) 
* [ComPlusAssembly](complusassembly.md) 

## Attributes
**AccessChecksLevel** (enumeration)
  :  This attribute's value must be one of the following:
- *applicationLevel*
- *applicationComponentLevel*

**Activation** (enumeration)
  :  This attribute's value must be one of the following:
- *inproc*
- *local*

**ApplicationAccessChecksEnabled** (wxs:YesNoTypeUnion)
  : 

**ApplicationDirectory** (String)
  : 

**ApplicationId** (String)
  : Id for the application. This attribute can be omitted, in which case an id will be generated on install. If the element is a locater, this attribute can be omitted if a value is provided for the Name attribute.

**Authentication** (enumeration)
  :  This attribute's value must be one of the following:
- *default*
- *none*
- *connect*
- *call*
- *packet*
- *integrity*
- *privacy*

**AuthenticationCapability** (enumeration)
  :  This attribute's value must be one of the following:
- *none*
- *secureReference*
- *staticCloaking*
- *dynamicCloaking*

**Changeable** (wxs:YesNoTypeUnion)
  : 

**CommandLine** (String)
  : 

**ConcurrentApps** (xs:int)
  : 

**CreatedBy** (String)
  : 

**CRMEnabled** (wxs:YesNoTypeUnion)
  : 

**CRMLogFile** (String)
  : 

**Deleteable** (wxs:YesNoTypeUnion)
  : 

**Description** (String)
  : 

**DumpEnabled** (wxs:YesNoTypeUnion)
  : 

**DumpOnException** (wxs:YesNoTypeUnion)
  : 

**DumpOnFailfast** (wxs:YesNoTypeUnion)
  : 

**DumpPath** (String)
  : 

**EventsEnabled** (wxs:YesNoTypeUnion)
  : 

**Id** (String, required)
  : Identifier for the element.

**Identity** (String)
  : 

**ImpersonationLevel** (enumeration)
  :  This attribute's value must be one of the following:
- *anonymous*
- *identify*
- *impersonate*
- *delegate*

**IsEnabled** (wxs:YesNoTypeUnion)
  : 

**MaxDumpCount** (xs:int)
  : 

**Name** (String)
  : Name of the application. This attribute can be omitted if the element is a locater, and a value is provided for the PartitionId attribute.

**Partition** (String)
  : If the element is not a child of a ComPlusPartition element, this attribute can be provided with the id of a ComPlusPartition element representing the partition the application belongs to.

**Password** (String)
  : 

**QCAuthenticateMsgs** (enumeration)
  :  This attribute's value must be one of the following:
- *secureApps*
- *off*
- *on*

**QCListenerMaxThreads** (xs:int)
  : 

**QueueListenerEnabled** (wxs:YesNoTypeUnion)
  : 

**QueuingEnabled** (wxs:YesNoTypeUnion)
  : 

**RecycleActivationLimit** (xs:int)
  : 

**RecycleCallLimit** (xs:int)
  : 

**RecycleExpirationTimeout** (xs:int)
  : 

**RecycleLifetimeLimit** (xs:int)
  : 

**RecycleMemoryLimit** (xs:int)
  : 

**Replicable** (wxs:YesNoTypeUnion)
  : 

**RunForever** (wxs:YesNoTypeUnion)
  : 

**ShutdownAfter** (xs:int)
  : 

**SoapActivated** (wxs:YesNoTypeUnion)
  : 

**SoapBaseUrl** (String)
  : 

**SoapMailTo** (String)
  : 

**SoapVRoot** (String)
  : 

**SRPEnabled** (wxs:YesNoTypeUnion)
  : 

**SRPTrustLevel** (enumeration)
  :  This attribute's value must be one of the following:
- *disallowed*
- *fullyTrusted*

**ThreeGigSupportEnabled** (wxs:YesNoTypeUnion)
  : 


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)
---
custom_edit_url: null
sidebar_position: 5
---
# ComPlusComponent element (Complus extension)
Represents a COM+ component in an assembly.

## Parents
[ComPlusAssembly](complusassembly.md)

## Children
* [ComPlusInterface](complusinterface.md) 
* [ComPlusRoleForComponent](complusroleforcomponent.md) 
* [ComPlusSubscription](complussubscription.md) 

## Attributes
**AllowInprocSubscribers** (wxs:YesNoTypeUnion)
  : 

**CLSID** ([uuid](uuid.md 'Values of this type will look like: "01234567-89AB-CDEF-0123-456789ABCDEF".'), required)
  : CLSID of the component.

**ComponentAccessChecksEnabled** (wxs:YesNoTypeUnion)
  : 

**ComponentTransactionTimeout** (xs:int)
  : 

**ComponentTransactionTimeoutEnabled** (wxs:YesNoTypeUnion)
  : 

**COMTIIntrinsics** (wxs:YesNoTypeUnion)
  : 

**ConstructionEnabled** (wxs:YesNoTypeUnion)
  : 

**ConstructorString** (String)
  : 

**CreationTimeout** (xs:int)
  : 

**Description** (String)
  : 

**EventTrackingEnabled** (wxs:YesNoTypeUnion)
  : 

**ExceptionClass** (String)
  : 

**FireInParallel** (wxs:YesNoTypeUnion)
  : 

**Id** (String, required)
  : Identifier for the element.

**IISIntrinsics** (wxs:YesNoTypeUnion)
  : 

**InitializesServerApplication** (wxs:YesNoTypeUnion)
  : 

**IsEnabled** (wxs:YesNoTypeUnion)
  : 

**IsPrivateComponent** (wxs:YesNoTypeUnion)
  : 

**JustInTimeActivation** (wxs:YesNoTypeUnion)
  : 

**LoadBalancingSupported** (wxs:YesNoTypeUnion)
  : 

**MaxPoolSize** (xs:int)
  : 

**MinPoolSize** (xs:int)
  : 

**MultiInterfacePublisherFilterCLSID** (String)
  : 

**MustRunInClientContext** (wxs:YesNoTypeUnion)
  : 

**MustRunInDefaultContext** (wxs:YesNoTypeUnion)
  : 

**ObjectPoolingEnabled** (wxs:YesNoTypeUnion)
  : 

**PublisherID** (String)
  : 

**SoapAssemblyName** (String)
  : 

**SoapTypeName** (String)
  : 

**Synchronization** (enumeration)
  :  This attribute's value must be one of the following:
- *ignored*
- *none*
- *supported*
- *required*
- *requiresNew*

**Transaction** (enumeration)
  :  This attribute's value must be one of the following:
- *ignored*
- *none*
- *supported*
- *required*
- *requiresNew*

**TxIsolationLevel** (enumeration)
  :  This attribute's value must be one of the following:
- *any*
- *readUnCommitted*
- *readCommitted*
- *repeatableRead*
- *serializable*


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)
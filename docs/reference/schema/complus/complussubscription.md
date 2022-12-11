---
custom_edit_url: null
sidebar_position: 16
---
# ComPlusSubscription element (Complus extension)
Defines an event subscription for a COM+ component.

## Parents
[Component](../wxs/component.md), [ComPlusComponent](compluscomponent.md)

## Attributes
**Component** (String)
  : If the element is not a child of a ComPlusComponent element, this attribute should be provided with the id of a ComPlusComponent element representing the component the subscription is to be created for.

**Description** (String)
  : 

**Enabled** (wxs:YesNoTypeUnion)
  : 

**EventClassPartitionID** (String)
  : 

**EventCLSID** (String)
  : CLSID of the event class for the subscription. If a value for this attribute is not provided, a value for the PublisherID attribute must be provided.

**FilterCriteria** (String)
  : 

**Id** (String, required)
  : Identifier for the element.

**InterfaceID** (String)
  : 

**MachineName** (String)
  : 

**MethodName** (String)
  : 

**Name** (String, required)
  : Name of the subscription.

**PerUser** (wxs:YesNoTypeUnion)
  : 

**PublisherID** (String)
  : Publisher id for the subscription. If a value for this attribute is not provided, a value for the EventCLSID attribute must be provided.

**Queued** (wxs:YesNoTypeUnion)
  : 

**SubscriberMoniker** (String)
  : 

**SubscriptionId** (String)
  : Id of the subscription. If a value is not provided for this attribute, an id will be generated during installation.

**UserName** (String)
  : 


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/complus.xsd)
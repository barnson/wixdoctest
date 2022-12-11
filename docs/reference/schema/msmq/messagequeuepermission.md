---
custom_edit_url: null
sidebar_position: 2
---
# MessageQueuePermission element (Msmq extension)


## Parents
[Component](../wxs/component.md), [MessageQueue](messagequeue.md)

## Attributes
**ChangeQueuePermissions** (wxs:YesNoTypeUnion)
  : 

**DeleteJournalMessage** (wxs:YesNoTypeUnion)
  : 

**DeleteMessage** (wxs:YesNoTypeUnion)
  : 

**DeleteQueue** (wxs:YesNoTypeUnion)
  : 

**GetQueuePermissions** (wxs:YesNoTypeUnion)
  : 

**GetQueueProperties** (wxs:YesNoTypeUnion)
  : 

**Group** (String)
  : 

**Id** (String, required)
  : Identifier for the message queue permission. If the Id is not specified, one will be generated.

**MessageQueue** (String)
  : Message queue to set permissions on. Must be specified when under a Component element. Cannot be specified when under a MessageQueue element.

**PeekMessage** (wxs:YesNoTypeUnion)
  : 

**QueueGenericAll** (wxs:YesNoTypeUnion)
  : 

**QueueGenericExecute** (wxs:YesNoTypeUnion)
  : 

**QueueGenericRead** (wxs:YesNoTypeUnion)
  : 

**QueueGenericWrite** (wxs:YesNoTypeUnion)
  : 

**ReceiveJournalMessage** (wxs:YesNoTypeUnion)
  : 

**ReceiveMessage** (wxs:YesNoTypeUnion)
  : 

**SetQueueProperties** (wxs:YesNoTypeUnion)
  : 

**TakeQueueOwnership** (wxs:YesNoTypeUnion)
  : 

**User** (String)
  : 

**WriteMessage** (wxs:YesNoTypeUnion)
  : 


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/msmq.xsd)
---
custom_edit_url: null
sidebar_position: 1
---
# MessageQueue element (Msmq extension)
Installs an MSMQ message queue.

## Parents
[Component](../wxs/component.md)

## Children
* [MessageQueuePermission](messagequeuepermission.md) 

## Attributes
**Authenticate** (wxs:YesNoTypeUnion)
  : The default value is "no".

**BasePriority** (Integer)
  : The base priority of the queue.

**Id** (String)
  : Identifier for the message queue. If the Id is not specified, one will be generated.

**Journal** (wxs:YesNoTypeUnion)
  : The default value is "no".

**JournalQuota** (Integer)
  : 

**Label** (String, required)
  : 

**MulticastAddress** (String)
  : 

**PathName** (String, required)
  : 

**PrivLevel** (enumeration)
  :  This attribute's value must be one of the following:
- *none*
- *optional*
- *body*

**Quota** (Integer)
  : 

**ServiceTypeGuid** (String)
  : 

**Transactional** (wxs:YesNoTypeUnion)
  : The default value is "no".


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/msmq.xsd)
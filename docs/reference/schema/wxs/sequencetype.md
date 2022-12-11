---
custom_edit_url: null
sidebar_position: 313
---
# SequenceType type
Controls which sequences the item assignment is sequenced in.

## Enumeration values
- *both*: Schedules the assignment in the InstallUISequence and the InstallExecuteSequence.
- *first*: Schedules the assignment to run in the InstallUISequence or the InstallExecuteSequence if the InstallUISequence is skipped.
- *execute*: Schedules the assignment only in the the InstallExecuteSequence.
- *ui*: Schedules the assignment only in the the InstallUISequence.

[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/wix.xsd)
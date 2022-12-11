---
custom_edit_url: null
sidebar_position: 3
---
# SqlLogFileSpec element (Sql extension)
File specification for a Sql database.

## Parents
[SqlDatabase](sqldatabase.md)

## Attributes
**Filename** (String)
  : Specifies the operating-system file name for the log file.

**GrowthSize** (String)
  : Specifies the growth increment of the log file. The GB, MB and KB and % suffixes can be used to specify gigabytes, megabytes, kilobytes or a percentage of the current file size to grow. The default is megabytes if no suffix is specified. The default value is 10% if GrowthSize is not specified, and the minimum value is 64 KB. The GrowthSize setting for a file cannot exceed the MaxSize setting.

**Id** (String)
  : Unique identifier in your installation package for this log file specification. If an Id is not provided, one will generated for you.

**MaxSize** (String)
  : Specifies the maximum size to which the log file can grow. The GB, MB and KB suffixes can be used to to specify gigabytes, megabytes or kilobytes. The default is megabytes if no suffix is specified. If MaxSize is not specified, the file will grow until the disk is full.

**Name** (String)
  : Specifies the logical name for the log file.

**Size** (String)
  : Specifies the size of the log file. The GB, MB and KB suffixes can be used to specify gigabytes, megabytes or kilobytes. The default is megabytes if no suffix is specified. When a Size is not supplied for a log file, SQL Server makes the file 1 MB.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/sql.xsd)
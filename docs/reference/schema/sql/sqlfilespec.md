---
custom_edit_url: null
sidebar_position: 2
---
# SqlFileSpec element (Sql extension)
File specification for a Sql database.

## Parents
[SqlDatabase](sqldatabase.md)

## Attributes
**Filename** (String, required)
  : Specifies the operating-system file name for the database file.

**GrowthSize** (String)
  : Specifies the growth increment of the database file. The GB, MB and KB and % suffixes can be used to specify gigabytes, megabytes, kilobytes or a percentage of the current file size to grow. The default is megabytes if no suffix is specified. The default value is 10% if GrowthSize is not specified, and the minimum value is 64 KB. The GrowthSize setting for a file cannot exceed the MaxSize setting.

**Id** (String, required)
  : Unique identifier in your installation package for this file specification. If an Id is not provided, one will generated for you.

**MaxSize** (String)
  : Specifies the maximum size to which the database file can grow. The GB, MB and KB suffixes can be used to to specify gigabytes, megabytes or kilobytes. The default is megabytes if no suffix is specified. If MaxSize is not specified, the file will grow until the disk is full.

**Name** (String)
  : Specifies the logical name for the database file.

**Size** (String)
  : Specifies the size of the database file. The GB, MB and KB suffixes can be used to specify gigabytes, megabytes or kilobytes. The default is megabytes if no suffix is specified. When a Size is not supplied for a database file, SQL Server uses the size of the primary file in the model database.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/sql.xsd)
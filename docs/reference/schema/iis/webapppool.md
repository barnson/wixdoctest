---
custom_edit_url: null
sidebar_position: 9
---
# WebAppPool element (Iis extension)
IIS Application Pool

## Parents
[Component](../wxs/component.md), [Fragment](../wxs/fragment.md), [Module](../wxs/module.md), [Package](../wxs/package.md)

## Children
* [RecycleTime](recycletime.md) 

## Attributes
**CpuAction** (enumeration)
  : Action taken when CPU exceeds maximum CPU use (as defined with MaxCpuUsage and RefreshCpu). This attribute's value must be one of the following:
- *none*
- *shutdown*

**Id** (String)
  : Id of the AppPool. If the Id is not specified, it will be generated.

**Identity** (enumeration)
  : Identity you want the AppPool to run under (applicationPoolIdentity is only available on IIS7). Use the 'other' value in conjunction with the User attribute to specify non-standard user. This attribute's value must be one of the following:
- *networkService*
- *localService*
- *localSystem*
- *other*
- *applicationPoolIdentity*

**IdleTimeout** (Integer)
  : Shutdown worker process after being idle for (time in minutes).

**ManagedPipelineMode** (String)
  : Specifies the request-processing mode that is used to process requests for managed content.  Only available on IIS7, ignored on IIS6. See https://learn.microsoft.com/en-us/iis/configuration/system.applicationHost/applicationPools/applicationPoolDefaults/ for valid values. This attribute may be set via a formatted Property (e.g. [MyProperty]).

**ManagedRuntimeVersion** (String)
  : Specifies the .NET Framework version to be used by the application pool.  Only available on IIS7, ignored on IIS6. See https://learn.microsoft.com/en-us/iis/configuration/system.applicationHost/applicationPools/applicationPoolDefaults/ for valid values. This attribute may be set via a formatted Property (e.g. [MyProperty]).

**MaxCpuUsage** ([PercentType](percenttype.md 'Values of this type are any integers between 0 and 100, inclusive.'))
  : Maximum CPU usage (percent).

**MaxWorkerProcesses** (Integer)
  : Maximum number of worker processes.

**Name** (String, required)
  : Name of the AppPool to be shown in IIs.

**PrivateMemory** (Integer)
  : Specifies the amount of private memory (in KB) that a worker process can use before the worker process recycles. The maximum value supported for this attribute is 4,294,967 KB.

**QueueLimit** (Integer)
  : Limit the kernel request queue (number of requests).

**RecycleMinutes** (Integer)
  : How often, in minutes, you want the AppPool to be recycled.

**RecycleRequests** (Integer)
  : How often, in requests, you want the AppPool to be recycled.

**RefreshCpu** (Integer)
  : Refresh CPU usage numbers (in minutes).

**User** (String)
  : User account to run the AppPool as. To use this, you must set the Identity attribute to 'other'.

**VirtualMemory** (Integer)
  : Specifies the amount of virtual memory (in KB) that a worker process can use before the worker process recycles. The maximum value supported for this attribute is 4,294,967 KB.


[Edit the schema for this page](https://github.com/wixtoolset/web/blob/master/src/xsd4/iis.xsd)
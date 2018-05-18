---
Description: 'The Performance Counter provider is a high-performance provider that provides raw performance counter data to the WMI Performance Counter Classes derived from Win32\_PerfRawData. The \_\_Win32Provider instance name is &\#0034;NT5\_GenericPerfProvider\_V1&\#0034;.'
audience: developer
author: 'REDMOND\\markl'
manager: 'REDMOND\\markl'
ms.assetid: '2c7206e7-f5f8-4d40-b993-56122e48069b'
ms.prod: 'windows-server-dev'
ms.technology: 'windows-management-instrumentation'
ms.tgt_platform: multiple
title: Performance Counter Provider
---

# Performance Counter Provider

\[The Performance Counter Provider is no longer available for use. Instead, use the [WMIPerfInst](wmiperfinst-provider.md) provider.\]

The Performance Counter provider is a high-performance provider that provides raw performance counter data to the WMI [Performance Counter Classes](https://msdn.microsoft.com/library/aa392738) derived from [**Win32\_PerfRawData**](https://msdn.microsoft.com/library/aa394299). The [**\_\_Win32Provider**](--win32provider.md) instance name is "NT5\_GenericPerfProvider\_V1".

The [**Win32\_PerfRawData**](https://msdn.microsoft.com/library/aa394299) classes are located in the WMI "Root\\CIMv2" namespace. Each WMI performance class corresponds to a performance object in a performance library. The properties of these classes represent the counters for the object. The WMI class name for a raw counter object is of the form **Win32\_PerfRawData\_\_*service\_name*\_*object\_name***. For example, the WMI class name that contains the logical disk counters is [**Win32\_PerfRawData\_PerfDisk\_LogicalDisk**](https://msdn.microsoft.com/library/aa394307).

You can use the corresponding [**Win32\_PerfFormattedData**](https://msdn.microsoft.com/library/aa394253) class to get the pre-calculated performance data shown in [*System Monitor*](gloss-s.md#wmi-gloss-system-monitor). For example, use the [**Win32\_PerfFormattedData\_PerfDisk\_LogicalDisk**](https://msdn.microsoft.com/library/aa394261) class to get pre-calculated disk data.

For more information about how to write a client that can access raw performance data, see [Accessing Performance Data in C++](accessing-performance-data-in-c--.md).

As a high-performance provider, the Performance Counter provider implements the standard [**IWbemProviderInit**](iwbemproviderinit.md) interface, as well as the [**IWbemRefresher::Refresh**](iwbemrefresher-refresh.md) method and the following [**IWbemHiPerfProvider**](iwbemhiperfprovider.md) methods:

-   [**CreateRefreshableEnum**](iwbemhiperfprovider-createrefreshableenum.md)
-   [**CreateRefreshableObject**](iwbemhiperfprovider-createrefreshableobject.md)
-   [**CreateRefresher**](iwbemhiperfprovider-createrefresher.md)
-   [**GetObjects**](iwbemhiperfprovider-getobjects.md)
-   [**QueryInstances**](iwbemhiperfprovider-queryinstances.md)
-   [**StopRefreshing**](iwbemhiperfprovider-stoprefreshing.md)

## Related topics

<dl> <dt>

[WMI Providers](wmi-providers.md)
</dt> </dl>

 

 



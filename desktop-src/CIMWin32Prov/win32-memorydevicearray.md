---
Description: The Win32\_MemoryDeviceArray association WMI class relates a memory device and the memory array in which it resides.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 39ea6333-2352-488b-99e4-97594bea7dcd
ms.prod: windows-server-dev
ms.technology:
- cimwin32
- windows-management-instrumentation
ms.tgt_platform: multiple
title: Win32\_MemoryDeviceArray class
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- Win32_MemoryDeviceArray
- Win32_MemoryDeviceArray.GroupComponent
- Win32_MemoryDeviceArray.PartComponent
api_type: 
- DllExport
api_location: 
- CIMWin32.dll
---

# Win32\_MemoryDeviceArray class

The **Win32\_MemoryDeviceArray** association [WMI class](https://msdn.microsoft.com/library/aa393244) relates a memory device and the memory array in which it resides.

The following syntax is simplified from Managed Object Format (MOF) code and includes all of the inherited properties. Properties are listed in alphabetic order, not MOF order.

## Syntax

``` syntax
[Dynamic, Provider("CIMWin32"), UUID("{B24EF563-BBBE-11d2-ABFB-00805F538618}"), AMENDMENT]
class Win32_MemoryDeviceArray : CIM_Component
{
  Win32_MemoryArray  REF GroupComponent;
  Win32_MemoryDevice REF PartComponent;
};
```

## Members

The **Win32\_MemoryDeviceArray** class has these types of members:

-   [Properties](#properties)

### Properties

The **Win32\_MemoryDeviceArray** class has these properties.

<dl> <dt>

**GroupComponent**
</dt> <dd> <dl> <dt>

Data type: **Win32\_MemoryArray**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Key**](https://msdn.microsoft.com/library/aa392157), [**Override**](https://msdn.microsoft.com/library/aa393650) ("GroupComponent"), [**MappingStrings**](https://msdn.microsoft.com/library/aa393650) ("WMI\|Win32\_MemoryArray")
</dt> </dl>

A [**Win32\_MemoryArray**](win32-memoryarray.md) that represents the memory array part of the Win32\_MemoryDeviceArray association.

</dd> <dt>

**PartComponent**
</dt> <dd> <dl> <dt>

Data type: **Win32\_MemoryDevice**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Key**](https://msdn.microsoft.com/library/aa392157), [**Override**](https://msdn.microsoft.com/library/aa393650) ("PartComponent"), [**MappingStrings**](https://msdn.microsoft.com/library/aa393650) ("WMI\|Win32\_MemoryDevice")
</dt> </dl>

A [**Win32\_MemoryDevice**](win32-memorydevice.md) that represents a memory device part of the Win32\_MemoryDeviceArray association.

</dd> </dl>

## Remarks

The **Win32\_MemoryDeviceArray** class is derived from [**CIM\_Component**](cim-component.md).

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista<br/>                                                                |
| Minimum supported server<br/> | Windows Server 2008<br/>                                                          |
| Namespace<br/>                | Root\\CIMV2<br/>                                                                  |
| MOF<br/>                      | <dl> <dt>CIMWin32.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



## See also

<dl> <dt>

[**CIM\_Component**](cim-component.md)
</dt> <dt>

[Computer System Hardware Classes](computer-system-hardware-classes.md)
</dt> </dl>

 

 




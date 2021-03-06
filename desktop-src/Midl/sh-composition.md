---
title: sh_composition keyword
description: The \ sh\_composition\ keyword specifies the system object is a handle to a composition surface.
keywords:
- sh_composition keyword MIDL
topic_type:
- apiref
api_name:
- sh_composition
api_type:
- NA
ms.topic: reference
ms.date: 02/05/2021
---

# sh\_composition keyword

The **sh\_composition** keyword specifies that a `system_handle` holds a handle to a composition surface.

``` syntax
[system_handle(sh_composition)]

[system_handle(sh_composition, access-rights)]
```

## Parameters

This keyword is a parameter for [**system_handle**](system-handle.md).

The [**system_handle**](system-handle.md) documentation also contains details on optional use of the *access-rights* parameter. The default behavior is `DUPLICATE_SAME_ACCESS` per [**DuplicateHandle** function](/windows/win32/api/handleapi/nf-handleapi-duplicatehandle) specifications.

## Remarks

In order to use this keyword with the `system_handle` attribute, the `-target` flag must be set to `NT100` (or higher) when running midl.exe.

## Examples

``` syntax
interface MyInterface : IUnknown                         
{         
    HRESULT GetVisualSurface([out, system_handle(sh_composition)] HANDLE* visual);
}
```

## Requirements

| &nbsp; | &nbsp; |
|-|-|
| Minimum supported client | Windows 10 Anniversary Update (version 1607, build 14393) |
| Minimum supported server | Windows Server 2016 (build 14393) |

## See also

<dl> <dt>

[**system_handle**](system-handle.md)
</dt> <dt>

[DirectComposition](/windows/win32/api/_directcomp/)
</dt> <dt>

[**DCompositionCreateSurfaceHandle** function](/windows/win32/api/dcomp/nf-dcomp-dcompositioncreatesurfacehandle)
</dt> </dl>

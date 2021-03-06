---
title: "ICorProfilerObjectEnum Interface"
ms.date: "03/30/2017"
api_name: 
  - "ICorProfilerObjectEnum"
api_location: 
  - "mscorwks.dll"
api_type: 
  - "COM"
f1_keywords: 
  - "ICorProfilerObjectEnum"
helpviewer_keywords: 
  - "ICorProfilerObjectEnum interface [.NET Framework profiling]"
ms.assetid: 13e1651c-9523-40ef-bfd7-87fb94519f8b
topic_type: 
  - "apiref"
---
# ICorProfilerObjectEnum Interface
Provides methods to sequentially iterate through a collection of frozen objects that are generated by the [Ngen.exe (Native Image Generator)](../../tools/ngen-exe-native-image-generator.md).  
  
## Methods  
  
|Method|Description|  
|------------|-----------------|  
|[Clone Method](icorprofilerobjectenum-clone-method.md)|Gets an interface pointer to a copy of this `ICorProfilerObjectEnum` interface.|  
|[GetCount Method](icorprofilerobjectenum-getcount-method.md)|Gets the total number of frozen objects in the collection.|  
|[Next Method](icorprofilerobjectenum-next-method.md)|Gets the specified number of contiguous objects from a sequential collection of objects, starting at the enumerator's current position in the sequence.|  
|[Reset Method](icorprofilerobjectenum-reset-method.md)|Moves this enumerator's cursor to the starting position of the sequence.|  
|[Skip Method](icorprofilerobjectenum-skip-method.md)|Advances the cursor of this enumerator from its current position so that the specified number of elements are skipped.|  
  
## Remarks  
 The `ICorProfilerObjectEnum` interface is an enumerator. It allows the receiver of an array to pull elements from the sender at a rate that is appropriate for the receiver. In other words, the receiver is able to explicitly control the flow of array elements, thereby avoiding the problems related to passing large arrays as method parameters.  
  
 Use [ICorProfilerInfo2::EnumModuleFrozenObjects](icorprofilerinfo2-enummodulefrozenobjects-method.md) to obtain a pointer to the `ICorProfilerObjectEnum` interface.  
  
## Requirements  
 **Platforms:** See [System Requirements](../../get-started/system-requirements.md).  
  
 **Header:** CorProf.idl, CorProf.h  
  
 **Library:** CorGuids.lib  
  
 **.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]  
  
## See also

- [Profiling Interfaces](profiling-interfaces.md)
- [EnumModuleFrozenObjects Method](icorprofilerinfo2-enummodulefrozenobjects-method.md)

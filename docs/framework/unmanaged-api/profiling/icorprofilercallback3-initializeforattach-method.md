---
title: ICorProfilerCallback3::InitializeForAttach 方法
ms.date: 03/30/2017
api_name:
- ICorProfilerCallback3.InitializeForAttach Method
api_location:
- Mscorwks.dll
api_type:
- COM
f1_keywords:
- ICorProfilerCallback3::InitializeForAttach
helpviewer_keywords:
- InitializeForAttach method [.NET Framework profiling]
- ICorProfilerCallback3::InitializeForAttach method [.NET Framework profiling]
ms.assetid: bed097b3-6d52-46c9-bee7-ac7910b6fc3f
topic_type:
- apiref
author: mairaw
ms.author: mairaw
ms.openlocfilehash: 4ebdd76655124922008667898e38f873ad93598e
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54555591"
---
# <a name="icorprofilercallback3initializeforattach-method"></a>ICorProfilerCallback3::InitializeForAttach 方法
由公共语言运行时 (CLR) 调用，从而给予分析器一个在附加操作后可将其状态初始化的机会。  
  
## <a name="syntax"></a>语法  
  
```  
HRESULT InitializeForAttach(  
            [in] IUnknown * pCorProfilerInfoUnk,  
            [in] void * pvClientData,  
            [in] UINT cbClientData);  
```  
  
#### <a name="parameters"></a>参数  
 `pCorProfilerInfoUnk`  
 [in] `ICorProfilerInfo*` 接口的接口指针。  
  
 `pvClientData`  
 [in]对数据的指针传递到[iclrprofiling:: Attachprofiler](../../../../docs/framework/unmanaged-api/profiling/iclrprofiling-attachprofiler-method.md)中的方法及其`pvClientData`参数。 如果此参数为 NULL，则 `cbClientData` 将为 0（零）。 当 CLR 从 `InitializeForAttach` 返回时将释放此内存。  
  
 `cbClientData`  
 [in] `pvClientData` 指向的数据的大小（以字节为单位）。  
  
## <a name="remarks"></a>备注  
 CLR 调用 `InitializeForAttach` 以便给予分析器请求回调的机会。  
  
## <a name="requirements"></a>要求  
 **平台：** 请参阅[系统需求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** CorProf.idl, CorProf.h  
  
 **库：** CorGuids.lib  
  
 **.NET Framework 版本：**[!INCLUDE[net_current_v40plus](../../../../includes/net-current-v40plus-md.md)]  
  
## <a name="see-also"></a>请参阅
- [ICorProfilerCallback 接口](../../../../docs/framework/unmanaged-api/profiling/icorprofilercallback-interface.md)
- [ICorProfilerInfo3 接口](../../../../docs/framework/unmanaged-api/profiling/icorprofilerinfo3-interface.md)
- [Profiling 接口](../../../../docs/framework/unmanaged-api/profiling/profiling-interfaces.md)
- [分析](../../../../docs/framework/unmanaged-api/profiling/index.md)

---
title: ICorDebugValue::GetAddress 方法
ms.date: 03/30/2017
api_name:
- ICorDebugValue.GetAddress
api_location:
- mscordbi.dll
api_type:
- COM
f1_keywords:
- ICorDebugValue::GetAddress
helpviewer_keywords:
- ICorDebugValue::GetAddress method [.NET Framework debugging]
- GetAddress method, ICorDebugValue interface [.NET Framework debugging]
ms.assetid: a247c792-45e1-4538-9e1f-b46acca4a463
topic_type:
- apiref
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: b88c49ba93ff3c4cc3f5c7a656dfa5da6e82109e
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54559828"
---
# <a name="icordebugvaluegetaddress-method"></a>ICorDebugValue::GetAddress 方法
获取此"ICorDebugValue"对象，它是正在调试的过程中的地址。  
  
## <a name="syntax"></a>语法  
  
```  
HRESULT GetAddress (  
    [out] CORDB_ADDRESS   *pAddress  
);  
```  
  
#### <a name="parameters"></a>参数  
 `pAddress`  
 [out]指向`CORDB_ADDRESS`对象，它指定此值对象的地址。  
  
## <a name="remarks"></a>备注  
 如果值为不可用，则返回 0 （零）。 这可能是如果值为至少一部分在寄存器中或存储在垃圾回收器句柄 (`GCHandle`)。  
  
## <a name="requirements"></a>要求  
 **平台：** 请参阅[系统需求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** CorDebug.idl、 CorDebug.h  
  
 **库：** CorGuids.lib  
  
 **.NET Framework 版本：**[!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]  
  
## <a name="see-also"></a>请参阅


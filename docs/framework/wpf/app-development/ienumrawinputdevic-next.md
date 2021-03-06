---
title: IEnumRAWINPUTDEVIC:Next
ms.date: 03/30/2017
helpviewer_keywords:
- Next method [WPF]
ms.assetid: 3698b44d-510e-4d18-b32b-85f17188ee26
ms.openlocfilehash: a1f76bf42da9a311633de39e42dee2055fac4a27
ms.sourcegitcommit: 8f95d3a37e591963ebbb9af6e90686fd5f3b8707
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/23/2019
ms.locfileid: "56745180"
---
# <a name="ienumrawinputdevicnext"></a>IEnumRAWINPUTDEVIC:Next
枚举下一个`celt` [RAWINPUTDEVICE](/windows/desktop/api/winuser/ns-winuser-rawinputdevice)在枚举器的列表中，将它们中返回的结构`rgelt`以及中枚举元素的实际数目`pceltFetched`。  
  
## <a name="syntax"></a>语法  
  
```  
HRESULT Next(  
      [in] ULONG celt,  
      [out, size_is(celt), length_is(*pceltFetched)] RAWINPUTDEVICE *rgelt,  
      [out] ULONG *pceltFetched);  
```  
  
#### <a name="parameters"></a>参数  
 `celt`  
  
 [in]数[RAWINPUTDEVICE](/windows/desktop/api/winuser/ns-winuser-rawinputdevice)结构中返回`rgelt`。  
  
 `rgelt`  
  
 [out] celt 大小（或更大）的数组，用于接收枚举的 RAWINPUTDEVICE 结构。  
  
 `pceltFetched`  
  
 [out] 指向 `rgelt` 中实际提供的元素数量的指针。 如果 `rgelt` 为一，则调用方可传入 `NULL`。  
  
## <a name="property-valuereturn-value"></a>属性值/返回值  
 HRESULT：如果提供的元素数，则为 S_OK `celt`;否则为 S_FALSE。

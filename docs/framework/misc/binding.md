---
title: <binding>
ms.date: 03/30/2017
ms.topic: reference
ms.assetid: 666183d6-4d1f-45c7-ac64-bdf93ee8f36f
ms.openlocfilehash: fb51eb1962603439b89a203eb668dfb543049170
ms.sourcegitcommit: 14355b4b2fe5bcf874cac96d0a9e6376b567e4c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "55271468"
---
# <a name="binding"></a>\<binding>
可以使用 `binding` 元素来配置 Windows Communication Foundation (WCF) 提供的不同类型的预定义绑定。  
  
## <a name="system-provided-binding"></a>系统提供的绑定  
 系统提供的绑定可以消除 WCF 消息堆栈的复杂性。 使用系统提供的绑定的应用程序不需要对堆栈的完全控制权限。 在每个系统提供的绑定上公开的属性最适合绑定所针对的使用方案。  
  
 每个系统提供的绑定的配置节可以定义用于配置此绑定的一些配置。 每个配置均由唯一的名称进行标识。  
  
 无法向系统提供的绑定添加元素或属性。 为此，应该按照本主题的“自定义绑定”节中的描述来实现自定义绑定。 可以定义一个自定义绑定，该自定义绑定将完全模仿系统提供的绑定，并添加用户应用程序希望获得其控制权限的一些设置。  
  
## <a name="custom-binding"></a>自定义绑定  
 自定义绑定提供了对 WCF 消息堆栈的完全控制。 单个绑定按照堆栈元素在堆栈上出现的顺序来指定它们的配置元素，从而定义消息堆栈。 每个元素都定义和配置了该堆栈的一个元素。 在每个自定义绑定中，必须有且只能有一个 `transport` 元素。 如果没有该元素，消息堆栈将是不完整的。  
  
 元素在堆栈中出现的顺序非常重要，因为在将操作应用于消息时会采用该顺序。 建议的堆栈元素顺序如下：  
  
1.  事务（可选）  
  
2.  可靠消息（可选）  
  
3.  安全（可选）  
  
4.  编码器  
  
5.  传输  
  
 自定义绑定由其 `name` 特性来标识。  
  
## <a name="see-also"></a>请参阅
- <xref:System.ServiceModel.Configuration.BindingsSection>
- <xref:System.ServiceModel.Channels.Binding>
- <xref:System.ServiceModel.Channels.BindingElement>
- [绑定](../../../docs/framework/wcf/bindings.md)
- [自定义绑定](../../../docs/framework/wcf/extending/custom-bindings.md)
- [\<customBinding>](../../../docs/framework/configure-apps/file-schema/wcf/custombinding.md)

---
title: 如何：设置笔颜色
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
- cpp
helpviewer_keywords:
- pens [Windows Forms], setting color
- colored pens
ms.assetid: a9df06f9-a6d5-4d9b-a2d1-583943540775
ms.openlocfilehash: d0402a7d6bb641ef6d97eb41bc25f3c59b3b4250
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54569435"
---
# <a name="how-to-set-the-color-of-a-pen"></a>如何：设置笔颜色
此示例将更改的预先存在的颜色<xref:System.Drawing.Pen>对象  
  
## <a name="example"></a>示例  
 [!code-cpp[System.Drawing.ConceptualHowTos#9](../../../../samples/snippets/cpp/VS_Snippets_Winforms/System.Drawing.ConceptualHowTos/cpp/form1.cpp#9)]
 [!code-csharp[System.Drawing.ConceptualHowTos#9](../../../../samples/snippets/csharp/VS_Snippets_Winforms/System.Drawing.ConceptualHowTos/CS/form1.cs#9)]
 [!code-vb[System.Drawing.ConceptualHowTos#9](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/System.Drawing.ConceptualHowTos/VB/form1.vb#9)]  
  
## <a name="compiling-the-code"></a>编译代码  
 此示例需要：  
  
-   一个<xref:System.Drawing.Pen>名为对象`myPen`。  
  
## <a name="robust-programming"></a>可靠编程  
 应调用<xref:System.Drawing.Pen.Dispose%2A>消耗系统资源的对象 (如<xref:System.Drawing.Pen>对象) 结束使用它们之后。  
  
## <a name="see-also"></a>请参阅
- <xref:System.Drawing.Pen>
- [图形编程入门](../../../../docs/framework/winforms/advanced/getting-started-with-graphics-programming.md)
- [如何：创建钢笔](../../../../docs/framework/winforms/advanced/how-to-create-a-pen.md)
- [使用笔绘制直线和形状](../../../../docs/framework/winforms/advanced/using-a-pen-to-draw-lines-and-shapes.md)
- [GDI+ 中的笔、直线和矩形](../../../../docs/framework/winforms/advanced/pens-lines-and-rectangles-in-gdi.md)

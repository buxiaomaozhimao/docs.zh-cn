---
title: 如何：使元素就地旋转
ms.date: 03/30/2017
helpviewer_keywords:
- graphics [WPF], spinning elements
- spinning elements [WPF]
ms.assetid: 1f011976-8b07-4c31-9faf-019e0ddaa24c
ms.openlocfilehash: a4fcd54d673fe8d71b83ff623eabfd7f4f500e7c
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54734524"
---
# <a name="how-to-make-an-element-spin-in-place"></a>如何：使元素就地旋转
此示例演示如何使某个元素通过使用旋转<xref:System.Windows.Media.RotateTransform>和一个<xref:System.Windows.Media.Animation.DoubleAnimation>。  
  
 下面的示例应用<xref:System.Windows.Media.RotateTransform>到<xref:System.Windows.UIElement.RenderTransform%2A>元素的属性。 该示例使用<xref:System.Windows.Media.Animation.DoubleAnimation>进行动画处理<xref:System.Windows.Media.RotateTransform.Angle%2A>的<xref:System.Windows.Media.RotateTransform>。 若要使元素就地旋转，该示例设置<xref:System.Windows.UIElement.RenderTransformOrigin%2A>到点 （0.5，0.5） 元素的属性。  
  
## <a name="example"></a>示例  
 [!code-xaml[transformanimations_snip#11](../../../../samples/snippets/xaml/VS_Snippets_Wpf/transformanimations_snip/XAML/RotateAboutCenterExample.xaml#11)]  
  
 有关完整示例，其中包括转换的更多示例，请参阅[2d 转换示例](https://go.microsoft.com/fwlink/?LinkID=158252)。  
  
## <a name="see-also"></a>请参阅
- [动画概述](../../../../docs/framework/wpf/graphics-multimedia/animation-overview.md)
- [转换概述](../../../../docs/framework/wpf/graphics-multimedia/transforms-overview.md)

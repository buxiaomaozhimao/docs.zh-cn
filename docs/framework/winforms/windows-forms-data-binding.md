---
title: Windows 窗体数据绑定
ms.date: 03/30/2017
helpviewer_keywords:
- data [Windows Forms]
- Windows Forms, data binding
- data [Windows Forms], architecture
- Windows Forms controls, data binding
ms.assetid: c3826d8e-ea25-4ad4-a669-45bfb19192aa
ms.openlocfilehash: b33ad9d78230588b9c1afd5d59fd0333e2cd18a6
ms.sourcegitcommit: 8f95d3a37e591963ebbb9af6e90686fd5f3b8707
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/23/2019
ms.locfileid: "56747056"
---
# <a name="windows-forms-data-binding"></a>Windows 窗体数据绑定
Windows 窗体中的数据绑定使你可以显示和更改窗体上的控件中的数据源的信息。 可以绑定到传统数据源和几乎任何包含数据的结构。  
  
## <a name="in-this-section"></a>本节内容  
 [数据绑定和 Windows 窗体](../../../docs/framework/winforms/data-binding-and-windows-forms.md)  
 提供了 Windows 窗体中的数据绑定概述。  
  
 [Windows 窗体支持的数据源](../../../docs/framework/winforms/data-sources-supported-by-windows-forms.md)  
 介绍了可以与 Windows 窗体一起使用的数据源。  
  
 [与数据绑定相关的接口](../../../docs/framework/winforms/interfaces-related-to-data-binding.md)  
 介绍了几种与 Windows 窗体数据绑定一起使用的接口。  
  
 [如何：在 Windows 窗体中导航数据](../../../docs/framework/winforms/how-to-navigate-data-in-windows-forms.md)  
 演示如何在数据源中的项之间进行导航。  
  
 [Windows 窗体数据绑定中的更改通知](../../../docs/framework/winforms/change-notification-in-windows-forms-data-binding.md)  
 描述了 Windows 窗体数据绑定的不同类型的更改通知。  
  
 [如何：实现 INotifyPropertyChanged 接口](../../../docs/framework/winforms/how-to-implement-the-inotifypropertychanged-interface.md)  
 演示如何实现 <xref:System.ComponentModel.INotifyPropertyChanged> 接口。 该接口与属性在业务对象上更改的绑定控件通信  
  
 [如何：应用 PropertyNameChanged 模式](../../../docs/framework/winforms/how-to-apply-the-propertynamechanged-pattern.md)  
 演示如何将应用*PropertyName*Changed 模式 Windows 窗体用户控件的属性。  
  
 [如何：实现 ITypedList 接口](../../../docs/framework/winforms/how-to-implement-the-itypedlist-interface.md)  
 演示如何通过实现 <xref:System.ComponentModel.ITypedList> 接口，启用可绑定列表的架构发现。  
  
 [如何：实现 IListSource 接口](../../../docs/framework/winforms/how-to-implement-the-ilistsource-interface.md)  
 演示如何实现 <xref:System.ComponentModel.IListSource> 接口，以创建可绑定的类，其不实现 <xref:System.Collections.IList>，但提供其他位置的列表。  
  
 [如何：确保多个控件绑定到相同的数据源保持同步](../../../docs/framework/winforms/multiple-controls-bound-to-data-source-synchronized.md)  
 演示如何处理 <xref:System.Windows.Forms.BindingSource.BindingComplete> 事件，以确保所有绑定到数据源的控件保持同步。  
  
 [如何：请确保子表中的选定的行保持在正确的位置](../../../docs/framework/winforms/ensure-the-selected-row-in-a-child-table-correct.md)  
 演示如何确保在更改父表的字段时，选定的子表行不会更改。  
  
 另请参阅[与数据绑定相关的接口](interfaces-related-to-data-binding.md)，[如何：在 Windows 窗体中导航数据](how-to-navigate-data-in-windows-forms.md)，和[如何：创建 Windows 窗体上的简单绑定控件](how-to-create-a-simple-bound-control-on-a-windows-form.md)。  
  
## <a name="reference"></a>参考  
 <xref:System.Windows.Forms.Binding?displayProperty=nameWithType>  
 描述表示可绑定组件和数据源之间的绑定的类。  
  
 <xref:System.Windows.Forms.BindingSource?displayProperty=nameWithType>  
 描述用来封装数据源以绑定到控件的类。  
  
## <a name="related-sections"></a>相关章节  
 [BindingSource 组件](../../../docs/framework/winforms/controls/bindingsource-component.md)  
 包含演示如何使用 <xref:System.Windows.Forms.BindingSource> 组件的主题列表。  
  
 [DataGridView 控件](../../../docs/framework/winforms/controls/datagridview-control-windows-forms.md)  
 提供演示如何使用可绑定的 datagrid 控件的主题列表。  
  
 另请参阅[Visual Studio 中访问数据](/visualstudio/data-tools/accessing-data-in-visual-studio)。

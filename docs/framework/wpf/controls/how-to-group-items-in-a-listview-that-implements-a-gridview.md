---
title: 如何：对实现 GridView 的 ListView 中的项进行分组
ms.date: 03/30/2017
helpviewer_keywords:
- ListView controls [WPF], grouping items with GridViews
- grouping items in ListViews implementing GridViews [WPF]
- GridView controls [WPF], grouping items
ms.assetid: eebef25b-ddc6-424e-a66d-ea228d1bf33d
ms.openlocfilehash: 1570eab70dae690f508975162b7553de92be6f12
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54664351"
---
# <a name="how-to-group-items-in-a-listview-that-implements-a-gridview"></a>如何：对实现 GridView 的 ListView 中的项进行分组
此示例演示如何显示组中的项数<xref:System.Windows.Controls.GridView>视图模式<xref:System.Windows.Controls.ListView>控件。  
  
## <a name="example"></a>示例  
 若要显示组中的项数<xref:System.Windows.Controls.ListView>，定义<xref:System.Windows.Data.CollectionViewSource>。 下面的示例演示<xref:System.Windows.Data.CollectionViewSource>分组数据项的值根据`Catalog`数据字段。  
  
 [!code-xaml[GridViewWithGroups#GroupingCollectionViewSource](../../../../samples/snippets/csharp/VS_Snippets_Wpf/GridViewWithGroups/CS/Window1.xaml#groupingcollectionviewsource)]  
  
 下面的示例设置<xref:System.Windows.Controls.ItemsControl.ItemsSource%2A>有关<xref:System.Windows.Controls.ListView>到<xref:System.Windows.Data.CollectionViewSource>前面的示例定义。 该示例还定义了<xref:System.Windows.Controls.ItemsControl.GroupStyle%2A>实现<xref:System.Windows.Controls.Expander>控件。  
  
 [!code-xaml[GridViewWithGroups#ListViewGroups](../../../../samples/snippets/csharp/VS_Snippets_Wpf/GridViewWithGroups/CS/Window1.xaml#listviewgroups)]  
[!code-xaml[GridViewWithGroups#ListViewEnd](../../../../samples/snippets/csharp/VS_Snippets_Wpf/GridViewWithGroups/CS/Window1.xaml#listviewend)]  
  
## <a name="see-also"></a>请参阅
- <xref:System.Windows.Controls.ListView>
- <xref:System.Windows.Controls.GridView>
- [帮助主题](../../../../docs/framework/wpf/controls/listview-how-to-topics.md)
- [ListView 概述](../../../../docs/framework/wpf/controls/listview-overview.md)
- [GridView 概述](../../../../docs/framework/wpf/controls/gridview-overview.md)

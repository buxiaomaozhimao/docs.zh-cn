---
title: 如何：Windows 窗体 ListView 控件中显示图标
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- ListView control [Windows Forms], displaying icons
- icons [Windows Forms], displaying for ListView controls
- lists [Windows Forms], displaying icons
- ImageList component [Windows Forms], with ListView control
- list views [Windows Forms], displaying icons
ms.assetid: 9d577542-8595-429b-99e5-078770ec9d35
ms.openlocfilehash: 3c3df1fb38c9fbcf672e9ffcd8c0aa3c881be00b
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54510619"
---
# <a name="how-to-display-icons-for-the-windows-forms-listview-control"></a>如何：Windows 窗体 ListView 控件中显示图标
Windows 窗体<xref:System.Windows.Forms.ListView>控件可以显示来自三个图像列表的图标。 列表、 详细信息，以及 SmallIcon 视图中显示图像的图像列表中指定<xref:System.Windows.Forms.ListView.SmallImageList%2A>属性。 图标视图将从图像列表中指定的图像显示<xref:System.Windows.Forms.ListView.LargeImageList%2A>属性。 列表视图还可以显示一组额外的图标，在中设置<xref:System.Windows.Forms.ListView.StateImageList%2A>属性旁边的大或小图标。 有关图像列表的详细信息，请参阅[ImageList 组件](../../../../docs/framework/winforms/controls/imagelist-component-windows-forms.md)和[如何：添加或删除图像与 Windows 窗体 ImageList 组件](../../../../docs/framework/winforms/controls/how-to-add-or-remove-images-with-the-windows-forms-imagelist-component.md)。  
  
### <a name="to-display-images-in-a-list-view"></a>在列表视图中显示图像  
  
1.  设置相应的属性 —<xref:System.Windows.Forms.ListView.SmallImageList%2A>， <xref:System.Windows.Forms.ListView.LargeImageList%2A>，或<xref:System.Windows.Forms.ListView.StateImageList%2A>— 对现有<xref:System.Windows.Forms.ImageList>你想要使用的组件。  
  
     可以在属性窗口中，使用在设计器或在代码中设置这些属性。  
  
     [!code-csharp[System.Windows.Forms.ListViewLegacyTopics#41](../../../../samples/snippets/csharp/VS_Snippets_Winforms/System.Windows.Forms.ListViewLegacyTopics/CS/Class1.cs#41)]
     [!code-vb[System.Windows.Forms.ListViewLegacyTopics#41](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/System.Windows.Forms.ListViewLegacyTopics/VB/Class1.vb#41)]  
  
2.  设置<xref:System.Windows.Forms.ListViewItem.ImageIndex%2A>或<xref:System.Windows.Forms.ListViewItem.StateImageIndex%2A>每个都有一个关联的图标的列表项的属性。  
  
     可以设置这些属性，在代码中，或在**列表视图项集合编辑器**。 若要打开**列表视图项集合编辑器**，单击省略号按钮 (![VisualStudioEllipsesButton 屏幕快照](../../../../docs/framework/winforms/media/vbellipsesbutton.png "vbEllipsesButton")) 旁边<xref:System.Windows.Forms.ListView.Items%2A>上的属性**属性**窗口。  
  
     [!code-csharp[System.Windows.Forms.ListViewLegacyTopics#42](../../../../samples/snippets/csharp/VS_Snippets_Winforms/System.Windows.Forms.ListViewLegacyTopics/CS/Class1.cs#42)]
     [!code-vb[System.Windows.Forms.ListViewLegacyTopics#42](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/System.Windows.Forms.ListViewLegacyTopics/VB/Class1.vb#42)]  
  
## <a name="see-also"></a>请参阅
- [ListView 控件概述](../../../../docs/framework/winforms/controls/listview-control-overview-windows-forms.md)
- [如何：添加和删除使用 Windows 窗体 ListView 控件的项](../../../../docs/framework/winforms/controls/how-to-add-and-remove-items-with-the-windows-forms-listview-control.md)
- [如何：将列添加到 Windows 窗体 ListView 控件](../../../../docs/framework/winforms/controls/how-to-add-columns-to-the-windows-forms-listview-control.md)
- [如何：将自定义信息添加到 TreeView 或 ListView 控件 （Windows 窗体）](../../../../docs/framework/winforms/controls/add-custom-information-to-a-treeview-or-listview-control-wf.md)
- [ImageList 组件](../../../../docs/framework/winforms/controls/imagelist-component-windows-forms.md)

---
title: 如何：使列成为只读，Windows 窗体 DataGridView 控件中
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- data grids [Windows Forms], read-only columns
- DataGridView control [Windows Forms], read-only columns
ms.assetid: 2bb73ebb-1a55-4362-9fda-e50574c087d5
ms.openlocfilehash: 6fbdf661983d39ad4793946f10deb3e224f2f711
ms.sourcegitcommit: 07c4368273b446555cb2c85397ea266b39d5fe50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "56583623"
---
# <a name="how-to-make-columns-read-only-in-the-windows-forms-datagridview-control"></a>如何：使列成为只读，Windows 窗体 DataGridView 控件中
无需对所有的数据进行编辑。 在 <xref:System.Windows.Forms.DataGridView> 控件中，列 <xref:System.Windows.Forms.DataGridViewColumn.ReadOnly%2A> 属性值确定用户是否可在该列中编辑单元格。 有关如何使控件完全只读的信息，请参阅[如何：防止行中添加和删除 Windows 窗体 DataGridView 控件](../../../../docs/framework/winforms/controls/prevent-row-addition-and-deletion-datagridview.md)。  
  
 Visual Studio 中对此任务提供支持。  另请参阅[如何：将列设为只读、 只在 Windows 窗体 DataGridView 控件使用设计器](make-columns-read-only-in-the-datagrid-using-the-designer.md)。  
  
### <a name="to-make-a-column-read-only-programmatically"></a>以编程方式将列设置为只读  
  
-   将 <xref:System.Windows.Forms.DataGridViewColumn.ReadOnly%2A?displayProperty=nameWithType> 属性设置为 `true`。  
  
     [!code-csharp[System.Windows.Forms.DataGridViewMisc#064](../../../../samples/snippets/csharp/VS_Snippets_Winforms/System.Windows.Forms.DataGridViewMisc/CS/datagridviewmisc.cs#064)]
     [!code-vb[System.Windows.Forms.DataGridViewMisc#064](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/System.Windows.Forms.DataGridViewMisc/VB/datagridviewmisc.vb#064)]  
  
## <a name="compiling-the-code"></a>编译代码  
 此示例需要：  
  
-   名为 `dataGridView1` 的 <xref:System.Windows.Forms.DataGridView> 控件具有名为 `CompanyName` 的列。  
  
-   对 <xref:System?displayProperty=nameWithType> 和 <xref:System.Windows.Forms?displayProperty=nameWithType> 程序集的引用。  
  
## <a name="see-also"></a>请参阅
- <xref:System.Windows.Forms.DataGridView>
- <xref:System.Windows.Forms.DataGridView.Columns%2A?displayProperty=nameWithType>
- <xref:System.Windows.Forms.DataGridViewColumn.ReadOnly%2A?displayProperty=nameWithType>
- [Windows 窗体 DataGridView 控件中的列、行和单元格基本功能](../../../../docs/framework/winforms/controls/basic-column-row-and-cell-features-wf-datagridview-control.md)
- [如何：防止添加和 Windows 窗体 DataGridView 控件中的删除行](../../../../docs/framework/winforms/controls/prevent-row-addition-and-deletion-datagridview.md)

---
title: 如何：添加或删除映像使用 Windows 窗体 ImageList 组件
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
- cpp
helpviewer_keywords:
- images [Windows Forms], removing from ImageList component
- images [Windows Forms], storing for controls
- ImageList component [Windows Forms], adding images
- ImageList component [Windows Forms], removing images
- images [Windows Forms], adding to ImageList component
- images [Windows Forms], displaying with controls
ms.assetid: c5eacc56-f769-4e2e-bfb7-f756620913db
ms.openlocfilehash: a81cf11ea5ca405e2013b7c7375a863aeb1f110f
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54609611"
---
# <a name="how-to-add-or-remove-images-with-the-windows-forms-imagelist-component"></a>如何：添加或删除映像使用 Windows 窗体 ImageList 组件
Windows 窗体<xref:System.Windows.Forms.ImageList>组件通常用图像填充之前与控件关联。 但是，可以添加和删除与控件关联的图像列表后的图像。  
  
> [!NOTE]
>  当删除映像时，请确认<xref:System.Windows.Forms.ButtonBase.ImageIndex%2A>任何关联控件的属性是否仍然有效。  
  
### <a name="to-add-images-programmatically"></a>若要以编程方式添加映像  
  
-   使用<xref:System.Windows.Forms.ImageList.ImageCollection.Add%2A>图像列表的方法<xref:System.Windows.Forms.ImageList.Images%2A>属性。  
  
     在下面的代码示例中，将路径设置的映像的位置是**我的文档**文件夹。 使用此位置是因为您可以假定大多数运行 Windows 操作系统的计算机将包含此文件夹。 选择此位置还使得用户可以具有最少的系统的访问级别更多安全地运行应用程序。 下面的代码示例，则需要具有的窗体<xref:System.Windows.Forms.ImageList>已添加的控件。  
  
    ```vb  
    Public Sub LoadImage()  
       Dim myImage As System.Drawing.Image = _  
         Image.FromFile _  
       (System.Environment.GetFolderPath _  
       (System.Environment.SpecialFolder.Personal) _  
       & "\Image.gif")  
       ImageList1.Images.Add(myImage)  
    End Sub  
    ```  
  
    ```csharp  
    public void addImage()  
    {  
    // Be sure that you use an appropriate escape sequence (such as the   
    // @) when specifying the location of the file.  
       System.Drawing.Image myImage =   
         Image.FromFile  
       (System.Environment.GetFolderPath  
       (System.Environment.SpecialFolder.Personal)  
       + @"\Image.gif");  
       imageList1.Images.Add(myImage);  
    }  
    ```  
  
    ```cpp  
    public:  
       void addImage()  
       {  
       // Replace the bold image in the following sample   
       // with your own icon.  
       // Be sure that you use an appropriate escape sequence (such as   
       // \\) when specifying the location of the file.  
          System::Drawing::Image ^ myImage =   
             Image::FromFile(String::Concat(  
             System::Environment::GetFolderPath(  
             System::Environment::SpecialFolder::Personal),  
             "\\Image.gif"));  
          imageList1->Images->Add(myImage);  
       }  
    ```  
  
### <a name="to-add-images-with-a-key-value"></a>若要添加图像与密钥值。  
  
-   使用之一<xref:System.Windows.Forms.ImageList.ImageCollection.Add%2A>方法的图像列表的<xref:System.Windows.Forms.ImageList.Images%2A>采用键值的属性。  
  
     在下面的代码示例中，将路径设置的映像的位置是**我的文档**文件夹。 使用此位置是因为您可以假定大多数运行 Windows 操作系统的计算机将包含此文件夹。 选择此位置还使得用户可以具有最少的系统的访问级别更多安全地运行应用程序。 下面的代码示例，则需要具有的窗体<xref:System.Windows.Forms.ImageList>已添加的控件。  
  
    ```vb  
    Public Sub LoadImage()  
       Dim myImage As System.Drawing.Image = _  
         Image.FromFile _  
       (System.Environment.GetFolderPath _  
       (System.Environment.SpecialFolder.Personal) _  
       & "\Image.gif")  
       ImageList1.Images.Add("myPhoto", myImage)  
    End Sub  
    ```  
  
```csharp  
public void addImage()  
{  
// Be sure that you use an appropriate escape sequence (such as the   
// @) when specifying the location of the file.  
   System.Drawing.Image myImage =   
     Image.FromFile  
   (System.Environment.GetFolderPath  
   (System.Environment.SpecialFolder.Personal)  
   + @"\Image.gif");  
   imageList1.Images.Add("myPhoto", myImage);  
}  
```  
  
### <a name="to-remove-all-images-programmatically"></a>若要以编程方式删除所有映像  
  
-   使用<xref:System.Windows.Forms.ImageList.ImageCollection.Remove%2A>方法来删除单一映像  
  
     -  
  
     使用<xref:System.Windows.Forms.ImageList.ImageCollection.Clear%2A>方法清除图像列表中的所有映像。  
  
    ```vb  
    ' Removes the first image in the image list  
    ImageList1.Images.Remove(myImage)  
    ' Clears all images in the image list  
    ImageList1.Images.Clear()  
    ```  
  
```csharp  
// Removes the first image in the image list.  
imageList1.Images.Remove(myImage);  
// Clears all images in the image list.  
imageList1.Images.Clear();  
```  
  
### <a name="to-remove-images-by-key"></a>删除密钥的图像  
  
-   使用<xref:System.Windows.Forms.ImageList.ImageCollection.RemoveByKey%2A>方法删除其密钥的单一映像。  
  
    ```vb  
    ' Removes the image named "myPhoto" from the list.  
    ImageList1.Images.RemoveByKey("myPhoto")  
    ```  
  
```csharp  
// Removes the image named "myPhoto" from the list.  
imageList1.Images.RemoveByKey("myPhoto");  
```  
  
## <a name="see-also"></a>请参阅
- [ImageList 组件](../../../../docs/framework/winforms/controls/imagelist-component-windows-forms.md)
- [ImageList 组件概述](../../../../docs/framework/winforms/controls/imagelist-component-overview-windows-forms.md)
- [图像、位图和图元文件](../../../../docs/framework/winforms/advanced/images-bitmaps-and-metafiles.md)

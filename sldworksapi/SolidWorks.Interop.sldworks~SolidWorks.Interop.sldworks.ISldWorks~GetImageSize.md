<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetImageSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetImageSize Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetImageSize Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Small*
:   Small image size suitable for the current DPI setting of the display device

*Medium*
:   Medium image size suitable for the current DPI setting of the display device

*Large*
:   Large image size suitable for the current DPI setting of the display device

Gets:

* small, medium, and large image sizes suitable for the current DPI setting of the display device.* default image size for the current DPI setting of the display device for images that are not based on the SOLIDWORKS icon size setting.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetImageSize( _    ByRef Small As System.Integer, _    ByRef Medium As System.Integer, _    ByRef Large As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Small As System.Integer Dim Medium As System.Integer Dim Large As System.Integer Dim value As System.Integer   value = instance.GetImageSize(Small, Medium, Large) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetImageSize(     out System.int Small,    out System.int Medium,    out System.int Large ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetImageSize(  &   [Out] System.int Small, &   [Out] System.int Medium, &   [Out] System.int Large ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Small*
:   Small image size suitable for the current DPI setting of the display device

*Medium*
:   Medium image size suitable for the current DPI setting of the display device

*Large*
:   Large image size suitable for the current DPI setting of the display device

#### Return Value

Default image size for the current DPI setting of the display device for images that are not based on the SOLIDWORKS icon size setting as defined in swImageSizeToUse\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetImageSize.

# ![](dotnetimages/collapse.gif)Example

[Create Flyouts in the CommandManager (C#)](Create_Flyouts_in_the_CommandManager_Example_CSharp.htm)

[Create Flyouts in the CommandManager (VB.NET)](Create_Flyouts_in_the_CommandManager_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can use this method to determine the correct size for:

* buttons for your PropertyManager pages.* icons for your macro features.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ICommandGroup::IconList Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~IconList.html)

[ICommandGroup::MainIconList Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~MainIconList.html)

[ICommandManager::CreateFlyoutGroup2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~CreateFlyoutGroup2.html)

[IFlyoutGroup::IconList Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup~IconList.html)

[IFlyoutGroup::MainIconList Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlyoutGroup~MainIconList.html)

[IFrame::AddMenuPopupIcon3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuPopupIcon3.html)

[IPropertyManagerPageBitmapButton::SetBitmapsByName3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmapButton~SetBitmapsByName3.html)

[ISldWorks::AddMenuItem5 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenuItem5.html)

[ISldWorks::AddToolbar5 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddToolbar5.html)

[ITaskPaneView::AddCustomButton2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITaskpaneView~AddCustomButton2.html)

[ISldWorks::CreateTaskpaneView3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CreateTaskpaneView3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0
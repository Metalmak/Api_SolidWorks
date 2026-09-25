<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~CreateTaskpaneView3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateTaskpaneView3 Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : CreateTaskpaneView3 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ImageList*
:   Array of strings of paths to six image files for the tab of this Task Pane view (see **Remarks**)

*ToolTip*
:   Tool tip for this Task Pane view

Creates an application-level Task Pane view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateTaskpaneView3( _    ByVal ImageList As System.Object, _    ByVal ToolTip As System.String _ ) As TaskpaneView ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim ImageList As System.Object Dim ToolTip As System.String Dim value As TaskpaneView   value = instance.CreateTaskpaneView3(ImageList, ToolTip) ``` | |

| C# |  |
| --- | --- |
| ``` TaskpaneView CreateTaskpaneView3(     System.object ImageList,    System.string ToolTip ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` TaskpaneView^ CreateTaskpaneView3(  &   System.Object^ ImageList, &   System.String^ ToolTip ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ImageList*
:   Array of strings of paths to six image files for the tab of this Task Pane view (see **Remarks**)

*ToolTip*
:   Tool tip for this Task Pane view

#### Return Value

[Task Pane view](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITaskpaneView.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::CreateTaskpaneView3.

# ![](dotnetimages/collapse.gif)Example

[Add Task Pane View (VBA)](Add_Task_Pane_View_Example_VB.htm)

[Add Task Pane View (VB.NET)](Add_Task_Pane_View_Example_VBNET.htm)

[Add Task Pane View (C#)](Add_Task_Pane_View_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method supports high resolution screens with high resolution operating system scaling options.

ImageList contains paths to PNG or BMP images in six pixel sizes:

* 20 X 20* 32 X 32* 40 X 40* 64 X 64* 96 X 96* 128 X 128

The SOLIDWORKS user interface displays icons in three sizes: small, medium and large. After using this method to specify an image in six sizes, SOLIDWORKS selects the appropriate images to display as required by the current screen resolution or operating system scale.

| If OS scale is... | Then SOLIDWORKS icon... | Uses image pixel size... |
| --- | --- | --- |
| 100% | Small | 20X20 |
|  | Medium | 32X32 |
|  | Large | 40X40 |
| 150% | Small | 32X32 |
|  | Medium | 40X40 |
|  | Large | 64X64 |
| 200% | Small | 40X40 |
|  | Medium | 64X64 |
|  | Large | 96X96 |
| 250% | Small | 64X64 |
|  | Medium | 96X96 |
|  | Large | 128X128 |

The images should use a 256-color palette and gray (192, 192, 192) for transparent areas.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::ActivateTaskPane Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ActivateTaskPane.html)

[ISldWorks::RefreshTaskpaneContent Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RefreshTaskpaneContent.html)

[ISldWorks::TaskPaneIsPinned Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~TaskPaneIsPinned.html)

[ISldWorks::GetImageSize Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetImageSize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0
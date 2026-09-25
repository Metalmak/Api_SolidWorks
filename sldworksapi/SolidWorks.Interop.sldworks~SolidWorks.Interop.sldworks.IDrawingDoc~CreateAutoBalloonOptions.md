<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateAutoBalloonOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateAutoBalloonOptions Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : CreateAutoBalloonOptions Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Creates an object that stores auto balloon options.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateAutoBalloonOptions() As AutoBalloonOptions ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim value As AutoBalloonOptions   value = instance.CreateAutoBalloonOptions() ``` | |

| C# |  |
| --- | --- |
| ``` AutoBalloonOptions CreateAutoBalloonOptions() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` AutoBalloonOptions^ CreateAutoBalloonOptions(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

[IAutoBalloonOptions](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAutoBalloonOptions.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::CreateAutoBalloonOptions.

# ![](dotnetimages/collapse.gif)Example

[Add Autoballoons to Drawing (C#)](Add_Autoballoon_to_Face_Example_CSharp.htm)

[Add Autoballoons to Drawing (VB.NET)](Add_Autoballoon_to_Face_Example_VBNET.htm)

[Add Autoballoons to Drawing (VBA)](Add_Autoballoon_to_Face_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To automatically create BOM balloons:

1. Select one or more views or sheets for which to automatically create BOM balloons.

   - Call this method to create an [IAutoBalloonOptions](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAutoBalloonOptions.html) object.

     - Set the properties on the IAutoBalloonOptions object.

       - Pass the IAutoBalloonOptions object in a call to [IDrawingDoc::AutoBalloon5](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~AutoBalloon5.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IModelDocExtension::CreateBalloonOptions Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CreateBalloonOptions.html)

[IModelDocExtension::CreateStackedBalloonOptions Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CreateStackedBalloonOptions.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0
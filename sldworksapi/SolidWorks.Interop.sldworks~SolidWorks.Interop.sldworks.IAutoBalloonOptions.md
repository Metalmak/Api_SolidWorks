<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAutoBalloonOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAutoBalloonOptions Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAutoBalloonOptions_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IAutoBalloonOptions Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to auto balloon options.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IAutoBalloonOptions ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAutoBalloonOptions ``` | |

| C# |  |
| --- | --- |
| ``` public interface IAutoBalloonOptions ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IAutoBalloonOptions ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AutoBalloonOptions.

# ![](dotnetimages/collapse.gif)Example

[Add Auto Balloons to Drawing (VBA)](Add_Autoballoon_to_Face_Example_VB.htm)

[Add Auto Balloons to Drawing (VB.NET)](Add_Autoballoon_to_Face_Example_VBNET.htm)

[Add Auto Balloons to Drawing (C#)](Add_Autoballoon_to_Face_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To automatically create BOM balloons:

1. Select one or more views or sheets for which to automatically create BOM balloons.

   - Call [IDrawingDoc::CreateAutoBalloonOptions](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~CreateAutoBalloonOptions.html) to create IAutoBalloonOptions object.

     - Set the properties on IAutoBalloonOptions.

       - Pass IAutoBalloonOptions in a call to [IDrawingDoc::AutoBalloon5](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~AutoBalloon5.html).

# ![](dotnetimages/collapse.gif)Accessors

[IDrawingDoc::CreateAutoBalloonOptions](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~CreateAutoBalloonOptions.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[AutoBalloonOptions](SWObjectModel.pdf#AutoBalloonOptions)

# ![](dotnetimages/collapse.gif)See Also

####

[IAutoBalloonOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAutoBalloonOptions_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IBalloonOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBalloonOptions.html)

[IStackedBalloonOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStackedBalloonOptions.html)
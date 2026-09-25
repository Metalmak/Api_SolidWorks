<!-- source: swinspectionapi/SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionProjectData~AutoBalloon.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Inspection API Help | Send comments on this topic. |
| AutoBalloon Property (IInspectionProjectData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swinspectionAddIn Namespace](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn_namespace.html) > [IInspectionProjectData Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionProjectData.html) : AutoBalloon Property (IInspectionProjectData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets whether to autoballoon drawings in this inspection project.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property AutoBalloon As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IInspectionProjectData Dim value As System.Boolean   instance.AutoBalloon = value   value = instance.AutoBalloon ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AutoBalloon {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool AutoBalloon {    System.bool get();    void set ( &   System.bool value); } ``` | |

#### Property Value

True to autoballoon the drawing, false to manually add balloons to the drawing

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See InspectionProjectData properties.

# ![](dotnetimages/collapse.gif)See Also

####

[IInspectionProjectData Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionProjectData.html)

[IInspectionProjectData Members](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionProjectData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Inspection API 2022 FCS
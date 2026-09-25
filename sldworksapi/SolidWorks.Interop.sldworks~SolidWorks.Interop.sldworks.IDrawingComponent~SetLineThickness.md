<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent~SetLineThickness.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetLineThickness Method (IDrawingComponent) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingComponent Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent.html) : SetLineThickness Method (IDrawingComponent) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*LineFontOption*
:   Line font style of the component as defined in swDrawingComponentLineFontOption\_e

*LineWeights*
:   Line weight style as defined in swLineWeights\_e

*Thickness*
:   Thickness of line; only valid if LineWeights set to swLW\_CUSTOM

Sets the line thickness for the drawing component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetLineThickness( _    ByVal LineFontOption As System.Integer, _    ByVal LineWeights As System.Integer, _    ByVal Thickness As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingComponent Dim LineFontOption As System.Integer Dim LineWeights As System.Integer Dim Thickness As System.Double   instance.SetLineThickness(LineFontOption, LineWeights, Thickness) ``` | |

| C# |  |
| --- | --- |
| ``` void SetLineThickness(     System.int LineFontOption,    System.int LineWeights,    System.double Thickness ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetLineThickness(  &   System.int LineFontOption, &   System.int LineWeights, &   System.double Thickness ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*LineFontOption*
:   Line font style of the component as defined in swDrawingComponentLineFontOption\_e

*LineWeights*
:   Line weight style as defined in swLineWeights\_e

*Thickness*
:   Thickness of line; only valid if LineWeights set to swLW\_CUSTOM

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingComponent::SetLineThickness.

# ![](dotnetimages/collapse.gif)Example

[Get Components in Drawing View (C#)](Get_Components_in_Drawing_View_Example_CSharp.htm)

[Get Components in Drawing View (VB.NET)](Get_Components_in_Drawing_View_Example_VBNET.htm)

[Get Components in Drawing View (VBA)](Get_Components_in_Drawing_View_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingComponent Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent.html)

[IDrawingComponent Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent_members.html)

[IDrawingComponent::GetLineThickness Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent~GetLineThickness.html)

[IDrawingComponent::GetLineStyle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent~GetLineStyle.html)

[IDrawingComponent::SetLineStyle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent~SetLineStyle.html)

[IDrawingComponent::UseDocumentDefaults Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingComponent~UseDocumentDefaults.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~Display.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Display Method (IEdge) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEdge Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html) : Display Method (IEdge) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Width*
:   Highlight width

*Red*
:   Red value of RGB value for the color, between 0 and 1

*Green*
:   Green value of RGB value for the color, between 0 and 1

*Blue*
:   Blue value if RGB value for the color, between 0 and 1

*HighlightState*
:   True if the edge is highlighted, false if not

Highlights this edge with the specified color.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Display( _    ByVal Width As System.Integer, _    ByVal Red As System.Double, _    ByVal Green As System.Double, _    ByVal Blue As System.Double, _    ByVal HighlightState As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEdge Dim Width As System.Integer Dim Red As System.Double Dim Green As System.Double Dim Blue As System.Double Dim HighlightState As System.Boolean   instance.Display(Width, Red, Green, Blue, HighlightState) ``` | |

| C# |  |
| --- | --- |
| ``` void Display(     System.int Width,    System.double Red,    System.double Green,    System.double Blue,    System.bool HighlightState ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Display(  &   System.int Width, &   System.double Red, &   System.double Green, &   System.double Blue, &   System.bool HighlightState ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Width*
:   Highlight width

*Red*
:   Red value of RGB value for the color, between 0 and 1

*Green*
:   Green value of RGB value for the color, between 0 and 1

*Blue*
:   Blue value if RGB value for the color, between 0 and 1

*HighlightState*
:   True if the edge is highlighted, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Edge::Display.

# ![](dotnetimages/collapse.gif)Example

[Add Highlighting to or Remove Highlighting From Edges (VBA)](Add_Highlighting_to_or_Remove_Highlight_from_Edges_Example_VB.htm)

[Get Faces Affected by Feature (VBA)](Get_Faces_Affected_by_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To show the same edge with a different color, hide it and then set a different color. SOLIDWORKS shows the edge in the specified color until you hide it. Rotation, zoom, other repaint actions do not cause the edge to disappear.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdge Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html)

[IEdge Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge_members.html)

[IFace2::IHighlight Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~IHighlight.html)

[IFace2::Highlight Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~Highlight.html)

[IVertex::Display Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVertex~Display.html)

[IEdge::Highlight Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~Highlight.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVertex~Display.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Display Method (IVertex) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IVertex Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVertex.html) : Display Method (IVertex) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TopDoc*
:   [Model](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) in which to display the vertex

*Color*
:   COLORREF value for highlighting

*Scale*
:   Radius of the circle used to display the vertex

    NOTE: Vertex is displayed as a circle. By default, the radius is 4 pixels. Therefore, a scale of 1 is equal to 4 pixels.

*HighlightState*
:   True to highlight the vertex, false to not

Highlights the vertex in the specified color.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Display( _    ByVal TopDoc As ModelDoc2, _    ByVal Color As System.Integer, _    ByVal Scale As System.Double, _    ByVal HighlightState As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IVertex Dim TopDoc As ModelDoc2 Dim Color As System.Integer Dim Scale As System.Double Dim HighlightState As System.Boolean   instance.Display(TopDoc, Color, Scale, HighlightState) ``` | |

| C# |  |
| --- | --- |
| ``` void Display(     ModelDoc2 TopDoc,    System.int Color,    System.double Scale,    System.bool HighlightState ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Display(  &   ModelDoc2^ TopDoc, &   System.int Color, &   System.double Scale, &   System.bool HighlightState ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TopDoc*
:   [Model](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) in which to display the vertex

*Color*
:   COLORREF value for highlighting

*Scale*
:   Radius of the circle used to display the vertex

    NOTE: Vertex is displayed as a circle. By default, the radius is 4 pixels. Therefore, a scale of 1 is equal to 4 pixels.

*HighlightState*
:   True to highlight the vertex, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Vertex::Display.

# ![](dotnetimages/collapse.gif)Example

[Display Vertices (VBA)](Display_Vertices_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **If HighlightState set to...** | **Then the vertex is...** |
| True | Highlighted in the color specified for Color |
| False | Hidden and Color is ignored |

# ![](dotnetimages/collapse.gif)See Also

####

[IVertex Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVertex.html)

[IVertex Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVertex_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0
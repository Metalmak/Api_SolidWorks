<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakLine~GetPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetPosition Method (IBreakLine) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBreakLine Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakLine.html) : GetPosition Method (IBreakLine) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Break line to work with (0 or 1)

Gets the location of this break line in the drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPosition( _    ByVal Index As System.Integer _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBreakLine Dim Index As System.Integer Dim value As System.Double   value = instance.GetPosition(Index) ``` | |

| C# |  |
| --- | --- |
| ``` System.double GetPosition(     System.int Index ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double GetPosition(  &   System.int Index ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Break line to work with (0 or 1)

#### Return Value

Location of the break line (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BreakLine::GetPosition.

# ![](dotnetimages/collapse.gif)Example

[Create Break View (C#)](Create_Broken_View_Example_CSharp.htm)

[Create Break View (VB.NET)](Create_Broken_View_Example_VBNET.htm)

[Create Break View (VBA)](Create_Broken_View_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

A drawing view break consists of a pair of lines. This method gets the break line at the location indicated by the Index argument.

|  |  |
| --- | --- |
| **If the orientation of the break is...** | **Then the return value is...** |
| Horizontal | Y value relative to the drawing view origin (center) that indicates where the break is along the Y axis |
| Vertical | X value relative to the drawing view origin (center) that indicates where the break is along the X axis |

To determine the orientation of the break line, use [IBreakLine::Orientation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBreakLine~Orientation.html) .

# ![](dotnetimages/collapse.gif)See Also

####

[IBreakLine Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakLine.html)

[IBreakLine Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakLine_members.html)

[IBreakline::SetPosition Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakLine~SetPosition.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision NUmber 11.0
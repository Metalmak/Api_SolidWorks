<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlock~GetExtents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetExtents Method (ITitleBlock) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITitleBlock Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlock.html) : GetExtents Method (ITitleBlock) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XUpperLeft*
:   X upper-left coordinate

*YUpperLeft*
:   Y upper-left coordinate

*XLowerRight*
:   X lower-right coordinate

*YLowerRight*
:   Y lower-right coordinate

Gets the coordinates on the drawing sheet format that define the extents of the title block.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetExtents( _    ByRef XUpperLeft As System.Double, _    ByRef YUpperLeft As System.Double, _    ByRef XLowerRight As System.Double, _    ByRef YLowerRight As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITitleBlock Dim XUpperLeft As System.Double Dim YUpperLeft As System.Double Dim XLowerRight As System.Double Dim YLowerRight As System.Double   instance.GetExtents(XUpperLeft, YUpperLeft, XLowerRight, YLowerRight) ``` | |

| C# |  |
| --- | --- |
| ``` void GetExtents(     out System.double XUpperLeft,    out System.double YUpperLeft,    out System.double XLowerRight,    out System.double YLowerRight ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetExtents(  &   [Out] System.double XUpperLeft, &   [Out] System.double YUpperLeft, &   [Out] System.double XLowerRight, &   [Out] System.double YLowerRight ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XUpperLeft*
:   X upper-left coordinate

*YUpperLeft*
:   Y upper-left coordinate

*XLowerRight*
:   X lower-right coordinate

*YLowerRight*
:   Y lower-right coordinate

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TitleBlock::GetExtents.

# ![](dotnetimages/collapse.gif)See Also

####

[ITitleBlock Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlock.html)

[ITitleBlock Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlock_members.html)

[ITitleBlock::SetExtents Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlock~SetExtents.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0
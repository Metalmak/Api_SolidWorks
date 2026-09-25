<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlock~SetExtents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetExtents Method (ITitleBlock) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITitleBlock Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlock.html) : SetExtents Method (ITitleBlock) |

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

Sets the coordinates on the drawing sheet format that define the extens of the title blcok.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetExtents( _    ByVal XUpperLeft As System.Double, _    ByVal YUpperLeft As System.Double, _    ByVal XLowerRight As System.Double, _    ByVal YLowerRight As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITitleBlock Dim XUpperLeft As System.Double Dim YUpperLeft As System.Double Dim XLowerRight As System.Double Dim YLowerRight As System.Double   instance.SetExtents(XUpperLeft, YUpperLeft, XLowerRight, YLowerRight) ``` | |

| C# |  |
| --- | --- |
| ``` void SetExtents(     System.double XUpperLeft,    System.double YUpperLeft,    System.double XLowerRight,    System.double YLowerRight ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetExtents(  &   System.double XUpperLeft, &   System.double YUpperLeft, &   System.double XLowerRight, &   System.double YLowerRight ) ``` | |

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

See TitleBlock::SetExtents.

# ![](dotnetimages/collapse.gif)See Also

####

[ITitleBlock Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlock.html)

[ITitleBlock Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlock_members.html)

[ITitleBlock::GetExtents Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITitleBlock~GetExtents.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0
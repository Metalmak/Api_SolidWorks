<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDiagnoseResult~IGetCoEdgesAtGap.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetCoEdgesAtGap Method (IDiagnoseResult) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDiagnoseResult Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDiagnoseResult.html) : IGetCoEdgesAtGap Method (IDiagnoseResult) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Index number of the gap to get

*CoEdgeCount*
:   Number of coedges at that gap

Gets the coedges at the specified gap.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetCoEdgesAtGap( _    ByVal Index As System.Integer, _    ByVal CoEdgeCount As System.Integer _ ) As CoEdge ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDiagnoseResult Dim Index As System.Integer Dim CoEdgeCount As System.Integer Dim value As CoEdge   value = instance.IGetCoEdgesAtGap(Index, CoEdgeCount) ``` | |

| C# |  |
| --- | --- |
| ``` CoEdge IGetCoEdgesAtGap(     System.int Index,    System.int CoEdgeCount ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CoEdge^ IGetCoEdgesAtGap(  &   System.int Index, &   System.int CoEdgeCount ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Index number of the gap to get

*CoEdgeCount*
:   Number of coedges at that gap

#### Return Value

* in-process, unmanaged C++: Pointer to an array of [ICoEdge](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICoEdge.html) objects

- VBA, VB.NET, C#, and C++/CLI: Not supported

  See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Call:

* [IDiagnoseResult::GetGapsCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDiagnoseResult~GetGapsCount.html) before calling this method to determine the index number of the gap to get on this body.* [IDiagnoseResult::GetCoEdgesCountAtGap](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDiagnoseResult~GetCoEdgesCountAtGap.html) before calling this method to get the number of coedges at the gap on this body.

# ![](dotnetimages/collapse.gif)See Also

####

[IDiagnoseResult Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDiagnoseResult.html)

[IDiagnoseResult Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDiagnoseResult_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP4, Revision Number 12.4
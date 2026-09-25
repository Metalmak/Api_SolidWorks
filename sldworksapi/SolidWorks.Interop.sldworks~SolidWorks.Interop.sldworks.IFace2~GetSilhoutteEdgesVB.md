<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~GetSilhoutteEdgesVB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSilhoutteEdgesVB Method (IFace2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFace2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) : GetSilhoutteEdgesVB Method (IFace2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Xroot*
:   X component of the root point

*Yroot*
:   Y component of the root point

*Zroot*
:   Z component of the root point

*Xnormal*
:   X component of the direction vector

*Ynormal*
:   Y component of the direction vector

*Znormal*
:   Z component of the direction vector

Gets the silhouette edges.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSilhoutteEdgesVB( _    ByVal Xroot As System.Double, _    ByVal Yroot As System.Double, _    ByVal Zroot As System.Double, _    ByVal Xnormal As System.Double, _    ByVal Ynormal As System.Double, _    ByVal Znormal As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFace2 Dim Xroot As System.Double Dim Yroot As System.Double Dim Zroot As System.Double Dim Xnormal As System.Double Dim Ynormal As System.Double Dim Znormal As System.Double Dim value As System.Object   value = instance.GetSilhoutteEdgesVB(Xroot, Yroot, Zroot, Xnormal, Ynormal, Znormal) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetSilhoutteEdgesVB(     System.double Xroot,    System.double Yroot,    System.double Zroot,    System.double Xnormal,    System.double Ynormal,    System.double Znormal ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetSilhoutteEdgesVB(  &   System.double Xroot, &   System.double Yroot, &   System.double Zroot, &   System.double Xnormal, &   System.double Ynormal, &   System.double Znormal ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Xroot*
:   X component of the root point

*Yroot*
:   Y component of the root point

*Zroot*
:   Z component of the root point

*Xnormal*
:   X component of the direction vector

*Ynormal*
:   Y component of the direction vector

*Znormal*
:   Z component of the direction vector

#### Return Value

Array of [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Face2::GetSilhoutteEdgesVB.

# ![](dotnetimages/collapse.gif)Remarks

The return array has two elements for each edge: the first is the silhouette edge and the second is unused. To iterate through the edges, an application needs to step through every second element.

The returned edges are transient and cannot be selected.

# ![](dotnetimages/collapse.gif)See Also

####

[IFace2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)

[IFace2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2_members.html)

[IFace2::IGetSilhoutteEdges Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~IGetSilhoutteEdges.html)

[IFace2::IGetSilhoutteEdgeCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~IGetSilhoutteEdgeCount.html)

[IModelDoc2::InsertSplitLineSil Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertSplitLineSil.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0
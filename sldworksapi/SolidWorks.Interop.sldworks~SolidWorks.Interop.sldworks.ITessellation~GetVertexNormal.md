<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetVertexNormal.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetVertexNormal Method (ITessellation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITessellation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation.html) : GetVertexNormal Method (ITessellation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VertexId*
:   ID of the vertex from which you want to return the normal information

Gets the information that describes the normal direction corresponding to vertex.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetVertexNormal( _    ByVal VertexId As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITessellation Dim VertexId As System.Integer Dim value As System.Object   value = instance.GetVertexNormal(VertexId) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetVertexNormal(     System.int VertexId ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetVertexNormal(  &   System.int VertexId ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*VertexId*
:   ID of the vertex from which you want to return the normal information

#### Return Value

Array of 3 doubles describing the normal vector direction of this vertex corresponding to the face to which it belongs

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Tessellation::GetVertexNormal.

# ![](dotnetimages/collapse.gif)See Also

####

[ITessellation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation.html)

[ITessellation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation_members.html)

[ITessellation::IGetVertexNormal Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetVertexNormal.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0
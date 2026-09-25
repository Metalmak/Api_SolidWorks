<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~GetFacetFins.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetFacetFins Method (ITessellation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITessellation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation.html) : GetFacetFins Method (ITessellation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FacetId*
:   ID of the facet to use to return the fin IDs

Gets all of the fin IDs of the fins that border this facet.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFacetFins( _    ByVal FacetId As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITessellation Dim FacetId As System.Integer Dim value As System.Object   value = instance.GetFacetFins(FacetId) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetFacetFins(     System.int FacetId ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetFacetFins(  &   System.int FacetId ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FacetId*
:   ID of the facet to use to return the fin IDs

#### Return Value

Array of long or integer values that describe the fin IDs

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Tessellation::GetFacetFins.

# ![](dotnetimages/collapse.gif)Example

[Tessellate a Body (C#)](Tessellate_a_Body_Example_CSharp.htm)

[Tessellate a Body (VB.NET)](Tessellate_a_Body_Example_VBNET.htm)

[Tessellate a Body (VBA)](Tessellate_a_Body_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ITessellation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation.html)

[ITessellation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation_members.html)

[ITessellation::IGetFacetFins Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetFacetFins.html)

[ITessellation::IGetFacetFinsCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITessellation~IGetFacetFinsCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0
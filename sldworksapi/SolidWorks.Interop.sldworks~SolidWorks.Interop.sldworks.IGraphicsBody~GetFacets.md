<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGraphicsBody~GetFacets.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetFacets Method (IGraphicsBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IGraphicsBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGraphicsBody.html) : GetFacets Method (IGraphicsBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the facets on this graphics body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFacets() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGraphicsBody Dim value As System.Object   value = instance.GetFacets() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetFacets() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetFacets(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of [IFacet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet.html)s

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See GraphicsBody::GetFacets.

# ![](dotnetimages/collapse.gif)Example

See the [IFacet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IGraphicsBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGraphicsBody.html)

[IGraphicsBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGraphicsBody_members.html)

[IGraphicsBody::GetFacetCount Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGraphicsBody~GetFacetCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30
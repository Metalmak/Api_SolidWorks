<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISymmetricMateFeatureData~EntitiesToMate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EntitiesToMate Property (ISymmetricMateFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISymmetricMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISymmetricMateFeatureData.html) : EntitiesToMate Property (ISymmetricMateFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the entities in this symmetry mate.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property EntitiesToMate As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISymmetricMateFeatureData Dim value As System.Object   instance.EntitiesToMate = value   value = instance.EntitiesToMate ``` | |

| C# |  |
| --- | --- |
| ``` System.object EntitiesToMate {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ EntitiesToMate {    System.Object^ get();    void set ( &   System.Object^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Array of two similar entities: [vertexes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVertex.html), [sketch points](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html), [edges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html), [axes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html), [sketch lines](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchLine.html), [planes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html), [planar faces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html), spheres of equal radii, or cylinders of equal radii

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See [SymmetricMateFeatureData::EntitiesToMate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISymmetricMateFeatureData~EntitiesToMate.html).

# ![](dotnetimages/collapse.gif)Example

See the [ISymmetricMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISymmetricMateFeatureData.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ISymmetricMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISymmetricMateFeatureData.html)

[ISymmetricMateFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISymmetricMateFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0
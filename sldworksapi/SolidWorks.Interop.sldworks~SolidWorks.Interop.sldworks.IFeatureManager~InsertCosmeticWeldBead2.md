<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertCosmeticWeldBead2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertCosmeticWeldBead2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertCosmeticWeldBead2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WeldMode*
:   Weld mode as defined inswCosmeticWeldBeadMode\_e

*WeldFromFaceOrEdgeSet*
:   Array of weld-from entities (see **Remarks**)

*WeldToFaceOrEdgeSet*
:   Array of weld-to entities or Nothing or null (see **Remarks**)

*WeldSize*
:   Size of weld bead

Inserts a cosmetic weld bead using either weld geometry or a weld path.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertCosmeticWeldBead2( _    ByVal WeldMode As System.Integer, _    ByVal WeldFromFaceOrEdgeSet As System.Object, _    ByVal WeldToFaceOrEdgeSet As System.Object, _    ByVal WeldSize As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim WeldMode As System.Integer Dim WeldFromFaceOrEdgeSet As System.Object Dim WeldToFaceOrEdgeSet As System.Object Dim WeldSize As System.Double Dim value As System.Object   value = instance.InsertCosmeticWeldBead2(WeldMode, WeldFromFaceOrEdgeSet, WeldToFaceOrEdgeSet, WeldSize) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertCosmeticWeldBead2(     System.int WeldMode,    System.object WeldFromFaceOrEdgeSet,    System.object WeldToFaceOrEdgeSet,    System.double WeldSize ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertCosmeticWeldBead2(  &   System.int WeldMode, &   System.Object^ WeldFromFaceOrEdgeSet, &   System.Object^ WeldToFaceOrEdgeSet, &   System.double WeldSize ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WeldMode*
:   Weld mode as defined inswCosmeticWeldBeadMode\_e

*WeldFromFaceOrEdgeSet*
:   Array of weld-from entities (see **Remarks**)

*WeldToFaceOrEdgeSet*
:   Array of weld-to entities or Nothing or null (see **Remarks**)

*WeldSize*
:   Size of weld bead

#### Return Value

Array of weld bead [features](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertCosmeticWeldBead2.

# ![](dotnetimages/collapse.gif)Example

[Insert Cosmetic Weld Bead Using Geometric Entities (C#)](Insert_Cosmetic_Weld_Bead_Using_Geometric_Entities_Example_CSharp.htm)

[Insert Cosmetic Weld Bead Using Geometric Entities (VB.NET)](Insert_Cosmetic_Weld_Bead_Using_Geometric_Entities_Example_VBNET.htm)

[Insert Cosmetic Weld Bead Using Geometric Entities (VBA)](Insert_Cosmetic_Weld_Bead_Using_Geometric_Entities_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |  |
| --- | --- | --- |
| **WeldMode** | **Selected entities** | **Selection marks** |
| swCosmeticWeldBeadMode\_e.swCosmeticWeldBeadMode\_WeldGeometry | Either [faces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) or [edges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html) as weld-from and weld-to entities  **NOTE**: Both weld-to and weld-from entities must all be the same type of entities; e.g., all faces or all edges. | * 4 for each weld-from entity in WeldFromFaceOrEdgeSet  * 8 for each weld-to entity in WeldToFaceOrEdgeSet |
| swCosmeticWeldBeadMode\_e.swCosmeticWeldBeadMode\_WeldPath | Edges, [sketches](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html), or a combination of edges and sketches are selected as weld-from entities | * 0 for each weld-from entity in WeldFromFaceOrEdgeSet* Nothing or null for WeldToFaceOrEdgeSet |

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData~GetFaces.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetFaces Method (ISMCornerReliefData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISMCornerReliefData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData.html) : GetFaces Method (ISMCornerReliefData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Face1*
:   First [IFace2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) that defines this two- or three-bend corner

*Face2*
:   Second IFace2 that defines this two- or three-bend corner

*Face3*
:   Third IFace2 that defines this three-bend corner; valid only if ICornerReliefFeatureData::CornerReliefBendType is swCornerReliefBendType\_e.swCornerReliefBendType\_ThreeBend; specify null or Nothing for a two-bend corner

Gets the faces used to create this sheet metal corner.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetFaces( _    ByRef Face1 As System.Object, _    ByRef Face2 As System.Object, _    ByRef Face3 As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISMCornerReliefData Dim Face1 As System.Object Dim Face2 As System.Object Dim Face3 As System.Object   instance.GetFaces(Face1, Face2, Face3) ``` | |

| C# |  |
| --- | --- |
| ``` void GetFaces(     out System.object Face1,    out System.object Face2,    out System.object Face3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetFaces(  &   [Out] System.Object^ Face1, &   [Out] System.Object^ Face2, &   [Out] System.Object^ Face3 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Face1*
:   First [IFace2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) that defines this two- or three-bend corner

*Face2*
:   Second IFace2 that defines this two- or three-bend corner

*Face3*
:   Third IFace2 that defines this three-bend corner; valid only if ICornerReliefFeatureData::CornerReliefBendType is swCornerReliefBendType\_e.swCornerReliefBendType\_ThreeBend; specify null or Nothing for a two-bend corner

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SMCornerReliefData::GetFaces.

# ![](dotnetimages/collapse.gif)Example

See the [ICornerReliefFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ISMCornerReliefData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData.html)

[ISMCornerReliefData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30
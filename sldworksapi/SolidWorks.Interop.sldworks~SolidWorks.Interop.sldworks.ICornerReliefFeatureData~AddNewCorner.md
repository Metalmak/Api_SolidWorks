<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~AddNewCorner.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddNewCorner Method (ICornerReliefFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICornerReliefFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData.html) : AddNewCorner Method (ICornerReliefFeatureData) |

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

*ReliefType*
:   Corner relief type as defined by swCornerReliefType\_e

*Corner*
:   [ISMCornerReliefData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData.html)

Adds a corner with the specified parameters to this sheet metal corner relief feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddNewCorner( _    ByVal Face1 As System.Object, _    ByVal Face2 As System.Object, _    ByVal Face3 As System.Object, _    ByVal ReliefType As System.Integer, _    ByRef Corner As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICornerReliefFeatureData Dim Face1 As System.Object Dim Face2 As System.Object Dim Face3 As System.Object Dim ReliefType As System.Integer Dim Corner As System.Object Dim value As System.Integer   value = instance.AddNewCorner(Face1, Face2, Face3, ReliefType, Corner) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddNewCorner(     System.object Face1,    System.object Face2,    System.object Face3,    System.int ReliefType,    out System.object Corner ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddNewCorner(  &   System.Object^ Face1, &   System.Object^ Face2, &   System.Object^ Face3, &   System.int ReliefType, &   [Out] System.Object^ Corner ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Face1*
:   First [IFace2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) that defines this two- or three-bend corner

*Face2*
:   Second IFace2 that defines this two- or three-bend corner

*Face3*
:   Third IFace2 that defines this three-bend corner; valid only if ICornerReliefFeatureData::CornerReliefBendType is swCornerReliefBendType\_e.swCornerReliefBendType\_ThreeBend; specify null or Nothing for a two-bend corner

*ReliefType*
:   Corner relief type as defined by swCornerReliefType\_e

*Corner*
:   [ISMCornerReliefData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData.html)

#### Return Value

Error code as defined by swCornerReliefError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CornerReliefFeatureData::AddNewCorner.

# ![](dotnetimages/collapse.gif)See Also

####

[ICornerReliefFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData.html)

[ICornerReliefFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30
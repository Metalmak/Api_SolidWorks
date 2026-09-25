<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~CollectAllCorners.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CollectAllCorners Method (ICornerReliefFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICornerReliefFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData.html) : CollectAllCorners Method (ICornerReliefFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ReliefType*
:   Corner relief type as defined by swCornerReliefType\_e

*Corners*
:   Array of [ISMCornerReliefData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData.html)s

Creates corners, all with the specified relief, in a selected sheet-metal body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CollectAllCorners( _    ByVal ReliefType As System.Integer, _    ByRef Corners As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICornerReliefFeatureData Dim ReliefType As System.Integer Dim Corners As System.Object Dim value As System.Integer   value = instance.CollectAllCorners(ReliefType, Corners) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CollectAllCorners(     System.int ReliefType,    out System.object Corners ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CollectAllCorners(  &   System.int ReliefType, &   [Out] System.Object^ Corners ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ReliefType*
:   Corner relief type as defined by swCornerReliefType\_e

*Corners*
:   Array of [ISMCornerReliefData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMCornerReliefData.html)s

#### Return Value

Error code as defined by swCornerReliefError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CornerReliefFeatureData::CollectAllCorners.

# ![](dotnetimages/collapse.gif)Example

See the [ICornerReliefFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ICornerReliefFeatureData::SetBodyScope](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~SetBodyScope.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICornerReliefFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData.html)

[ICornerReliefFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30
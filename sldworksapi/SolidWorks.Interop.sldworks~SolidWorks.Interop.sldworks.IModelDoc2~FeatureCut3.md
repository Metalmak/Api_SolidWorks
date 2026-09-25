<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~FeatureCut3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureCut3 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : FeatureCut3 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Sd*

*Flip*

*Dir*

*T1*

*T2*

*D1*

*D2*

*Dchk1*

*Dchk2*

*Ddir1*

*Ddir2*

*Dang1*

*Dang2*

*OffsetReverse1*

*OffsetReverse2*

*KeepPieceIndex*

Obsolete. Superseded by [IFeatureManager::FeatureCut](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~FeatureCut.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub FeatureCut3( _    ByVal Sd As System.Boolean, _    ByVal Flip As System.Boolean, _    ByVal Dir As System.Boolean, _    ByVal T1 As System.Integer, _    ByVal T2 As System.Integer, _    ByVal D1 As System.Double, _    ByVal D2 As System.Double, _    ByVal Dchk1 As System.Boolean, _    ByVal Dchk2 As System.Boolean, _    ByVal Ddir1 As System.Boolean, _    ByVal Ddir2 As System.Boolean, _    ByVal Dang1 As System.Double, _    ByVal Dang2 As System.Double, _    ByVal OffsetReverse1 As System.Boolean, _    ByVal OffsetReverse2 As System.Boolean, _    ByVal KeepPieceIndex As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Sd As System.Boolean Dim Flip As System.Boolean Dim Dir As System.Boolean Dim T1 As System.Integer Dim T2 As System.Integer Dim D1 As System.Double Dim D2 As System.Double Dim Dchk1 As System.Boolean Dim Dchk2 As System.Boolean Dim Ddir1 As System.Boolean Dim Ddir2 As System.Boolean Dim Dang1 As System.Double Dim Dang2 As System.Double Dim OffsetReverse1 As System.Boolean Dim OffsetReverse2 As System.Boolean Dim KeepPieceIndex As System.Integer   instance.FeatureCut3(Sd, Flip, Dir, T1, T2, D1, D2, Dchk1, Dchk2, Ddir1, Ddir2, Dang1, Dang2, OffsetReverse1, OffsetReverse2, KeepPieceIndex) ``` | |

| C# |  |
| --- | --- |
| ``` void FeatureCut3(     System.bool Sd,    System.bool Flip,    System.bool Dir,    System.int T1,    System.int T2,    System.double D1,    System.double D2,    System.bool Dchk1,    System.bool Dchk2,    System.bool Ddir1,    System.bool Ddir2,    System.double Dang1,    System.double Dang2,    System.bool OffsetReverse1,    System.bool OffsetReverse2,    System.int KeepPieceIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void FeatureCut3(  &   System.bool Sd, &   System.bool Flip, &   System.bool Dir, &   System.int T1, &   System.int T2, &   System.double D1, &   System.double D2, &   System.bool Dchk1, &   System.bool Dchk2, &   System.bool Ddir1, &   System.bool Ddir2, &   System.double Dang1, &   System.double Dang2, &   System.bool OffsetReverse1, &   System.bool OffsetReverse2, &   System.int KeepPieceIndex ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Sd*

*Flip*

*Dir*

*T1*

*T2*

*D1*

*D2*

*Dchk1*

*Dchk2*

*Ddir1*

*Ddir2*

*Dang1*

*Dang2*

*OffsetReverse1*

*OffsetReverse2*

*KeepPieceIndex*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::FeatureCut3.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)
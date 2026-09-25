<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureExtrusion.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureExtrusion Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : FeatureExtrusion Method (IFeatureManager) |

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

*TranslateSurface1*

*TranslateSurface2*

*Merge*

*UseFeatScope*

*UseAutoSelect*

Obsolete. Superseded by [IFeatureManager::FeatureExtrusion2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~FeatureExtrusion2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureExtrusion( _    ByVal Sd As System.Boolean, _    ByVal Flip As System.Boolean, _    ByVal Dir As System.Boolean, _    ByVal T1 As System.Integer, _    ByVal T2 As System.Integer, _    ByVal D1 As System.Double, _    ByVal D2 As System.Double, _    ByVal Dchk1 As System.Boolean, _    ByVal Dchk2 As System.Boolean, _    ByVal Ddir1 As System.Boolean, _    ByVal Ddir2 As System.Boolean, _    ByVal Dang1 As System.Double, _    ByVal Dang2 As System.Double, _    ByVal OffsetReverse1 As System.Boolean, _    ByVal OffsetReverse2 As System.Boolean, _    ByVal TranslateSurface1 As System.Boolean, _    ByVal TranslateSurface2 As System.Boolean, _    ByVal Merge As System.Boolean, _    ByVal UseFeatScope As System.Boolean, _    ByVal UseAutoSelect As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Sd As System.Boolean Dim Flip As System.Boolean Dim Dir As System.Boolean Dim T1 As System.Integer Dim T2 As System.Integer Dim D1 As System.Double Dim D2 As System.Double Dim Dchk1 As System.Boolean Dim Dchk2 As System.Boolean Dim Ddir1 As System.Boolean Dim Ddir2 As System.Boolean Dim Dang1 As System.Double Dim Dang2 As System.Double Dim OffsetReverse1 As System.Boolean Dim OffsetReverse2 As System.Boolean Dim TranslateSurface1 As System.Boolean Dim TranslateSurface2 As System.Boolean Dim Merge As System.Boolean Dim UseFeatScope As System.Boolean Dim UseAutoSelect As System.Boolean Dim value As Feature   value = instance.FeatureExtrusion(Sd, Flip, Dir, T1, T2, D1, D2, Dchk1, Dchk2, Ddir1, Ddir2, Dang1, Dang2, OffsetReverse1, OffsetReverse2, TranslateSurface1, TranslateSurface2, Merge, UseFeatScope, UseAutoSelect) ``` | |

| C# |  |
| --- | --- |
| ``` Feature FeatureExtrusion(     System.bool Sd,    System.bool Flip,    System.bool Dir,    System.int T1,    System.int T2,    System.double D1,    System.double D2,    System.bool Dchk1,    System.bool Dchk2,    System.bool Ddir1,    System.bool Ddir2,    System.double Dang1,    System.double Dang2,    System.bool OffsetReverse1,    System.bool OffsetReverse2,    System.bool TranslateSurface1,    System.bool TranslateSurface2,    System.bool Merge,    System.bool UseFeatScope,    System.bool UseAutoSelect ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ FeatureExtrusion(  &   System.bool Sd, &   System.bool Flip, &   System.bool Dir, &   System.int T1, &   System.int T2, &   System.double D1, &   System.double D2, &   System.bool Dchk1, &   System.bool Dchk2, &   System.bool Ddir1, &   System.bool Ddir2, &   System.double Dang1, &   System.double Dang2, &   System.bool OffsetReverse1, &   System.bool OffsetReverse2, &   System.bool TranslateSurface1, &   System.bool TranslateSurface2, &   System.bool Merge, &   System.bool UseFeatScope, &   System.bool UseAutoSelect ) ``` | |

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

*TranslateSurface1*

*TranslateSurface2*

*Merge*

*UseFeatScope*

*UseAutoSelect*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::FeatureExtrusion.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)
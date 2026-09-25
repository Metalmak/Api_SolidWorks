<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertCutBlend4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertCutBlend4 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertCutBlend4 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Closed*

*KeepTangency*

*ForceNonRational*

*TessToleranceFactor*

*StartMatchingType*

*EndMatchingType*

*IsThinBody*

*Thickness1*

*Thickness2*

*ThinType*

Obsolete. Superseded by [IFeatureManager::InsertCutBlend](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertCutBlend.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertCutBlend4( _    ByVal Closed As System.Boolean, _    ByVal KeepTangency As System.Boolean, _    ByVal ForceNonRational As System.Boolean, _    ByVal TessToleranceFactor As System.Double, _    ByVal StartMatchingType As System.Short, _    ByVal EndMatchingType As System.Short, _    ByVal IsThinBody As System.Boolean, _    ByVal Thickness1 As System.Double, _    ByVal Thickness2 As System.Double, _    ByVal ThinType As System.Short _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Closed As System.Boolean Dim KeepTangency As System.Boolean Dim ForceNonRational As System.Boolean Dim TessToleranceFactor As System.Double Dim StartMatchingType As System.Short Dim EndMatchingType As System.Short Dim IsThinBody As System.Boolean Dim Thickness1 As System.Double Dim Thickness2 As System.Double Dim ThinType As System.Short   instance.InsertCutBlend4(Closed, KeepTangency, ForceNonRational, TessToleranceFactor, StartMatchingType, EndMatchingType, IsThinBody, Thickness1, Thickness2, ThinType) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertCutBlend4(     System.bool Closed,    System.bool KeepTangency,    System.bool ForceNonRational,    System.double TessToleranceFactor,    System.short StartMatchingType,    System.short EndMatchingType,    System.bool IsThinBody,    System.double Thickness1,    System.double Thickness2,    System.short ThinType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertCutBlend4(  &   System.bool Closed, &   System.bool KeepTangency, &   System.bool ForceNonRational, &   System.double TessToleranceFactor, &   System.short StartMatchingType, &   System.short EndMatchingType, &   System.bool IsThinBody, &   System.double Thickness1, &   System.double Thickness2, &   System.short ThinType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Closed*

*KeepTangency*

*ForceNonRational*

*TessToleranceFactor*

*StartMatchingType*

*EndMatchingType*

*IsThinBody*

*Thickness1*

*Thickness2*

*ThinType*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertCutBlend4.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)
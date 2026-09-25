<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertProtrusionSwept.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertProtrusionSwept Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertProtrusionSwept Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Propagate*

*Alignment*

*TwistCtrlOption*

*KeepTangency*

*ForceNonRational*

*StartMatchingType*

*EndMatchingType*

*IsThinBody*

*Thickness1*

*Thickness2*

*ThinType*

*Merge*

*UseFeatScope*

*UseAutoSelect*

Obsolete. Superseded by [IFeatureManager::InsertProtusionSwept3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertProtrusionSwept3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertProtrusionSwept( _    ByVal Propagate As System.Boolean, _    ByVal Alignment As System.Boolean, _    ByVal TwistCtrlOption As System.Short, _    ByVal KeepTangency As System.Boolean, _    ByVal ForceNonRational As System.Boolean, _    ByVal StartMatchingType As System.Short, _    ByVal EndMatchingType As System.Short, _    ByVal IsThinBody As System.Boolean, _    ByVal Thickness1 As System.Double, _    ByVal Thickness2 As System.Double, _    ByVal ThinType As System.Short, _    ByVal Merge As System.Boolean, _    ByVal UseFeatScope As System.Boolean, _    ByVal UseAutoSelect As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Propagate As System.Boolean Dim Alignment As System.Boolean Dim TwistCtrlOption As System.Short Dim KeepTangency As System.Boolean Dim ForceNonRational As System.Boolean Dim StartMatchingType As System.Short Dim EndMatchingType As System.Short Dim IsThinBody As System.Boolean Dim Thickness1 As System.Double Dim Thickness2 As System.Double Dim ThinType As System.Short Dim Merge As System.Boolean Dim UseFeatScope As System.Boolean Dim UseAutoSelect As System.Boolean Dim value As Feature   value = instance.InsertProtrusionSwept(Propagate, Alignment, TwistCtrlOption, KeepTangency, ForceNonRational, StartMatchingType, EndMatchingType, IsThinBody, Thickness1, Thickness2, ThinType, Merge, UseFeatScope, UseAutoSelect) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertProtrusionSwept(     System.bool Propagate,    System.bool Alignment,    System.short TwistCtrlOption,    System.bool KeepTangency,    System.bool ForceNonRational,    System.short StartMatchingType,    System.short EndMatchingType,    System.bool IsThinBody,    System.double Thickness1,    System.double Thickness2,    System.short ThinType,    System.bool Merge,    System.bool UseFeatScope,    System.bool UseAutoSelect ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertProtrusionSwept(  &   System.bool Propagate, &   System.bool Alignment, &   System.short TwistCtrlOption, &   System.bool KeepTangency, &   System.bool ForceNonRational, &   System.short StartMatchingType, &   System.short EndMatchingType, &   System.bool IsThinBody, &   System.double Thickness1, &   System.double Thickness2, &   System.short ThinType, &   System.bool Merge, &   System.bool UseFeatScope, &   System.bool UseAutoSelect ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Propagate*

*Alignment*

*TwistCtrlOption*

*KeepTangency*

*ForceNonRational*

*StartMatchingType*

*EndMatchingType*

*IsThinBody*

*Thickness1*

*Thickness2*

*ThinType*

*Merge*

*UseFeatScope*

*UseAutoSelect*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertProtrusionSwept.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)
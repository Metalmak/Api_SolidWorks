<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~InsertProtrusionSwept4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertProtrusionSwept4 Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : InsertProtrusionSwept4 Method (IModelDoc) |

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

Obsolete. Superseded by [IModelDoc2::InsertProtrusionSwept4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~InsertProtrusionSwept4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertProtrusionSwept4( _    ByVal Propagate As System.Boolean, _    ByVal Alignment As System.Boolean, _    ByVal TwistCtrlOption As System.Short, _    ByVal KeepTangency As System.Boolean, _    ByVal ForceNonRational As System.Boolean, _    ByVal StartMatchingType As System.Short, _    ByVal EndMatchingType As System.Short, _    ByVal IsThinBody As System.Boolean, _    ByVal Thickness1 As System.Double, _    ByVal Thickness2 As System.Double, _    ByVal ThinType As System.Short _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim Propagate As System.Boolean Dim Alignment As System.Boolean Dim TwistCtrlOption As System.Short Dim KeepTangency As System.Boolean Dim ForceNonRational As System.Boolean Dim StartMatchingType As System.Short Dim EndMatchingType As System.Short Dim IsThinBody As System.Boolean Dim Thickness1 As System.Double Dim Thickness2 As System.Double Dim ThinType As System.Short   instance.InsertProtrusionSwept4(Propagate, Alignment, TwistCtrlOption, KeepTangency, ForceNonRational, StartMatchingType, EndMatchingType, IsThinBody, Thickness1, Thickness2, ThinType) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertProtrusionSwept4(     System.bool Propagate,    System.bool Alignment,    System.short TwistCtrlOption,    System.bool KeepTangency,    System.bool ForceNonRational,    System.short StartMatchingType,    System.short EndMatchingType,    System.bool IsThinBody,    System.double Thickness1,    System.double Thickness2,    System.short ThinType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertProtrusionSwept4(  &   System.bool Propagate, &   System.bool Alignment, &   System.short TwistCtrlOption, &   System.bool KeepTangency, &   System.bool ForceNonRational, &   System.short StartMatchingType, &   System.short EndMatchingType, &   System.bool IsThinBody, &   System.double Thickness1, &   System.double Thickness2, &   System.short ThinType ) ``` | |

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

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::InsertProtrusionSwept4.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)
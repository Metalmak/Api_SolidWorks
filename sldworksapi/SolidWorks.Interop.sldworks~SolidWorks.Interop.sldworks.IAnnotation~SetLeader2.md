<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~SetLeader2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetLeader2 Method (IAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html) : SetLeader2 Method (IAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Leader*

*LeaderSide*

*SmartArrowHeadStyle*

*BentLeader*

*Perpendicular*

*AllAround*

Obsolete. Superseded by [IAnnotation::SetLeader3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~SetLeader3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetLeader2( _    ByVal Leader As System.Boolean, _    ByVal LeaderSide As System.Integer, _    ByVal SmartArrowHeadStyle As System.Boolean, _    ByVal BentLeader As System.Boolean, _    ByVal Perpendicular As System.Boolean, _    ByVal AllAround As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAnnotation Dim Leader As System.Boolean Dim LeaderSide As System.Integer Dim SmartArrowHeadStyle As System.Boolean Dim BentLeader As System.Boolean Dim Perpendicular As System.Boolean Dim AllAround As System.Boolean Dim value As System.Integer   value = instance.SetLeader2(Leader, LeaderSide, SmartArrowHeadStyle, BentLeader, Perpendicular, AllAround) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetLeader2(     System.bool Leader,    System.int LeaderSide,    System.bool SmartArrowHeadStyle,    System.bool BentLeader,    System.bool Perpendicular,    System.bool AllAround ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetLeader2(  &   System.bool Leader, &   System.int LeaderSide, &   System.bool SmartArrowHeadStyle, &   System.bool BentLeader, &   System.bool Perpendicular, &   System.bool AllAround ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Leader*

*LeaderSide*

*SmartArrowHeadStyle*

*BentLeader*

*Perpendicular*

*AllAround*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Annotation::SetLeader2.

# ![](dotnetimages/collapse.gif)See Also

####

[IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html)

[IAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation_members.html)
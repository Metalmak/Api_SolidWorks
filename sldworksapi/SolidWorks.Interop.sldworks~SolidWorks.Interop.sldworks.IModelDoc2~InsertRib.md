<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertRib.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertRib Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertRib Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Is2Sided*

*ReverseThicknessDir*

*Thickness*

*ReferenceEdgeIndex*

*ReverseMaterialDir*

*IsDrafted*

*DraftOutward*

*DraftAngle*

Obsolete. Superseded by [IModelDoc2::InsertRib2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~InsertRib2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertRib( _    ByVal Is2Sided As System.Boolean, _    ByVal ReverseThicknessDir As System.Boolean, _    ByVal Thickness As System.Double, _    ByVal ReferenceEdgeIndex As System.Integer, _    ByVal ReverseMaterialDir As System.Boolean, _    ByVal IsDrafted As System.Boolean, _    ByVal DraftOutward As System.Boolean, _    ByVal DraftAngle As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Is2Sided As System.Boolean Dim ReverseThicknessDir As System.Boolean Dim Thickness As System.Double Dim ReferenceEdgeIndex As System.Integer Dim ReverseMaterialDir As System.Boolean Dim IsDrafted As System.Boolean Dim DraftOutward As System.Boolean Dim DraftAngle As System.Double   instance.InsertRib(Is2Sided, ReverseThicknessDir, Thickness, ReferenceEdgeIndex, ReverseMaterialDir, IsDrafted, DraftOutward, DraftAngle) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertRib(     System.bool Is2Sided,    System.bool ReverseThicknessDir,    System.double Thickness,    System.int ReferenceEdgeIndex,    System.bool ReverseMaterialDir,    System.bool IsDrafted,    System.bool DraftOutward,    System.double DraftAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertRib(  &   System.bool Is2Sided, &   System.bool ReverseThicknessDir, &   System.double Thickness, &   System.int ReferenceEdgeIndex, &   System.bool ReverseMaterialDir, &   System.bool IsDrafted, &   System.bool DraftOutward, &   System.double DraftAngle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Is2Sided*

*ReverseThicknessDir*

*Thickness*

*ReferenceEdgeIndex*

*ReverseMaterialDir*

*IsDrafted*

*DraftOutward*

*DraftAngle*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertRib.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)
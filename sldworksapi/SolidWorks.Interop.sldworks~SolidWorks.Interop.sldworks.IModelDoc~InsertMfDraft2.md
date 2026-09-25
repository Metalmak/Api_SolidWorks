<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~InsertMfDraft2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertMfDraft2 Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : InsertMfDraft2 Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Angle*

*FlipDir*

*IsEdgeDraft*

*PropType*

*StepDraft*

Obsolete. Superseded by [IModelDoc2::InsertMfDraft2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~InsertMfDraft2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertMfDraft2( _    ByVal Angle As System.Double, _    ByVal FlipDir As System.Boolean, _    ByVal IsEdgeDraft As System.Boolean, _    ByVal PropType As System.Integer, _    ByVal StepDraft As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim Angle As System.Double Dim FlipDir As System.Boolean Dim IsEdgeDraft As System.Boolean Dim PropType As System.Integer Dim StepDraft As System.Boolean   instance.InsertMfDraft2(Angle, FlipDir, IsEdgeDraft, PropType, StepDraft) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertMfDraft2(     System.double Angle,    System.bool FlipDir,    System.bool IsEdgeDraft,    System.int PropType,    System.bool StepDraft ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertMfDraft2(  &   System.double Angle, &   System.bool FlipDir, &   System.bool IsEdgeDraft, &   System.int PropType, &   System.bool StepDraft ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Angle*

*FlipDir*

*IsEdgeDraft*

*PropType*

*StepDraft*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::InsertMfDraft2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)
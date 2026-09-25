<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DraftBody.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DraftBody Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : DraftBody Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumOfFaces*

*FaceList*

*EdgeList*

*DraftAngle*

*Dir*

Obsolete. Superseded by [IBody2::DraftBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~DraftBody2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DraftBody( _    ByVal NumOfFaces As System.Integer, _    ByVal FaceList As System.Object, _    ByVal EdgeList As System.Object, _    ByVal DraftAngle As System.Double, _    ByVal Dir As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim NumOfFaces As System.Integer Dim FaceList As System.Object Dim EdgeList As System.Object Dim DraftAngle As System.Double Dim Dir As System.Object Dim value As System.Boolean   value = instance.DraftBody(NumOfFaces, FaceList, EdgeList, DraftAngle, Dir) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool DraftBody(     System.int NumOfFaces,    System.object FaceList,    System.object EdgeList,    System.double DraftAngle,    System.object Dir ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool DraftBody(  &   System.int NumOfFaces, &   System.Object^ FaceList, &   System.Object^ EdgeList, &   System.double DraftAngle, &   System.Object^ Dir ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumOfFaces*

*FaceList*

*EdgeList*

*DraftAngle*

*Dir*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::DraftBody.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)
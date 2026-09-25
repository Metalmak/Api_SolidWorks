<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~IDraftBody.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IDraftBody Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : IDraftBody Method (IBody) |

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

Obsolete. Superseded by [IBody2::IDraftBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IDraftBody2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IDraftBody( _    ByVal NumOfFaces As System.Integer, _    ByRef FaceList As Face, _    ByRef EdgeList As Edge, _    ByVal DraftAngle As System.Double, _    ByRef Dir As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim NumOfFaces As System.Integer Dim FaceList As Face Dim EdgeList As Edge Dim DraftAngle As System.Double Dim Dir As System.Double Dim value As System.Boolean   value = instance.IDraftBody(NumOfFaces, FaceList, EdgeList, DraftAngle, Dir) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IDraftBody(     System.int NumOfFaces,    ref Face FaceList,    ref Edge EdgeList,    System.double DraftAngle,    ref System.double Dir ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IDraftBody(  &   System.int NumOfFaces, &   Face^% FaceList, &   Edge^% EdgeList, &   System.double DraftAngle, &   System.double% Dir ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumOfFaces*

*FaceList*

*EdgeList*

*DraftAngle*

*Dir*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::IDraftBody.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)
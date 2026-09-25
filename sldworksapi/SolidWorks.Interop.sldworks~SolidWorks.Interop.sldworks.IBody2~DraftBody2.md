<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DraftBody2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DraftBody2 Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : DraftBody2 Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumOfFaces*
:   Number of faces to draft

*FaceList*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) to draft

*EdgeList*
:   Array of [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html), one for each face, along which to apply the drafts

*BasePoint*
:   Pointer to a [MathPoint](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) object (x,y,z values of the base point)

*DraftAngle*
:   Draft angle

*Dir*
:   Array of 3 doubles (x, y, z), a vector which specifies the direction of the draft

Adds drafts to the specified faces on a temporary body. This method modifies the body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DraftBody2( _    ByVal NumOfFaces As System.Integer, _    ByVal FaceList As System.Object, _    ByVal EdgeList As System.Object, _    ByVal BasePoint As System.Object, _    ByVal DraftAngle As System.Double, _    ByVal Dir As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim NumOfFaces As System.Integer Dim FaceList As System.Object Dim EdgeList As System.Object Dim BasePoint As System.Object Dim DraftAngle As System.Double Dim Dir As System.Object Dim value As System.Boolean   value = instance.DraftBody2(NumOfFaces, FaceList, EdgeList, BasePoint, DraftAngle, Dir) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool DraftBody2(     System.int NumOfFaces,    System.object FaceList,    System.object EdgeList,    System.object BasePoint,    System.double DraftAngle,    System.object Dir ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool DraftBody2(  &   System.int NumOfFaces, &   System.Object^ FaceList, &   System.Object^ EdgeList, &   System.Object^ BasePoint, &   System.double DraftAngle, &   System.Object^ Dir ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumOfFaces*
:   Number of faces to draft

*FaceList*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) to draft

*EdgeList*
:   Array of [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html), one for each face, along which to apply the drafts

*BasePoint*
:   Pointer to a [MathPoint](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) object (x,y,z values of the base point)

*DraftAngle*
:   Draft angle

*Dir*
:   Array of 3 doubles (x, y, z), a vector which specifies the direction of the draft

#### Return Value

True if drafts are applied, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::DraftBody2.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::IDraftBody2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDraftBody2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteFaces3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DeleteFaces3 Method (IBody2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : DeleteFaces3 Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FaceList*
:   Array containing the [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) for deletion

*Option*
:   Additional control (see **Remarks**)

*DoLocalCheck*
:   True checks the bodies during the operation and sets the return value to indicate whether or not the resultant body is valid, false does not

*LocalCheckResult*
:   True if body is valid, false if not; to obtain this value, you must pass True for the DoLocalCheck argument

Obsolete. Superseded by [IBody2::IDeleteFaces4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~DeleteFaces4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DeleteFaces3( _    ByVal FaceList As System.Object, _    ByVal Option As System.Integer, _    ByVal DoLocalCheck As System.Boolean, _    ByRef LocalCheckResult As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim FaceList As System.Object Dim Option As System.Integer Dim DoLocalCheck As System.Boolean Dim LocalCheckResult As System.Boolean Dim value As System.Boolean   value = instance.DeleteFaces3(FaceList, Option, DoLocalCheck, LocalCheckResult) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool DeleteFaces3(     System.object FaceList,    System.int Option,    System.bool DoLocalCheck,    out System.bool LocalCheckResult ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool DeleteFaces3(  &   System.Object^ FaceList, &   System.int Option, &   System.bool DoLocalCheck, &   [Out] System.bool LocalCheckResult ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FaceList*
:   Array containing the [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) for deletion

*Option*
:   Additional control (see **Remarks**)

*DoLocalCheck*
:   True checks the bodies during the operation and sets the return value to indicate whether or not the resultant body is valid, false does not

*LocalCheckResult*
:   True if body is valid, false if not; to obtain this value, you must pass True for the DoLocalCheck argument

#### Return Value

True if a set of faces are deleted, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::DeleteFaces3.

# ![](dotnetimages/collapse.gif)Example

[Delete Faces (VBA)](Delete_Faces_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

All of the specified faces, which must belong to this temporary body, are deleted from IBody2. If the resulting body does not have a complete boundary, then SOLIDWORKS treats any holes as wounds and heals them as specified by the option argument. The option argument takes the following values:

|  |  |
| --- | --- |
| **Value** | **Loops on the faces to delete are...** |
| 0 | Dependent on each other and should be healed at the same time. If extending faces does not yield a solution, then SOLIDWORKS tries to shrink the faces. |
| 1 | Independent and should be healed separately. This option also grows the parent faces around the hole to cover it. |
| 2 | Independent and should be healed separately. This option also finds a surface in which all edges of a hole lie and attaches this to a face covering the hole (SOLIDWORKS creates a new face to cover the hole). |

For example, consider a cube with a through hole made up of four faces (a square hole). To delete these four faces, specify option 0 because the loop on the first face to be deleted is dependent on the loop of the second face to be deleted. Likewise, the loop on the second face to be deleted is dependent on the third face to be deleted, and so on.

Now consider the same cube with a through hole, except this through hole is a simple cylinder (one face). To delete the cylindrical face, specify option 1 to heal the loops independently. This is necessary because the cylindrical face actually has two loops (one at either end of the cylinder) that need to be healed separately.

It is possible to generate invalid geometry when you use this method because checking is disabled. Call [IBody2::Check3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~Check3.html) to verify that the body is a valid solid after using this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP1, Revision Number 12
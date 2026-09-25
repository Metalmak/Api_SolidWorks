<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDeleteBlends3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IDeleteBlends3 Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : IDeleteBlends3 Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumOfFaces*
:   Number of faces to delete

*FaceList*
:   * in-process, unmanaged C++: Pointer to an array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) of size NumOfFaces to delete* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*DoLocalCheck*
:   True to perform a local check, false to not

*UsePlanarCap*
:   True to use planar caps, false to not (see **Remarks**)

Removes a set of fillet faces from a temporary body and heals the body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IDeleteBlends3( _    ByVal NumOfFaces As System.Integer, _    ByRef FaceList As Face2, _    ByVal DoLocalCheck As System.Boolean, _    ByVal UsePlanarCap As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim NumOfFaces As System.Integer Dim FaceList As Face2 Dim DoLocalCheck As System.Boolean Dim UsePlanarCap As System.Boolean Dim value As System.Boolean   value = instance.IDeleteBlends3(NumOfFaces, FaceList, DoLocalCheck, UsePlanarCap) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IDeleteBlends3(     System.int NumOfFaces,    ref Face2 FaceList,    System.bool DoLocalCheck,    System.bool UsePlanarCap ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IDeleteBlends3(  &   System.int NumOfFaces, &   Face2^% FaceList, &   System.bool DoLocalCheck, &   System.bool UsePlanarCap ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumOfFaces*
:   Number of faces to delete

*FaceList*
:   * in-process, unmanaged C++: Pointer to an array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) of size NumOfFaces to delete* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*DoLocalCheck*
:   True to perform a local check, false to not

*UsePlanarCap*
:   True to use planar caps, false to not (see **Remarks**)

#### Return Value

True if the set of fillet faces are removed, false if not

# ![](dotnetimages/collapse.gif)Remarks

Typically when deleting blends, an entire chain of blends are deleted. However, if only a few blends are deleted from a chain of blends and the UsePlanarCap parameter is not set to true, then the resultant body might be invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::DeleteBlends3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteBlends3.html)

[IBody2::DeleteFaces5 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteFaces5.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0
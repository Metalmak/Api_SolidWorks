<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDeleteBlends2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IDeleteBlends2 Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : IDeleteBlends2 Method (IBody2) |

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
:   True to perform a local check, false if not

Obsolete. Superseded by [IBody2::DeleteBlends3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IDeleteBlends3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IDeleteBlends2( _    ByVal NumOfFaces As System.Integer, _    ByRef FaceList As Face2, _    ByVal DoLocalCheck As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim NumOfFaces As System.Integer Dim FaceList As Face2 Dim DoLocalCheck As System.Boolean Dim value As System.Boolean   value = instance.IDeleteBlends2(NumOfFaces, FaceList, DoLocalCheck) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IDeleteBlends2(     System.int NumOfFaces,    ref Face2 FaceList,    System.bool DoLocalCheck ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IDeleteBlends2(  &   System.int NumOfFaces, &   Face2^% FaceList, &   System.bool DoLocalCheck ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumOfFaces*
:   Number of faces to delete

*FaceList*
:   * in-process, unmanaged C++: Pointer to an array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) of size NumOfFaces to delete* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*DoLocalCheck*
:   True to perform a local check, false if not

#### Return Value

True if a set of fillet faces are removed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::IDeleteBlends2.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::DeleteBlends2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteBlends2.html)

[IBody2::DeleteFaces5 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteFaces5.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteBlends3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DeleteBlends3 Method (IBody2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : DeleteBlends3 Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FaceList*
:   List of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) to delete

*DoLocalCheck*
:   True to perform a local check, false to not

*UsePlanarCap*
:   True to use planar caps, false to not (see **Remarks**)

Removes a set of fillet faces from a temporary body and heals the body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DeleteBlends3( _    ByVal FaceList As System.Object, _    ByVal DoLocalCheck As System.Boolean, _    ByVal UsePlanarCap As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim FaceList As System.Object Dim DoLocalCheck As System.Boolean Dim UsePlanarCap As System.Boolean Dim value As System.Boolean   value = instance.DeleteBlends3(FaceList, DoLocalCheck, UsePlanarCap) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool DeleteBlends3(     System.object FaceList,    System.bool DoLocalCheck,    System.bool UsePlanarCap ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool DeleteBlends3(  &   System.Object^ FaceList, &   System.bool DoLocalCheck, &   System.bool UsePlanarCap ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FaceList*
:   List of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) to delete

*DoLocalCheck*
:   True to perform a local check, false to not

*UsePlanarCap*
:   True to use planar caps, false to not (see **Remarks**)

#### Return Value

True if the set of fillet faces are removed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::DeleteBlends3.

# ![](dotnetimages/collapse.gif)Example

[Delete Blended Faces (C#)](Delete_Blended_Faces_Example_CSharp.htm)

[Delete Blended Faces (VB.NET)](Delete_Blended_Faces_Example_VBNET.htm)

[Delete Blended Faces (VBA)](Delete_Blended_Faces_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Typically when deleting blends, an entire chain of blends is deleted. However, if only a few blends are deleted from a chain of blends and the UsePlanarCap parameter is not set to true, then the resultant body might be invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::IDeleteBlends3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDeleteBlends3.html)

[IBody5::DeleteFaces5 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteFaces5.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0
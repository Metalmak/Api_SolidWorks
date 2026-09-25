<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentBeadFeatureData~ISetFaces.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISetFaces Method (IWeldmentBeadFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IWeldmentBeadFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentBeadFeatureData.html) : ISetFaces Method (IWeldmentBeadFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Side*
:   Side as defined in swWeldBeadSide\_e

*Count1*
:   Number of faces in the first set of faces

*FaceSet1*
:   * in-process, unmanaged C++: Pointer to an array of the first set of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*Count2*
:   Number of faces in the second set of faces

*FaceSet2*
:   * in-process, unmanaged C++: Pointer to an array of the second set of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

    - VBA, VB.NET, C#, and C++/CLI: Not supported

Sets the faces to which to apply the weld bead.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ISetFaces( _    ByVal Side As System.Integer, _    ByVal Count1 As System.Integer, _    ByRef FaceSet1 As Face2, _    ByVal Count2 As System.Integer, _    ByRef FaceSet2 As Face2 _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IWeldmentBeadFeatureData Dim Side As System.Integer Dim Count1 As System.Integer Dim FaceSet1 As Face2 Dim Count2 As System.Integer Dim FaceSet2 As Face2 Dim value As System.Boolean   value = instance.ISetFaces(Side, Count1, FaceSet1, Count2, FaceSet2) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ISetFaces(     System.int Side,    System.int Count1,    ref Face2 FaceSet1,    System.int Count2,    ref Face2 FaceSet2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ISetFaces(  &   System.int Side, &   System.int Count1, &   Face2^% FaceSet1, &   System.int Count2, &   Face2^% FaceSet2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Side*
:   Side as defined in swWeldBeadSide\_e

*Count1*
:   Number of faces in the first set of faces

*FaceSet1*
:   * in-process, unmanaged C++: Pointer to an array of the first set of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*Count2*
:   Number of faces in the second set of faces

*FaceSet2*
:   * in-process, unmanaged C++: Pointer to an array of the second set of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

    - VBA, VB.NET, C#, and C++/CLI: Not supported

#### Return Value

True if the weld bead is applied to the specified faces, false if not

# ![](dotnetimages/collapse.gif)Remarks

Although you must select planar faces for the face sets, fillet weld beads can follow non-planar, tangent contours when you set [IWeldmentBeadFeatureData::TangentPropagation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IWeldmentBeadFeatureData~TangentPropagation.html) to TRUE.

See Accessing Selections that Define Features for additional details.

# ![](dotnetimages/collapse.gif)See Also

####

[IWeldmentBeadFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentBeadFeatureData.html)

[IWeldmentBeadFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentBeadFeatureData_members.html)

[IWeldmentBeadFeatureData::SetFaces Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentBeadFeatureData~SetFaces.html)

[IWeldmentBeadFeatureData::IGetFaces Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentBeadFeatureData~IGetFaces.html)

[IWeldmentBeadFeatureData::GetFacesCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentBeadFeatureData~GetFacesCount.html)

[IWeldmentBeadFeatureData::GetFaces Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentBeadFeatureData~GetFaces.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0
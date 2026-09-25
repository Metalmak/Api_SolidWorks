<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface3~IGetFirstFaceArray.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetFirstFaceArray Method (IMidSurface3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMidSurface3 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface3.html) : IGetFirstFaceArray Method (IMidSurface3) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FromFrontFaceListDisp*
:   * in-process, unmanaged C++: Pointer to an array of front [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

    :   - VBA, VB.NET, C#, and C++/CLI: Not supported

          See In-process Methods for details about this type of method.

*SizeOfFrontFaceList*
:   Number of front faces

*FromFaceBackListDisp*
:   * in-process, unmanaged C++: Pointer to an array of back [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*SizeOfBackFaceList*
:   :   Number of back faces

*Thickness*
:   Thickness between the faces

Gets the first face and the thickness between the faces.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetFirstFaceArray( _    ByRef FromFrontFaceListDisp As Face2, _    ByRef SizeOfFrontFaceList As System.Integer, _    ByRef FromFaceBackListDisp As Face2, _    ByRef SizeOfBackFaceList As System.Integer, _    ByRef Thickness As System.Double _ ) As Face2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMidSurface3 Dim FromFrontFaceListDisp As Face2 Dim SizeOfFrontFaceList As System.Integer Dim FromFaceBackListDisp As Face2 Dim SizeOfBackFaceList As System.Integer Dim Thickness As System.Double Dim value As Face2   value = instance.IGetFirstFaceArray(FromFrontFaceListDisp, SizeOfFrontFaceList, FromFaceBackListDisp, SizeOfBackFaceList, Thickness) ``` | |

| C# |  |
| --- | --- |
| ``` Face2 IGetFirstFaceArray(     out Face2 FromFrontFaceListDisp,    out System.int SizeOfFrontFaceList,    out Face2 FromFaceBackListDisp,    out System.int SizeOfBackFaceList,    out System.double Thickness ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Face2^ IGetFirstFaceArray(  &   [Out] Face2^ FromFrontFaceListDisp, &   [Out] System.int SizeOfFrontFaceList, &   [Out] Face2^ FromFaceBackListDisp, &   [Out] System.int SizeOfBackFaceList, &   [Out] System.double Thickness ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FromFrontFaceListDisp*
:   * in-process, unmanaged C++: Pointer to an array of front [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

    :   - VBA, VB.NET, C#, and C++/CLI: Not supported

          See In-process Methods for details about this type of method.

*SizeOfFrontFaceList*
:   Number of front faces

*FromFaceBackListDisp*
:   * in-process, unmanaged C++: Pointer to an array of back [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*SizeOfBackFaceList*
:   :   Number of back faces

*Thickness*
:   Thickness between the faces

#### Return Value

First [face](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

# ![](dotnetimages/collapse.gif)Remarks

A separator is needed between the front faces and back faces. Thus, a NULL always exists between the front faces and the back faces.

For example, if there are five faces in the model, then the mid-surface has five faces. To get the five faces:

* Call IMidSurface3::IGetGetFirstFaceArray once.

  * Call [IMidSurface3::IGetNextFaceArray](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMidSurface3~IGetNextFaceArray.html) four times.

At each call, the data is arranged as follows if there is one front face in the array:

[Neutral face], [front face], NULL, [back face]

If there are more than one front face in the array, then the data is arranged as follows:

[Neutral face], [front face1, front face2], NULL, [back face1, back face2]

To get the next face from the original paired faces, call IMidSurface3::IGetNextFaceArray.

# ![](dotnetimages/collapse.gif)See Also

####

[IMidSurface3 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface3.html)

[IMidSurface3 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface3_members.html)

[IMidSurface3::GetFaceCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface3~GetFaceCount.html)

[IMidSurface3::GetFirstFaceArray Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface3~GetFirstFaceArray.html)

[IMidSurface3::GetNextFaceArray Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface3~GetNextFaceArray.html)

[IMidSurface3::IGetNextFaceArray Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface3~IGetNextFaceArray.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0
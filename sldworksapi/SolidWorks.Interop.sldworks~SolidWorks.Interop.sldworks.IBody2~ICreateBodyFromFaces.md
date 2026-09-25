<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateBodyFromFaces.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateBodyFromFaces Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : ICreateBodyFromFaces Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumOfFaces*
:   Number of faces to use to create the body

*FaceList*
:   Array containing the faces to use to create the body

Creates a temporary body from the faces.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateBodyFromFaces( _    ByVal NumOfFaces As System.Integer, _    ByVal FaceList As System.Object _ ) As Body2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim NumOfFaces As System.Integer Dim FaceList As System.Object Dim value As Body2   value = instance.ICreateBodyFromFaces(NumOfFaces, FaceList) ``` | |

| C# |  |
| --- | --- |
| ``` Body2 ICreateBodyFromFaces(     System.int NumOfFaces,    System.object FaceList ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Body2^ ICreateBodyFromFaces(  &   System.int NumOfFaces, &   System.Object^ FaceList ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumOfFaces*
:   Number of faces to use to create the body

*FaceList*
:   Array containing the faces to use to create the body

#### Return Value

[IBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::ICreateBodyFromFaces.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::CreateBodyFromFaces Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateBodyFromFaces.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0
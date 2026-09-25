<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ReplaceSurfaces.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReplaceSurfaces Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ReplaceSurfaces Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NFaces*
:   Number of faces to have surfaces replaced

*FaceArray*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) to have the surfaces replaced

*NewSurfArray*
:   Array of [surfaces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface.html) to be replaced in these faces

*SenseArray*
:   Array of the senses of each surface in NewSurfArray

*Tolerance*
:   Tolerance

Replaces the surfaces of the given faces.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReplaceSurfaces( _    ByVal NFaces As System.Integer, _    ByVal FaceArray As System.Object, _    ByVal NewSurfArray As System.Object, _    ByVal SenseArray As System.Object, _    ByVal Tolerance As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim NFaces As System.Integer Dim FaceArray As System.Object Dim NewSurfArray As System.Object Dim SenseArray As System.Object Dim Tolerance As System.Double Dim value As System.Boolean   value = instance.ReplaceSurfaces(NFaces, FaceArray, NewSurfArray, SenseArray, Tolerance) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ReplaceSurfaces(     System.int NFaces,    System.object FaceArray,    System.object NewSurfArray,    System.object SenseArray,    System.double Tolerance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ReplaceSurfaces(  &   System.int NFaces, &   System.Object^ FaceArray, &   System.Object^ NewSurfArray, &   System.Object^ SenseArray, &   System.double Tolerance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NFaces*
:   Number of faces to have surfaces replaced

*FaceArray*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) to have the surfaces replaced

*NewSurfArray*
:   Array of [surfaces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface.html) to be replaced in these faces

*SenseArray*
:   Array of the senses of each surface in NewSurfArray

*Tolerance*
:   Tolerance

#### Return Value

True if operation is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ReplaceSurfaces.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::IReplaceSurfaces2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~IReplaceSurfaces2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 0.0
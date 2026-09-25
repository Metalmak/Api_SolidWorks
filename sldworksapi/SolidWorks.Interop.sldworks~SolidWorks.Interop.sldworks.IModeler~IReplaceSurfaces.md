<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~IReplaceSurfaces.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IReplaceSurfaces Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : IReplaceSurfaces Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NFaces*

*FaceArray*

*NewSurfArray*

*SenseArray*

*Tolerance*

Obsolete. Superseded by [IModeler::IReplaceSurfaces2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~IReplaceSurfaces2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IReplaceSurfaces( _    ByVal NFaces As System.Integer, _    ByRef FaceArray As Face, _    ByRef NewSurfArray As Surface, _    ByRef SenseArray As System.Integer, _    ByVal Tolerance As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim NFaces As System.Integer Dim FaceArray As Face Dim NewSurfArray As Surface Dim SenseArray As System.Integer Dim Tolerance As System.Double Dim value As System.Boolean   value = instance.IReplaceSurfaces(NFaces, FaceArray, NewSurfArray, SenseArray, Tolerance) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IReplaceSurfaces(     System.int NFaces,    ref Face FaceArray,    ref Surface NewSurfArray,    ref System.int SenseArray,    System.double Tolerance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IReplaceSurfaces(  &   System.int NFaces, &   Face^% FaceArray, &   Surface^% NewSurfArray, &   System.int% SenseArray, &   System.double Tolerance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NFaces*

*FaceArray*

*NewSurfArray*

*SenseArray*

*Tolerance*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::IReplaceSurfaces.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)
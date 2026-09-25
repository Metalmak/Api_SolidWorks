<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreatePlaneAtSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreatePlaneAtSurface Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : CreatePlaneAtSurface Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*InterIndex*

*ProjOpt*

*ReverseDir*

*NormalPlane*

*Angle*

Obsolete. Superseded by [IModelDoc2::CreatePlaneAtSurface3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~ICreatePlaneAtSurface3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub CreatePlaneAtSurface( _    ByVal InterIndex As System.Integer, _    ByVal ProjOpt As System.Boolean, _    ByVal ReverseDir As System.Boolean, _    ByVal NormalPlane As System.Boolean, _    ByVal Angle As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim InterIndex As System.Integer Dim ProjOpt As System.Boolean Dim ReverseDir As System.Boolean Dim NormalPlane As System.Boolean Dim Angle As System.Double   instance.CreatePlaneAtSurface(InterIndex, ProjOpt, ReverseDir, NormalPlane, Angle) ``` | |

| C# |  |
| --- | --- |
| ``` void CreatePlaneAtSurface(     System.int InterIndex,    System.bool ProjOpt,    System.bool ReverseDir,    System.bool NormalPlane,    System.double Angle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CreatePlaneAtSurface(  &   System.int InterIndex, &   System.bool ProjOpt, &   System.bool ReverseDir, &   System.bool NormalPlane, &   System.double Angle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*InterIndex*

*ProjOpt*

*ReverseDir*

*NormalPlane*

*Angle*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::CreatePlaneAtSurface.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)
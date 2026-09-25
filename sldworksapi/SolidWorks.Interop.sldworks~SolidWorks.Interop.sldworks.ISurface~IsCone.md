<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IsCone.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IsCone Method (ISurface) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html) : IsCone Method (ISurface) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether the surface is a cone.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IsCone() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISurface Dim value As System.Boolean   value = instance.IsCone() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsCone() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IsCone(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

True if surface is a cone, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Surface::IsCone.

# ![](dotnetimages/collapse.gif)Example

[Locate Apex of Conical Face (VBA)](Locate_Apex_of_Conical_Face_Example_VB.htm)

[Get Parameters of Conical Surface (VBA)](Get_Parameters_of_Conical_Surface_Example_VB.htm)

[Get Parameters of Conical Surface (VB.NET)](Get_Parameters_of_Conical_Surface_Example_VBNET.htm)

[Get Parameters of Conical Surface (C#)](Get_Parameters_of_Conical_Surface_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Closed cone faces that have an apex point do not have an edge or coedge at the apex.

# ![](dotnetimages/collapse.gif)See Also

####

[ISurface Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html)

[ISurface Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface_members.html)

[ISurface::IConeParams Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IConeParams.html)

[ISurface::ConeParams Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~ConeParams.html)

[IModeler::CreateConicalSurface2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CreateConicalSurface2.html)

[IModeler::ICreateConicalSurface2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICreateConicalSurface2.html)
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~AddProfileLine.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddProfileLine Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : AddProfileLine Method (IBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RootPoint*

*Direction*

Obsolete. Superseded by [IBody2::AddProfileBLine](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~AddProfileLine.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddProfileLine( _    ByVal RootPoint As System.Object, _    ByVal Direction As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim RootPoint As System.Object Dim Direction As System.Object Dim value As System.Object   value = instance.AddProfileLine(RootPoint, Direction) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddProfileLine(     System.object RootPoint,    System.object Direction ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddProfileLine(  &   System.Object^ RootPoint, &   System.Object^ Direction ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RootPoint*

*Direction*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::AddProfileLine.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~AutoDimension.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AutoDimension Method (ISketch) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html) : AutoDimension Method (ISketch) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EntitiesToDimension*

*HorizontalScheme*

*HorizontalPlacement*

*VerticalScheme*

*VerticalPlacement*

Obsolete. Superseded by [ISketch::AutoDimension2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch~AutoDimension2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AutoDimension( _    ByVal EntitiesToDimension As System.Integer, _    ByVal HorizontalScheme As System.Integer, _    ByVal HorizontalPlacement As System.Integer, _    ByVal VerticalScheme As System.Integer, _    ByVal VerticalPlacement As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketch Dim EntitiesToDimension As System.Integer Dim HorizontalScheme As System.Integer Dim HorizontalPlacement As System.Integer Dim VerticalScheme As System.Integer Dim VerticalPlacement As System.Integer Dim value As System.Integer   value = instance.AutoDimension(EntitiesToDimension, HorizontalScheme, HorizontalPlacement, VerticalScheme, VerticalPlacement) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AutoDimension(     System.int EntitiesToDimension,    System.int HorizontalScheme,    System.int HorizontalPlacement,    System.int VerticalScheme,    System.int VerticalPlacement ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AutoDimension(  &   System.int EntitiesToDimension, &   System.int HorizontalScheme, &   System.int HorizontalPlacement, &   System.int VerticalScheme, &   System.int VerticalPlacement ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*EntitiesToDimension*

*HorizontalScheme*

*HorizontalPlacement*

*VerticalScheme*

*VerticalPlacement*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sketch::AutoDimension.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html)

[ISketch Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch_members.html)
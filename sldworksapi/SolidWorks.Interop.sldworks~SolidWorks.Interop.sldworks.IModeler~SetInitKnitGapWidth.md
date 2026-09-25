<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~SetInitKnitGapWidth.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetInitKnitGapWidth Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : SetInitKnitGapWidth Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*InitGapWidth*
:   Desired knitting gap width for body knitting; valid range is from 1e-8 to 0.1 meters

Sets the initial gap bound width for sewing a body. Call this method before calling any calls that attempt to knit a body; for example, [IBody2::CreateBodyFromSurfaces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~CreateBodyFromSurfaces.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetInitKnitGapWidth( _    ByVal InitGapWidth As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim InitGapWidth As System.Double Dim value As System.Boolean   value = instance.SetInitKnitGapWidth(InitGapWidth) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetInitKnitGapWidth(     System.double InitGapWidth ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetInitKnitGapWidth(  &   System.double InitGapWidth ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*InitGapWidth*
:   Desired knitting gap width for body knitting; valid range is from 1e-8 to 0.1 meters

#### Return Value

True if successfully set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::SetInitKnitGapWidth.

# ![](dotnetimages/collapse.gif)Remarks

This initial gap width bound is adjusted during the knitting operation in an attempt to successfully knit a body. Upon completion of the knitting operation, the value is reset to the default value.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)

[IModeler::GetInitKnitGapWidth Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~GetInitKnitGapWidth.html)
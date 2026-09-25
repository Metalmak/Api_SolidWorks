<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStackedBalloonOptions~QuantityPlacement.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| QuantityPlacement Property (IStackedBalloonOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IStackedBalloonOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStackedBalloonOptions.html) : QuantityPlacement Property (IStackedBalloonOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets the placement of a BOM item quantity with respect to its balloon.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property QuantityPlacement As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IStackedBalloonOptions Dim value As System.Integer   instance.QuantityPlacement = value   value = instance.QuantityPlacement ``` | |

| C# |  |
| --- | --- |
| ``` System.int QuantityPlacement {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int QuantityPlacement {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Placement of BOM item quantity value as defined in swBalloonQuantityPlacement\_e; only swBalloonQuantityPlacement\_e.swBalloonQuantityPlacement\_Top and swBalloonQuantityPlacement\_e.swBalloonQuantityPlacement\_Bottom are valid options for stacked balloons

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See StackedBalloonOptions::QuantityPlacement.

# ![](dotnetimages/collapse.gif)Example

See [IStackedBalloonOptions](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStackedBalloonOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

See the SOLIDWORKS Help for additional details about stacked balloons.

# ![](dotnetimages/collapse.gif)See Also

####

[IStackedBalloonOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStackedBalloonOptions.html)

[IStackedBalloonOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStackedBalloonOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0
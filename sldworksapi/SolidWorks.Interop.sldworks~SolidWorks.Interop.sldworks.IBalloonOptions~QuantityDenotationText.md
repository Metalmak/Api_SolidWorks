<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBalloonOptions~QuantityDenotationText.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| QuantityDenotationText Property (IBalloonOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBalloonOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBalloonOptions.html) : QuantityDenotationText Property (IBalloonOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets the label of the BOM item quantity.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property QuantityDenotationText As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBalloonOptions Dim value As System.String   instance.QuantityDenotationText = value   value = instance.QuantityDenotationText ``` | |

| C# |  |
| --- | --- |
| ``` System.string QuantityDenotationText {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ QuantityDenotationText {    System.String^ get();    void set ( &   System.String^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Item quantity label

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BalloonOptions::QuantityDenotationText.

# ![](dotnetimages/collapse.gif)Example

See [IBalloonOptions](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBalloonOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

See the SOLIDWORKS Help for additional details about balloons.

# ![](dotnetimages/collapse.gif)See Also

####

[IBalloonOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBalloonOptions.html)

[IBalloonOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBalloonOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0
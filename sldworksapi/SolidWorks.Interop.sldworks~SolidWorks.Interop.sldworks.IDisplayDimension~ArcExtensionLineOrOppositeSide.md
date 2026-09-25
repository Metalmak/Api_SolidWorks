<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~ArcExtensionLineOrOppositeSide.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ArcExtensionLineOrOppositeSide Property (IDisplayDimension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : ArcExtensionLineOrOppositeSide Property (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to attach or extend the radial dimension leader on this radial display dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ArcExtensionLineOrOppositeSide As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim value As System.Boolean   instance.ArcExtensionLineOrOppositeSide = value   value = instance.ArcExtensionLineOrOppositeSide ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ArcExtensionLineOrOppositeSide {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool ArcExtensionLineOrOppositeSide {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

| If... | Then... |
| --- | --- |
| True | * Attach the radial dimension leader to the arc extension line. - or -* If the radial dimension leader encounters arc geometry, then extend the radial dimension leader to the opposite side of the arc. |
| False | Neither attach nor extend the radial dimension leader. |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::ArcExtensionLineOrOppositeSide.

# ![](dotnetimages/collapse.gif)Example

[Set Radial Dimension Leader (C#)](Edit_Radial_Dimension_Example_CSharp.htm)

[Set Radial Dimension Leader (VB.NET)](Edit_Radial_Dimension_Example_VBNET.htm)

[Set Radial Dimension Leader (VBA)](Edit_Radial_Dimension_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This property is only valid for radial display dimensions.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IModelDoc2::AddRadialDimension2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~AddRadialDimension2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0
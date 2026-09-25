<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SupplementaryAngle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SupplementaryAngle Method (IDisplayDimension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : SupplementaryAngle Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Changes the angle in the selected angular dimension to its supplementary angle.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SupplementaryAngle() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim value As System.Boolean   value = instance.SupplementaryAngle() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SupplementaryAngle() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SupplementaryAngle(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

True if the angle in the selected angular dimension changes to its supplementary angle, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::SupplementaryAngle.

# ![](dotnetimages/collapse.gif)Example

[Change Angle to Supplementary Angle (C#)](Change_Angle_to_Supplementary_Angle_Example_CSharp.htm)

[Change Angle to Supplementary Angle (VB.NET)](Change_Angle_to_Supplementary_Angle_Example_VBNET.htm)

[Change Angle to Supplementary Angle (VBA)](Change_Angle_to_Supplementary_Angle_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

| If the angle in the selected angular dimension is... | Then the supplementary angle is its... |
| --- | --- |
| >180 degrees (i.e., exterior) | Interior angle |
| <180 degrees (i.e., interior) | Exterior angle |

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IModelDocExtension::AddDimension Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~AddDimension.html)

[IModelDoc2::AddDimension2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~AddDimension2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 SP3, Revision Number 24.3
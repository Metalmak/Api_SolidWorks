<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure~Z.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Z Property (IMeasure) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMeasure Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure.html) : Z Property (IMeasure) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the z coordinate of the selected point in model space.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property Z As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMeasure Dim value As System.Double   value = instance.Z ``` | |

| C# |  |
| --- | --- |
| ``` System.double Z {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double Z {    System.double get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

z coordinate of the selected point in model space or -1 if this property is invalid for the selected entity

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Measure::Z.

# ![](dotnetimages/collapse.gif)Example

[Measure Selected Entities (C#)](Measure_Selected_Entities_Example_CSharp.htm)

[Measure Selected Entities (VB.NET)](Measure_Selected_Entities_Example_VBNET.htm)

[Measure Selected Entities (VBA)](Measure_Selected_Entities_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IMeasure Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure.html)

[IMeasure Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure_members.html)

[IMeasure::X Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure~X.html)

[IMeasure::Y Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure~Y.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0
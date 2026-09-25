<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure~Angle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Angle Property (IMeasure) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMeasure Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure.html) : Angle Property (IMeasure) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the angle between the two selected entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property Angle As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMeasure Dim value As System.Double   value = instance.Angle ``` | |

| C# |  |
| --- | --- |
| ``` System.double Angle {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double Angle {    System.double get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Angle in radians between the two selected entities or -1 if this property is invalid for the selected entities

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Measure::Angle.

# ![](dotnetimages/collapse.gif)Example

[Measure Selected Entities (C#)](Measure_Selected_Entities_Example_CSharp.htm)

[Measure Selected Entities (VB.NET)](Measure_Selected_Entities_Example_VBNET.htm)

[Measure Selected Entities (VBA)](Measure_Selected_Entities_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IMeasure Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure.html)

[IMeasure Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure_members.html)

[IMeasure::AngleDecimalPlaces Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure~AngleDecimalPlaces.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0
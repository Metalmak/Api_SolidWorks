<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure~IsIntersect.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IsIntersect Property (IMeasure) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMeasure Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure.html) : IsIntersect Property (IMeasure) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether the two selected entities intersect.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property IsIntersect As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMeasure Dim value As System.Boolean   value = instance.IsIntersect ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsIntersect {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool IsIntersect {    System.bool get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True if the two selected entities intersect, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Measure::IsIntersect.

# ![](dotnetimages/collapse.gif)Example

[Measure Selected Entities (C#)](Measure_Selected_Entities_Example_CSharp.htm)

[Measure Selected Entities (VB.NET)](Measure_Selected_Entities_Example_VBNET.htm)

[Measure Selected Entities (VBA)](Measure_Selected_Entities_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IMeasure Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure.html)

[IMeasure Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure_members.html)

[IMeasure::IsConcentricSpheres Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure~IsConcentricSpheres.html)

[IMeasure::IsParallel Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure~IsParallel.html)

[IMeasure::IsPerpendicular Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure~IsPerpendicular.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0
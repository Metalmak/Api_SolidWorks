<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure~Calculate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Calculate Method (IMeasure) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMeasure Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure.html) : Calculate Method (IMeasure) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Entities*
:   Array of entities to measure; if NULL, then this method measures the selected entities

Measures the selected or specified entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Calculate( _    ByVal Entities As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMeasure Dim Entities As System.Object Dim value As System.Boolean   value = instance.Calculate(Entities) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Calculate(     System.object Entities ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Calculate(  &   System.Object^ Entities ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Entities*
:   Array of entities to measure; if NULL, then this method measures the selected entities

#### Return Value

True if the specified or selected entities are valid types and combination , false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Measure::Calculate.

# ![](dotnetimages/collapse.gif)Example

[Measure Selected Entities (C#)](Measure_Selected_Entities_Example_CSharp.htm)

[Measure Selected Entities (VB.NET)](Measure_Selected_Entities_Example_VBNET.htm)

[Measure Selected Entities (VBA)](Measure_Selected_Entities_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IMeasure Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure.html)

[IMeasure Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMeasure_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0
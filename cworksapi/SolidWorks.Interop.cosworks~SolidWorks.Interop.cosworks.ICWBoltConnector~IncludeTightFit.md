<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector~IncludeTightFit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| IncludeTightFit Property (ICWBoltConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBoltConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector.html) : IncludeTightFit Property (ICWBoltConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to include tight fit if the radius of the shank is equal to the radius of the cylindrical faces associated with at least one of the components.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property IncludeTightFit As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBoltConnector Dim value As System.Boolean   instance.IncludeTightFit = value   value = instance.IncludeTightFit ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IncludeTightFit {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool IncludeTightFit {    System.bool get();    void set ( &   System.bool value); } ``` | |

#### Property Value

True to include tight fit, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWBoltConnector::IncludeTightFit.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBoltConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector.html)

[ICWBoltConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector_members.html)

[ICWBoltConnector::InsertTightFitEntity Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector~InsertTightFitEntity.html)

[ICWBoltConnector::RemoveTightFitEntity Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector~RemoveTightFitEntity.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0
<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector~InsertEntityAtSecondLocation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| InsertEntityAtSecondLocation Method (ICWBoltConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBoltConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector.html) : InsertEntityAtSecondLocation Method (ICWBoltConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispEntity*
:   Target entity (face, edge, or plane depending on the type of bolt connector)

Inserts a target entity at the second location.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertEntityAtSecondLocation( _    ByVal DispEntity As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBoltConnector Dim DispEntity As System.Object   instance.InsertEntityAtSecondLocation(DispEntity) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertEntityAtSecondLocation(     System.object DispEntity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertEntityAtSecondLocation(  &   System.Object^ DispEntity ) ``` | |

#### Parameters

*DispEntity*
:   Target entity (face, edge, or plane depending on the type of bolt connector)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWBoltConnector::InsertEntityAtSecondLocation.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBoltConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector.html)

[ICWBoltConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector_members.html)

[ICWBoltConnector::InsertEntityAtFirstLocation Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector~InsertEntityAtFirstLocation.html)

[ICWBoltConnector::RemoveEntityAtSecondLocation Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector~RemoveEntityAtSecondLocation.html)

[ICWBoltConnector::RemoveEntityAtFirstLocation Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBoltConnector~RemoveEntityAtFirstLocation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0
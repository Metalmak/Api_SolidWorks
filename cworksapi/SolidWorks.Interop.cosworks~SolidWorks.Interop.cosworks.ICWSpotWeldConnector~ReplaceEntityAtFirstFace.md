<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpotWeldConnector~ReplaceEntityAtFirstFace.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ReplaceEntityAtFirstFace Method (ICWSpotWeldConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWSpotWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpotWeldConnector.html) : ReplaceEntityAtFirstFace Method (ICWSpotWeldConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispEntity*
:   Spot-weld entity (a face of a shell or solid body)

Replaces the spot-weld entity (a face of a shell or solid body) on the first face.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ReplaceEntityAtFirstFace( _    ByVal DispEntity As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWSpotWeldConnector Dim DispEntity As System.Object   instance.ReplaceEntityAtFirstFace(DispEntity) ``` | |

| C# |  |
| --- | --- |
| ``` void ReplaceEntityAtFirstFace(     System.object DispEntity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ReplaceEntityAtFirstFace(  &   System.Object^ DispEntity ) ``` | |

#### Parameters

*DispEntity*
:   Spot-weld entity (a face of a shell or solid body)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWSpotWeldConnector::ReplaceEntityAtFirstFace.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWSpotWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpotWeldConnector.html)

[ICWSpotWeldConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpotWeldConnector_members.html)

[ICWSpotWeldConnector::ReplaceEntityAtSecondFace Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpotWeldConnector~ReplaceEntityAtSecondFace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0
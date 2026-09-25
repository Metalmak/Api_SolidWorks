<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpotWeldConnector~RemoveSpotWeldLocationAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| RemoveSpotWeldLocationAt Method (ICWSpotWeldConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWSpotWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpotWeldConnector.html) : RemoveSpotWeldLocationAt Method (ICWSpotWeldConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NIndex*
:   0-based index at which to remove the spot weld

Removes the spot-weld location at the specified index.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub RemoveSpotWeldLocationAt( _    ByVal NIndex As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWSpotWeldConnector Dim NIndex As System.Integer   instance.RemoveSpotWeldLocationAt(NIndex) ``` | |

| C# |  |
| --- | --- |
| ``` void RemoveSpotWeldLocationAt(     System.int NIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RemoveSpotWeldLocationAt(  &   System.int NIndex ) ``` | |

#### Parameters

*NIndex*
:   0-based index at which to remove the spot weld

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWSpotWeldConnector::RemoveSpotWeldLocationAt.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ICWSpotWeldLocation::GetSpotWeldLocationCount](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWSpotWeldConnector~GetSpotWeldLocationCount.html) to determine the value of NIndex.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWSpotWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpotWeldConnector.html)

[ICWSpotWeldConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpotWeldConnector_members.html)

[ICWSpotWEldConnector::InsertSpotWeldLocations Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpotWeldConnector~InsertSpotWeldLocations.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0
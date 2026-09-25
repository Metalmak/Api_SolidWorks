<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationDamperFeatureData~SetEndPoints.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetEndPoints Method (ISimulationDamperFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISimulationDamperFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationDamperFeatureData.html) : SetEndPoints Method (ISimulationDamperFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PDirDisp1*
:   Damper end point

*PDirDisp2*
:   Damper end point

Sets the end points for this damper feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetEndPoints( _    ByVal PDirDisp1 As System.Object, _    ByVal PDirDisp2 As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISimulationDamperFeatureData Dim PDirDisp1 As System.Object Dim PDirDisp2 As System.Object Dim value As System.Boolean   value = instance.SetEndPoints(PDirDisp1, PDirDisp2) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetEndPoints(     System.object PDirDisp1,    System.object PDirDisp2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetEndPoints(  &   System.Object^ PDirDisp1, &   System.Object^ PDirDisp2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PDirDisp1*
:   Damper end point

*PDirDisp2*
:   Damper end point

#### Return Value

True if the operation succeeds, false if it fails

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SimulationDamperFeatureData::SetEndPoints.

# ![](dotnetimages/collapse.gif)Example

See [ISimulationDamperFeatureData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISimulationDamperFeatureData.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ISimulationDamperFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationDamperFeatureData.html)

[ISimulationDamperFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationDamperFeatureData_members.html)

[ISimulationDamperFeatureData::GetEndPoints Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationDamperFeatureData~GetEndPoints.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0
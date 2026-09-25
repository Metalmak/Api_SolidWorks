<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationLinearSpringFeatureData~SetEndPoints.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetEndPoints Method (ISimulationLinearSpringFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISimulationLinearSpringFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationLinearSpringFeatureData.html) : SetEndPoints Method (ISimulationLinearSpringFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PDirDisp1*
:   Linear edge, vertex, or sketch point

*PDirDisp2*
:   Linear edge, vertex, or sketch point

Obsolete. Superseded by [ISimulationSpringFeatureData::SetEndPoints](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISimulationSpringFeatureData~SetEndPoints.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetEndPoints( _    ByVal PDirDisp1 As System.Object, _    ByVal PDirDisp2 As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISimulationLinearSpringFeatureData Dim PDirDisp1 As System.Object Dim PDirDisp2 As System.Object   instance.SetEndPoints(PDirDisp1, PDirDisp2) ``` | |

| C# |  |
| --- | --- |
| ``` void SetEndPoints(     System.object PDirDisp1,    System.object PDirDisp2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetEndPoints(  &   System.Object^ PDirDisp1, &   System.Object^ PDirDisp2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PDirDisp1*
:   Linear edge, vertex, or sketch point

*PDirDisp2*
:   Linear edge, vertex, or sketch point

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SimulationLinearSpringFeatureData::SetEndPoints.

# ![](dotnetimages/collapse.gif)See Also

####

[ISimulationLinearSpringFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationLinearSpringFeatureData.html)

[ISimulationLinearSpringFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationLinearSpringFeatureData_members.html)

[ISimulationLinearspringFeatureData::GetEndPoints Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationLinearSpringFeatureData~GetEndPoints.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0
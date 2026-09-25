<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationLinearSpringFeatureData~GetEndPoints.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetEndPoints Method (ISimulationLinearSpringFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISimulationLinearSpringFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationLinearSpringFeatureData.html) : GetEndPoints Method (ISimulationLinearSpringFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PDirDisp1*
:   Linear edge, vertex, sketch segment, or sketch point

*PDirDisp2*
:   Linear edge, vertex, sketch segment, or sketch point

*Type1*
:   Type of end point as defined in swSelectType\_e

*Type2*
:   Type of end point as defined in swSelectType\_e

Obsolete. Superseded by [ISimulationSpringFeatureData::GetEndPoints](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISimulationSpringFeatureData~GetEndPoints.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetEndPoints( _    ByRef PDirDisp1 As System.Object, _    ByRef PDirDisp2 As System.Object, _    ByRef Type1 As System.Integer, _    ByRef Type2 As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISimulationLinearSpringFeatureData Dim PDirDisp1 As System.Object Dim PDirDisp2 As System.Object Dim Type1 As System.Integer Dim Type2 As System.Integer   instance.GetEndPoints(PDirDisp1, PDirDisp2, Type1, Type2) ``` | |

| C# |  |
| --- | --- |
| ``` void GetEndPoints(     out System.object PDirDisp1,    out System.object PDirDisp2,    out System.int Type1,    out System.int Type2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetEndPoints(  &   [Out] System.Object^ PDirDisp1, &   [Out] System.Object^ PDirDisp2, &   [Out] System.int Type1, &   [Out] System.int Type2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PDirDisp1*
:   Linear edge, vertex, sketch segment, or sketch point

*PDirDisp2*
:   Linear edge, vertex, sketch segment, or sketch point

*Type1*
:   Type of end point as defined in swSelectType\_e

*Type2*
:   Type of end point as defined in swSelectType\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SimulationLinearSpringFeatureData::GetEndPoints.

# ![](dotnetimages/collapse.gif)See Also

####

[ISimulationLinearSpringFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationLinearSpringFeatureData.html)

[ISimulationLinearSpringFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationLinearSpringFeatureData_members.html)

[ISimulationLinearSpringFeatureData::SetEndPoints Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationLinearSpringFeatureData~SetEndPoints.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData~ModifyMemberParameters.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ModifyMemberParameters Method (IBeltChainFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBeltChainFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData.html) : ModifyMemberParameters Method (IBeltChainFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PulleyCompObject*
:   Pulley component

*Diameter*
:   Diameter > 0.0 to change; 0.0 to not change

*Flip*
:   True to flip the belt side, false to not

Changes diameter and whether to flip the belt side of the specified pulley component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ModifyMemberParameters( _    ByVal PulleyCompObject As System.Object, _    ByVal Diameter As System.Double, _    ByVal Flip As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBeltChainFeatureData Dim PulleyCompObject As System.Object Dim Diameter As System.Double Dim Flip As System.Boolean Dim value As System.Boolean   value = instance.ModifyMemberParameters(PulleyCompObject, Diameter, Flip) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ModifyMemberParameters(     System.object PulleyCompObject,    System.double Diameter,    System.bool Flip ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ModifyMemberParameters(  &   System.Object^ PulleyCompObject, &   System.double Diameter, &   System.bool Flip ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PulleyCompObject*
:   Pulley component

*Diameter*
:   Diameter > 0.0 to change; 0.0 to not change

*Flip*
:   True to flip the belt side, false to not

#### Return Value

True if pulley component successfully modifed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BeltChainFeatureData::ModifyMemberParameters.

# ![](dotnetimages/collapse.gif)See Also

####

[IBeltChainFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData.html)

[IBeltChainFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30
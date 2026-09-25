<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetIgesInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetIgesInfo Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : SetIgesInfo Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SystemName*
:   Name of the system as defined in swIGESPreferredSystem\_e

*Granularity*
:   Level of granularity

*AttemptKnitting*
:   True knits the objects, false does not

Sends IGES-specific data to the geometric modeler.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetIgesInfo( _    ByVal SystemName As System.String, _    ByVal Granularity As System.Double, _    ByVal AttemptKnitting As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim SystemName As System.String Dim Granularity As System.Double Dim AttemptKnitting As System.Boolean   instance.SetIgesInfo(SystemName, Granularity, AttemptKnitting) ``` | |

| C# |  |
| --- | --- |
| ``` void SetIgesInfo(     System.string SystemName,    System.double Granularity,    System.bool AttemptKnitting ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetIgesInfo(  &   System.String^ SystemName, &   System.double Granularity, &   System.bool AttemptKnitting ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SystemName*
:   Name of the system as defined in swIGESPreferredSystem\_e

*Granularity*
:   Level of granularity

*AttemptKnitting*
:   True knits the objects, false does not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::SetIgesInfo.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0
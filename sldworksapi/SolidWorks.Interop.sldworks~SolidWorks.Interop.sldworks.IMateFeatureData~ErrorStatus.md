<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateFeatureData~ErrorStatus.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ErrorStatus Property (IMateFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateFeatureData.html) : ErrorStatus Property (IMateFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the status of adding or editing this mate.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property ErrorStatus As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMateFeatureData Dim value As System.Integer   value = instance.ErrorStatus ``` | |

| C# |  |
| --- | --- |
| ``` System.int ErrorStatus {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int ErrorStatus {    System.int get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Status of adding or editing this mate as defined in swAddMateError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MateFeatureData::ErrorStatus.

# ![](dotnetimages/collapse.gif)See Also

####

[IMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateFeatureData.html)

[IMateFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetHoleStandards.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetHoleStandards Method (IHoleStandardsData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IHoleStandardsData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData.html) : GetHoleStandards Method (IHoleStandardsData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Indexes*
:   Array of Hole Wizard standards as defined in swWzdHoleStandards\_e

*Names*
:   Array of names of Hole Wizard standards

Gets Hole Wizard standards.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetHoleStandards( _    ByRef Indexes As System.Object, _    ByRef Names As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IHoleStandardsData Dim Indexes As System.Object Dim Names As System.Object Dim value As System.Boolean   value = instance.GetHoleStandards(Indexes, Names) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetHoleStandards(     out System.object Indexes,    out System.object Names ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetHoleStandards(  &   [Out] System.Object^ Indexes, &   [Out] System.Object^ Names ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Indexes*
:   Array of Hole Wizard standards as defined in swWzdHoleStandards\_e

*Names*
:   Array of names of Hole Wizard standards

#### Return Value

True if Hole Wizard standards retrieved successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See HoleStandardsData::GetHoleStandards.

# ![](dotnetimages/collapse.gif)Example

See the [IHoleStandardsData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData.html) example.

# ![](dotnetimages/collapse.gif)See Also

####

[IHoleStandardsData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData.html)

[IHoleStandardsData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData_members.html)

[IHoleStandardsData::GetFastenerTable Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetFastenerTable.html)

[IHoleStandardsData::GetFastenerTableTypes Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetFastenerTableTypes.html)

[IHoleStandardsData::GetFastenerTypes Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetFastenerTypes.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0
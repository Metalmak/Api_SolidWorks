<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~GetZoneSizeDistribution.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetZoneSizeDistribution Method (ISheet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html) : GetZoneSizeDistribution Method (ISheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Rows*
:   Zone rows; Nothing or null if the zone size distribution is swZoneSizeDistribution\_e.swZoneSizeDistribution\_50mmFromCenter

*Columns*
:   Zone columns; Nothing or null if the zone size distribution is swZoneSizeDistribution\_e.swZoneSizeDistribution\_50mmFromCenter

Gets the zone size distribution.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetZoneSizeDistribution( _    ByRef Rows As System.Integer, _    ByRef Columns As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheet Dim Rows As System.Integer Dim Columns As System.Integer Dim value As System.Integer   value = instance.GetZoneSizeDistribution(Rows, Columns) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetZoneSizeDistribution(     out System.int Rows,    out System.int Columns ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetZoneSizeDistribution(  &   [Out] System.int Rows, &   [Out] System.int Columns ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Rows*
:   Zone rows; Nothing or null if the zone size distribution is swZoneSizeDistribution\_e.swZoneSizeDistribution\_50mmFromCenter

*Columns*
:   Zone columns; Nothing or null if the zone size distribution is swZoneSizeDistribution\_e.swZoneSizeDistribution\_50mmFromCenter

#### Return Value

Zone size distribution as defined by swZoneSizeDistribution\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sheet::GetZoneSizeDistribution.

# ![](dotnetimages/collapse.gif)See Also

####

[ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html)

[ISheet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30
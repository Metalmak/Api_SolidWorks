<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetZoneSizeDistribution.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetZoneSizeDistribution Method (ISheet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html) : SetZoneSizeDistribution Method (ISheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   Type of zone size distribution as defined by swZoneSizeDistribution\_e

*Rows*
:   Number of zone rows; valid only if Type is swZoneSizeDistribution.swZoneSizeDistribution\_EvenlySized

*Column*
:   Number of zone columns; valid only if Type is swZoneSizeDistribution.swZoneSizeDistribution\_EvenlySized

Sets the zone size distribution.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetZoneSizeDistribution( _    ByVal Type As System.Integer, _    ByVal Rows As System.Integer, _    ByVal Column As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheet Dim Type As System.Integer Dim Rows As System.Integer Dim Column As System.Integer Dim value As System.Boolean   value = instance.SetZoneSizeDistribution(Type, Rows, Column) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetZoneSizeDistribution(     System.int Type,    System.int Rows,    System.int Column ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetZoneSizeDistribution(  &   System.int Type, &   System.int Rows, &   System.int Column ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*
:   Type of zone size distribution as defined by swZoneSizeDistribution\_e

*Rows*
:   Number of zone rows; valid only if Type is swZoneSizeDistribution.swZoneSizeDistribution\_EvenlySized

*Column*
:   Number of zone columns; valid only if Type is swZoneSizeDistribution.swZoneSizeDistribution\_EvenlySized

#### Return Value

True if zone size distribution successfully set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sheet::SetZoneSizeDistribution.

# ![](dotnetimages/collapse.gif)See Also

####

[ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html)

[ISheet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30
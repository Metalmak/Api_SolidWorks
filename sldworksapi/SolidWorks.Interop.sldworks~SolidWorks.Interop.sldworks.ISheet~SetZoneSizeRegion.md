<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetZoneSizeRegion.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetZoneSizeRegion Method (ISheet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html) : SetZoneSizeRegion Method (ISheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RegionType*
:   Type of zone size region as defined by swRegionType\_e

Sets the type of zone size region.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetZoneSizeRegion( _    ByVal RegionType As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheet Dim RegionType As System.Integer Dim value As System.Boolean   value = instance.SetZoneSizeRegion(RegionType) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetZoneSizeRegion(     System.int RegionType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetZoneSizeRegion(  &   System.int RegionType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RegionType*
:   Type of zone size region as defined by swRegionType\_e

#### Return Value

True of zone size region successfully set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sheet::SetZoneSizeRegion.

# ![](dotnetimages/collapse.gif)See Also

####

[ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html)

[ISheet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30
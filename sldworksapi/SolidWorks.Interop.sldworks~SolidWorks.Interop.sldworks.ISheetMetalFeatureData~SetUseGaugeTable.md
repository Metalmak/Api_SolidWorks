<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData~SetUseGaugeTable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetUseGaugeTable Method (ISheetMetalFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheetMetalFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData.html) : SetUseGaugeTable Method (ISheetMetalFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseGaugeTable*
:   True to use a gauge table, false to not

*GaugeTableFile*
:   Gauge table file name; valid only if UseGaugeTable is true

Sets whether to use a sheet metal feature gauge table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetUseGaugeTable( _    ByVal UseGaugeTable As System.Boolean, _    ByVal GaugeTableFile As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheetMetalFeatureData Dim UseGaugeTable As System.Boolean Dim GaugeTableFile As System.String Dim value As System.Integer   value = instance.SetUseGaugeTable(UseGaugeTable, GaugeTableFile) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetUseGaugeTable(     System.bool UseGaugeTable,    System.string GaugeTableFile ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetUseGaugeTable(  &   System.bool UseGaugeTable, &   System.String^ GaugeTableFile ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseGaugeTable*
:   True to use a gauge table, false to not

*GaugeTableFile*
:   Gauge table file name; valid only if UseGaugeTable is true

#### Return Value

Result code as defined in swSheetMetalModifierError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SheetMetalFeatureData::SetUseGaugeTable.

# ![](dotnetimages/collapse.gif)See Also

####

[ISheetMetalFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData.html)

[ISheetMetalFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData_members.html)

[ISheetMetalFeatureData::GetUseGaugeTable Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData~GetUseGaugeTable.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0
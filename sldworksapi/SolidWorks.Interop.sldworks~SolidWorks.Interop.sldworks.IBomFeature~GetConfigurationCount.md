<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~GetConfigurationCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetConfigurationCount Method (IBomFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature.html) : GetConfigurationCount Method (IBomFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OnlyVisible*
:   True to get the number of configurations currently displayed in this table, false to get the total number of configurations available in this table

Gets the number of configurations available to this BOM table or used in this BOM table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetConfigurationCount( _    ByVal OnlyVisible As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomFeature Dim OnlyVisible As System.Boolean Dim value As System.Integer   value = instance.GetConfigurationCount(OnlyVisible) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetConfigurationCount(     System.bool OnlyVisible ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetConfigurationCount(  &   System.bool OnlyVisible ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OnlyVisible*
:   True to get the number of configurations currently displayed in this table, false to get the total number of configurations available in this table

#### Return Value

Number of configurations in this BOM table or available to this BOM table

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BomFeature::GetConfigurationCount.

# ![](dotnetimages/collapse.gif)Remarks

The view associated with this BOM can contain a model with multiple configurations.

For a top-level only style BOM table, there can be several Quantity columns, each showing the results for a different configuration.  For the other styles of BOM tables, only a particular configuration can be shown in the table, and that configuration can be changed. To determine the style of the BOM table, use [IBomFeature::TableType](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomFeature~TableType.html).

|  |  |
| --- | --- |
| **If OnlyVisible is...** | **Then the value returned is...** |
| True | Number of configurations currently shown in the BOM table.  For a top-level only style BOM table, this could be any number from 0 to the total number of configurations available. For the other styles of BOM tables, this value is always 1. |
| false | Total number of configurations available. |

To get the configuration names, call [IBomFeature::GetConfigurations](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomFeature~GetConfigurations.html) or [IBomFeature::IGetConfigurations](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomFeature~IGetConfigurations.html).

Call this method before calling IBomFeature::IGetConfigurations to get the number of configurations.

# ![](dotnetimages/collapse.gif)See Also

####

[IBomFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature.html)

[IBomFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12
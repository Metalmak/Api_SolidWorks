<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData~SetInstanceDimensionValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetInstanceDimensionValue Method (IDimPatternFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDimPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData.html) : SetInstanceDimensionValue Method (IDimPatternFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TableRowIndex*
:   Index of the pattern instance in the pattern table (see **Remarks**)

*ControlDimName*
:   Name of the controlling dimension of the pattern instance (see **Remarks**)

*NewValue*
:   New value for the pattern dimension

Sets a new value for the pattern dimension of the specified pattern instance in this variable pattern feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetInstanceDimensionValue( _    ByVal TableRowIndex As System.Integer, _    ByVal ControlDimName As System.String, _    ByVal NewValue As System.Double _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimPatternFeatureData Dim TableRowIndex As System.Integer Dim ControlDimName As System.String Dim NewValue As System.Double Dim value As System.String   value = instance.SetInstanceDimensionValue(TableRowIndex, ControlDimName, NewValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.string SetInstanceDimensionValue(     System.int TableRowIndex,    System.string ControlDimName,    System.double NewValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ SetInstanceDimensionValue(  &   System.int TableRowIndex, &   System.String^ ControlDimName, &   System.double NewValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TableRowIndex*
:   Index of the pattern instance in the pattern table (see **Remarks**)

*ControlDimName*
:   Name of the controlling dimension of the pattern instance (see **Remarks**)

*NewValue*
:   New value for the pattern dimension

#### Return Value

| If a new value for the pattern dimension is... | Then Return Value is an... |
| --- | --- |
| Set | Empty string indicating success |
| Not set | Error string |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimPatternFeatureData::SetInstanceDimensionValue.

# ![](dotnetimages/collapse.gif)Example

[Delete and Insert Instances in Variable Pattern Feature (C#)](Delete_and_Insert_Instances_in_Variable_Pattern_Feature_Example_CSharp.htm)

[Delete and Insert Instances in Variable Pattern Feature (VB.NET)](Delete_and_Insert_Instances_in_Variable_Pattern_Feature_Example_VBNET.htm)

[Delete and Insert Instances in Variable Pattern Feature (VBA)](Delete_and_Insert_Instances_in_Variable_Pattern_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use:

* [IDimPatternFeatureData::GetTableRowIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData~GetTableRowIndex.html) to get TableRowIndex.* [IDimPatternFeatureData::GetControllingDimensionName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData~GetControllingDimensionName.html) to get ControlDimName.

# ![](dotnetimages/collapse.gif)See Also

####

[IDimPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData.html)

[IDimPatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData_members.html)

[IDimPatternFeatureData::GetInstanceDimensionName Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData~GetInstanceDimensionName.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0
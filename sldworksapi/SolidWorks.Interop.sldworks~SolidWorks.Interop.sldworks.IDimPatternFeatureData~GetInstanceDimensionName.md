<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData~GetInstanceDimensionName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetInstanceDimensionName Method (IDimPatternFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDimPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData.html) : GetInstanceDimensionName Method (IDimPatternFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*InstanceName*
:   Name of the pattern instance (see **Remarks**)

*ControllingDimName*
:   Controlling dimension of the pattern instance (see **Remarks**)

Gets the name of the pattern dimension for the pattern instance in this variable pattern feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetInstanceDimensionName( _    ByVal InstanceName As System.String, _    ByVal ControllingDimName As System.String _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimPatternFeatureData Dim InstanceName As System.String Dim ControllingDimName As System.String Dim value As System.String   value = instance.GetInstanceDimensionName(InstanceName, ControllingDimName) ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetInstanceDimensionName(     System.string InstanceName,    System.string ControllingDimName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetInstanceDimensionName(  &   System.String^ InstanceName, &   System.String^ ControllingDimName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*InstanceName*
:   Name of the pattern instance (see **Remarks**)

*ControllingDimName*
:   Controlling dimension of the pattern instance (see **Remarks**)

#### Return Value

Name of the pattern dimension

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimPatternFeatureData::GetInstanceDimensionName.

# ![](dotnetimages/collapse.gif)Example

[Insert Variable Pattern Feature (C#)](Insert_Advanced_Variable_Pattern_Feature_Example_CSharp.htm)

[Insert Variable Pattern Feature (VB.NET)](Insert_Advanced_Variable_Pattern_Feature_Example_VBNET.htm)

[Insert Variable Pattern Feature (VBA)](Insert_Advanced_Variable_Pattern_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

| Use.. | To get... |
| --- | --- |
| [IDimPatternFeatureData::GetInstanceNameByIndex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData~GetInstanceNameByIndex.html) | InstanceName |
| [IDimPatternFeatureData::GetControllingDimensionName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData~GetControllingDimensionName.html) | ControllingDimName |

# ![](dotnetimages/collapse.gif)See Also

####

[IDimPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData.html)

[IDimPatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData_members.html)

[IDimPatternFeatureData::SetInstanceDimensionValue Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData~SetInstanceDimensionValue.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0
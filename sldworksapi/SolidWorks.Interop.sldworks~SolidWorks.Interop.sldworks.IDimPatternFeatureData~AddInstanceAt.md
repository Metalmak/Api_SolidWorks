<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData~AddInstanceAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddInstanceAt Method (IDimPatternFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDimPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData.html) : AddInstanceAt Method (IDimPatternFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IsSuppressed*
:   True to suppress this pattern instance, false to not

*Index*
:   0-based index indicating where to add this pattern instance in the pattern table and pattern; -1 indicates to add this pattern instance to the end of the pattern table and pattern (see **Remarks**)

Adds a pattern instance to this variable pattern feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddInstanceAt( _    ByVal IsSuppressed As System.Boolean, _    ByVal Index As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimPatternFeatureData Dim IsSuppressed As System.Boolean Dim Index As System.Integer Dim value As System.Boolean   value = instance.AddInstanceAt(IsSuppressed, Index) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddInstanceAt(     System.bool IsSuppressed,    System.int Index ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddInstanceAt(  &   System.bool IsSuppressed, &   System.int Index ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IsSuppressed*
:   True to suppress this pattern instance, false to not

*Index*
:   0-based index indicating where to add this pattern instance in the pattern table and pattern; -1 indicates to add this pattern instance to the end of the pattern table and pattern (see **Remarks**)

#### Return Value

True if the pattern instance is added, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimPatternFeatureData::AddInstanceAt.

# ![](dotnetimages/collapse.gif)Example

[Delete and Insert Instances in Variable Pattern Feature (C#)](Delete_and_Insert_Instances_in_Variable_Pattern_Feature_Example_CSharp.htm)

[Delete and Insert Instances in Variable Pattern Feature (VB.NET)](Delete_and_Insert_Instances_in_Variable_Pattern_Feature_Example_VBNET.htm)

[Delete and Insert Instances in Variable Pattern Feature (VBA)](Delete_and_Insert_Instances_in_Variable_Pattern_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use [IDimPatternFeatureData::GetInstanceCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData~GetInstanceCount.html) to get the number of pattern instances.

By default, this pattern instance inherits the default values of the parent sketch or feature of the variable pattern feature. Use [IDimPatternFeatureData::SetInstanceDimensionValue](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData~SetInstanceDimensionValue.html) to modify this pattern instance's values.

# ![](dotnetimages/collapse.gif)See Also

####

[IDimPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData.html)

[IDimPatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData_members.html)

[IDimPatternFeatureData::DeleteInstanceAt Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData~DeleteInstanceAt.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0
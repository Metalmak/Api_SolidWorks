<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertVaryInstanceIncrement.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertVaryInstanceIncrement Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertVaryInstanceIncrement Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DName*
:   | If IncrementType is... | Then set DName to... |
    | --- | --- |
    | 1 | Name of the pattern instance dimension to increment |
    | 2 | "Spacing Increment" |

*PatternType*
:   Type of pattern (see **Remarks**):

    * 2 = linear* 4 = circular* 256 = table-driven

*IncrementType*
:   Type of increment:

    * 1 = dimension* 2 = spacing

*Direction*
:   Direction in which to apply the dimension or spacing increment.

    | If PatternType is... | Then set Direction to... |
    | --- | --- |
    | 2 | * 0 = direction 1  * 1 = direction 2 |
    | 4 | 0 = direction 1 |

*IncrementValue*
:   Value with which to increment the pattern instance dimension or spacing

Obsolete. Superseded by [IInstanceToVaryOptions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertVaryInstanceIncrement( _    ByVal DName As System.String, _    ByVal PatternType As System.Integer, _    ByVal IncrementType As System.Integer, _    ByVal Direction As System.Integer, _    ByVal IncrementValue As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim DName As System.String Dim PatternType As System.Integer Dim IncrementType As System.Integer Dim Direction As System.Integer Dim IncrementValue As System.Double Dim value As System.Boolean   value = instance.InsertVaryInstanceIncrement(DName, PatternType, IncrementType, Direction, IncrementValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertVaryInstanceIncrement(     System.string DName,    System.int PatternType,    System.int IncrementType,    System.int Direction,    System.double IncrementValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertVaryInstanceIncrement(  &   System.String^ DName, &   System.int PatternType, &   System.int IncrementType, &   System.int Direction, &   System.double IncrementValue ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DName*
:   | If IncrementType is... | Then set DName to... |
    | --- | --- |
    | 1 | Name of the pattern instance dimension to increment |
    | 2 | "Spacing Increment" |

*PatternType*
:   Type of pattern (see **Remarks**):

    * 2 = linear* 4 = circular* 256 = table-driven

*IncrementType*
:   Type of increment:

    * 1 = dimension* 2 = spacing

*Direction*
:   Direction in which to apply the dimension or spacing increment.

    | If PatternType is... | Then set Direction to... |
    | --- | --- |
    | 2 | * 0 = direction 1  * 1 = direction 2 |
    | 4 | 0 = direction 1 |

*IncrementValue*
:   Value with which to increment the pattern instance dimension or spacing

#### Return Value

True if the increment is applied successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertVaryInstanceIncrement.

# ![](dotnetimages/collapse.gif)Remarks

To vary the spacings or dimensions of pattern instances:

1. Call this method multiple times to increment multiple dimensions or spacings of pattern instances.- Call [IFeatureManager::InsertVaryInstanceOverride](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertVaryInstanceOverride.html) multiple times to override multiple dimensions or spacings of pattern instances.

| If PatternType is... | Call IFeatureManager::CreateFeature(...) |
| --- | --- |
| 2 | LinearPatternFeatureData object |
| 4 | CircularPatternFeatureData object |
| 256 | DimPatternFeatureData object |

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0
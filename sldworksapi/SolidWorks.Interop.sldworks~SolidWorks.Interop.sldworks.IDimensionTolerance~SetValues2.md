<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimensionTolerance~SetValues2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetValues2 Method (IDimensionTolerance) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDimensionTolerance Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimensionTolerance.html) : SetValues2 Method (IDimensionTolerance) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MinValue*
:   Dimension tolerance minimum value

*MaxValue*
:   Dimension tolerance maximum value

*WhichConfigurations*
:   Configurations to which to set the dimension tolerance minimum and maximum values as defined in swSetValueInConfiguration\_e

*Config\_names*
:   Names of the configurations for which to set dimension tolerance values

Sets the tolerance minimum and maximum values of a [dimension](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetValues2( _    ByVal MinValue As System.Double, _    ByVal MaxValue As System.Double, _    ByVal WhichConfigurations As System.Integer, _    ByVal Config_names As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimensionTolerance Dim MinValue As System.Double Dim MaxValue As System.Double Dim WhichConfigurations As System.Integer Dim Config_names As System.Object Dim value As System.Boolean   value = instance.SetValues2(MinValue, MaxValue, WhichConfigurations, Config_names) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetValues2(     System.double MinValue,    System.double MaxValue,    System.int WhichConfigurations,    System.object Config_names ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetValues2(  &   System.double MinValue, &   System.double MaxValue, &   System.int WhichConfigurations, &   System.Object^ Config_names ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MinValue*
:   Dimension tolerance minimum value

*MaxValue*
:   Dimension tolerance maximum value

*WhichConfigurations*
:   Configurations to which to set the dimension tolerance minimum and maximum values as defined in swSetValueInConfiguration\_e

*Config\_names*
:   Names of the configurations for which to set dimension tolerance values

#### Return Value

True if the dimension tolerance values are set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimensionTolerance::SetValues2.

# ![](dotnetimages/collapse.gif)Example

[Change Dimension Tolerance in a Configuration (C#)](Change_Dimension_Tolerance_in_Configuration_Example_CSharp.htm)

[Change Dimension Tolerance in a Configuration (VB.NET)](Change_Dimension_Tolerance_in_Configuration_Example_VBNET.htm)

[Change Dimension Tolerance in a Configuration (VBA)](Change_Dimension_Tolerance_in_Configuration_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You cannot set the dimension tolerance values if the [tolerance type](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~Type.html) is swTolType\_e.swTolNONE. Depending on the tolerance type, the dimension tolerance minimum and maximum values might not be visible.

|  |  |
| --- | --- |
| **To get the dimension tolerance...** | **Use...** |
| Minimum value | [IDimensionTolerance::GetMinValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetMinValue.html) |
| Maximum value | [IDimensionTolerance::GetMaxValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetMaxValue.html) |

To see the effects of changing the dimension tolerance values, call [IModelView::GraphicsRedraw](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView~GraphicsRedraw.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IDimensionTolerance Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimensionTolerance.html)

[IDimensionTolerance Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimensionTolerance_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 SP04, Revision Number 21.4
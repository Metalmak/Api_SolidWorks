<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData~GetOverrideDefaultParameter2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetOverrideDefaultParameter2 Method (ISheetMetalFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheetMetalFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData.html) : GetOverrideDefaultParameter2 Method (ISheetMetalFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Parameter*
:   Default parameter as defined in swSheetMetalOverrideDefaultParameters\_e

*OverrideDefaultParameter*
:   True if Parameter is overridden, false if not

Gets whether the specified default parameter is overridden in this sheet metal feature in a multibody sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetOverrideDefaultParameter2( _    ByVal Parameter As System.Integer, _    ByRef OverrideDefaultParameter As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheetMetalFeatureData Dim Parameter As System.Integer Dim OverrideDefaultParameter As System.Boolean Dim value As System.Integer   value = instance.GetOverrideDefaultParameter2(Parameter, OverrideDefaultParameter) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetOverrideDefaultParameter2(     System.int Parameter,    out System.bool OverrideDefaultParameter ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetOverrideDefaultParameter2(  &   System.int Parameter, &   [Out] System.bool OverrideDefaultParameter ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Parameter*
:   Default parameter as defined in swSheetMetalOverrideDefaultParameters\_e

*OverrideDefaultParameter*
:   True if Parameter is overridden, false if not

#### Return Value

Result code as defined in swSheetMetalModifierError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SheetMetalFeatureData::GetOverrideDefaultParameter2.

# ![](dotnetimages/collapse.gif)Example

[Set Override Option for Auto Relief Default Parameters (C#)](Set_Override_Option_for_Auto_Relief_Default_Parameters_Example_CSharp.htm)

[Set Override Option for Auto Relief Default Parameters (VB.NET)](Set_Override_Option_for_Auto_Relief_Default_Parameters_Example_VBNET.htm)

[Set Override Option for Auto Relief Default Parameters (VBA)](Set_Override_Option_for_Auto_Relief_Default_Parameters_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This property is only valid for multibody sheet metal parts created in SOLIDWORKS 2013 and later.

# ![](dotnetimages/collapse.gif)See Also

####

[ISheetMetalFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData.html)

[ISheetMetalFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData_members.html)

[ISheetMetalFeatureData::SetOverrideDefaultParameter2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData~SetOverrideDefaultParameter2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0
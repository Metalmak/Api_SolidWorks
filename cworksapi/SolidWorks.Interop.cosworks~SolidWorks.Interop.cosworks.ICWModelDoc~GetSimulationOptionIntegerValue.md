<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~GetSimulationOptionIntegerValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetSimulationOptionIntegerValue Method (ICWModelDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) : GetSimulationOptionIntegerValue Method (ICWModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UserPreferenceValue*
:   User preference as defined by [swsUserPreferenceIntegerValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUserPreferenceIntegerValue_e.html)

Gets the integer value for the specified user preference.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSimulationOptionIntegerValue( _    ByVal UserPreferenceValue As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWModelDoc Dim UserPreferenceValue As System.Integer Dim value As System.Integer   value = instance.GetSimulationOptionIntegerValue(UserPreferenceValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetSimulationOptionIntegerValue(     System.int UserPreferenceValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetSimulationOptionIntegerValue(  &   System.int UserPreferenceValue ) ``` | |

#### Parameters

*UserPreferenceValue*
:   User preference as defined by [swsUserPreferenceIntegerValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUserPreferenceIntegerValue_e.html)

#### Return Value

Integer value (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWModelDoc::GetSimulationOptionIntegerValue.

# ![](dotnetimages/collapse.gif)Example

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (VBA)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_VB.htm)

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (VB.NET)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_VBNET.htm)

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (C#)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Values for colors are defined in [swsWindowsBasicColors\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsWindowsBasicColors_e.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html)

[ICWModelDoc Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc_members.html)

[ICWModelDoc::SetSimulationOptionIntegerValue Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~SetSimulationOptionIntegerValue.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2014 SP0
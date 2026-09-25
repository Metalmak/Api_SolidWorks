<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~SetSimulationOptionIntegerValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetSimulationOptionIntegerValue Method (ICWModelDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) : SetSimulationOptionIntegerValue Method (ICWModelDoc) |

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

*Value*
:   Integer value (see **Remarks**)

Sets the integer value for the specified user preference.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSimulationOptionIntegerValue( _    ByVal UserPreferenceValue As System.Integer, _    ByVal Value As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWModelDoc Dim UserPreferenceValue As System.Integer Dim Value As System.Integer Dim value As System.Boolean   value = instance.SetSimulationOptionIntegerValue(UserPreferenceValue, Value) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSimulationOptionIntegerValue(     System.int UserPreferenceValue,    System.int Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSimulationOptionIntegerValue(  &   System.int UserPreferenceValue, &   System.int Value ) ``` | |

#### Parameters

*UserPreferenceValue*
:   User preference as defined by [swsUserPreferenceIntegerValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUserPreferenceIntegerValue_e.html)

*Value*
:   Integer value (see **Remarks**)

#### Return Value

True if option successfully set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWModelDoc::SetSimulationOptionIntegerValue.

# ![](dotnetimages/collapse.gif)Example

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (VBA)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_VB.htm)

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (VB.NET)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_VBNET.htm)

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (C#)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To set color options you can either:

1. Locate the color you want, for example swsAqua, from [swsWindowsBasicColors\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsWindowsBasicColors_e.html).- Call this method, specifying Value with the integer value for swsAqua, 16776960, e.g., ICWModelDoc::SetSimulationOptionIntegerValue(swsUserPreferenceIntegerValue\_e.swsPlotShowHiddenBodyTranslucentSingleColor, 16776960).

-or-

1. Select a color from <http://cloford.com/resources/colours/500col.htm> (e.g., #FF0000 is the hexadecimal for Red 1).- Reverse the hexadecimal value of the selected color (e.g., #0000FF is the reverse hexadecimal for Red 1).- Call [ICWModelDoc::SetSimulationOptionIntegerValue](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWModelDoc~SetSimulationOptionIntegerValue.html)(swsUserPreferenceIntegerValue\_e.*option*, &h*color\_reverse\_hexadecimal*), e.g., ICWModelDoc::SetSimulationOptionIntegerValue(swsUserPreferenceIntegerValue\_e.swsPlotShowHiddenBodyTranslucentSingleColor, &h0000ff).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html)

[ICWModelDoc Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc_members.html)

[ICWModelDoc::GetSimulationOptionIntegerValue Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~GetSimulationOptionIntegerValue.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2014 SP0
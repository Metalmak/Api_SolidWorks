<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~SetSimulationOptionToggle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetSimulationOptionToggle Method (ICWModelDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) : SetSimulationOptionToggle Method (ICWModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NUserPreferenceValue*
:   User preference as defined by [swsUserPreferenceToggle\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUserPreferenceToggle_e.html)

*BValue*
:   Boolean value

Sets the boolean value for the specified user preference.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSimulationOptionToggle( _    ByVal NUserPreferenceValue As System.Integer, _    ByVal BValue As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWModelDoc Dim NUserPreferenceValue As System.Integer Dim BValue As System.Boolean Dim value As System.Boolean   value = instance.SetSimulationOptionToggle(NUserPreferenceValue, BValue) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSimulationOptionToggle(     System.int NUserPreferenceValue,    System.bool BValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSimulationOptionToggle(  &   System.int NUserPreferenceValue, &   System.bool BValue ) ``` | |

#### Parameters

*NUserPreferenceValue*
:   User preference as defined by [swsUserPreferenceToggle\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUserPreferenceToggle_e.html)

*BValue*
:   Boolean value

#### Return Value

True if option successfully set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWModelDoc::SetSimulationOptionToggle.

# ![](dotnetimages/collapse.gif)Example

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (VBA)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_VB.htm)

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (VB.NET)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_VBNET.htm)

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (C#)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWModelDoc Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html)

[ICWModelDoc Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc_members.html)

[ICWModelDoc::GetSimulationOptionToggle Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc~GetSimulationOptionToggle.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2014 SP0
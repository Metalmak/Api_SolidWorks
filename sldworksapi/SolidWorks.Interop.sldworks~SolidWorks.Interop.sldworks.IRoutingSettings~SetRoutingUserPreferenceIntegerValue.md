<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings~SetRoutingUserPreferenceIntegerValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetRoutingUserPreferenceIntegerValue Method (IRoutingSettings) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRoutingSettings Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html) : SetRoutingUserPreferenceIntegerValue Method (IRoutingSettings) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UserPreferenceValue*
:   User preference as defined in swUserPreferenceRoutingInteger\_e

*Value*
:   Integer value of the specified user preference

Sets an integer value for the specified routing user preference.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetRoutingUserPreferenceIntegerValue( _    ByVal UserPreferenceValue As System.Integer, _    ByVal Value As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingSettings Dim UserPreferenceValue As System.Integer Dim Value As System.Integer Dim value As System.Boolean   value = instance.SetRoutingUserPreferenceIntegerValue(UserPreferenceValue, Value) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetRoutingUserPreferenceIntegerValue(     System.int UserPreferenceValue,    System.int Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetRoutingUserPreferenceIntegerValue(  &   System.int UserPreferenceValue, &   System.int Value ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UserPreferenceValue*
:   User preference as defined in swUserPreferenceRoutingInteger\_e

*Value*
:   Integer value of the specified user preference

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RoutingSettings::SetRoutingUserPreferenceIntegerValue.

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingSettings Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html)

[IRoutingSettings Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings_members.html)

[IRoutingSettings::GetRoutingUserPreferenceIntegerValue Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings~GetRoutingUserPreferenceIntegerValue.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0
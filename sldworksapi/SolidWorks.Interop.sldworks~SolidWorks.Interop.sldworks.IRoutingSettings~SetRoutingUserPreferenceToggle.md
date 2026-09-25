<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings~SetRoutingUserPreferenceToggle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetRoutingUserPreferenceToggle Method (IRoutingSettings) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRoutingSettings Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html) : SetRoutingUserPreferenceToggle Method (IRoutingSettings) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UserPreferenceValue*
:   User preference as defined in swUserPreferenceRoutingToggle\_e

*OnFlag*
:   True to turn on, false to turn off

Sets whether the specified routing user preference is turned on or off.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetRoutingUserPreferenceToggle( _    ByVal UserPreferenceValue As System.Integer, _    ByVal OnFlag As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingSettings Dim UserPreferenceValue As System.Integer Dim OnFlag As System.Boolean   instance.SetRoutingUserPreferenceToggle(UserPreferenceValue, OnFlag) ``` | |

| C# |  |
| --- | --- |
| ``` void SetRoutingUserPreferenceToggle(     System.int UserPreferenceValue,    System.bool OnFlag ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetRoutingUserPreferenceToggle(  &   System.int UserPreferenceValue, &   System.bool OnFlag ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UserPreferenceValue*
:   User preference as defined in swUserPreferenceRoutingToggle\_e

*OnFlag*
:   True to turn on, false to turn off

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RoutingSettings::SetRoutingUserPreferenceToggle.

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingSettings Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html)

[IRoutingSettings Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings_members.html)

[IRoutingSettings::GetRoutingUserPreferenceToggle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings~GetRoutingUserPreferenceToggle.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0
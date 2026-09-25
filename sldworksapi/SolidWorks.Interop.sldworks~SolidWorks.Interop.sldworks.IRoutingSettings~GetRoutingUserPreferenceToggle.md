<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings~GetRoutingUserPreferenceToggle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetRoutingUserPreferenceToggle Method (IRoutingSettings) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRoutingSettings Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html) : GetRoutingUserPreferenceToggle Method (IRoutingSettings) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UserPreferenceToggle*
:   User preference as defined in swUserPreferenceRoutingToggle\_e

Gets whether the specified routing user preference is turned on.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetRoutingUserPreferenceToggle( _    ByVal UserPreferenceToggle As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingSettings Dim UserPreferenceToggle As System.Integer Dim value As System.Boolean   value = instance.GetRoutingUserPreferenceToggle(UserPreferenceToggle) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetRoutingUserPreferenceToggle(     System.int UserPreferenceToggle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetRoutingUserPreferenceToggle(  &   System.int UserPreferenceToggle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UserPreferenceToggle*
:   User preference as defined in swUserPreferenceRoutingToggle\_e

#### Return Value

True if on, false if off

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RoutingSettings::GetRoutingUserPreferenceToggle.

# ![](dotnetimages/collapse.gif)Example

See the [IRoutingSettings](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingSettings Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html)

[IRoutingSettings Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings_members.html)

[IRoutingSettings::SetRoutingUserPreferenceToggle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings~SetRoutingUserPreferenceToggle.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0
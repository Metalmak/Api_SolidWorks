<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_SuppressionStateChangeNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_SuppressionStateChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_SuppressionStateChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Feature*
:   [Feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) that changed suppression state

*NewSuppressionState*
:   New suppression state for the feature as defined by swFeatureSuppressionAction\_e

*PreviousSuppressionState*
:   Previous suppression state for the feature as defined by swFeatureSuppressionAction\_e

*ConfigurationOption*
:   Configuration option as defined by swInConfigurationOpts\_e

*ConfigurationNames*
:   Array of configurations in which the suppression state of the feature changes

Fired when the suppression state of a feature changes.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_SuppressionStateChangeNotifyEventHandler( _    ByVal Feature As Feature, _    ByVal NewSuppressionState As System.Integer, _    ByVal PreviousSuppressionState As System.Integer, _    ByVal ConfigurationOption As System.Integer, _    ByRef ConfigurationNames As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_SuppressionStateChangeNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_SuppressionStateChangeNotifyEventHandler(     Feature Feature,    System.int NewSuppressionState,    System.int PreviousSuppressionState,    System.int ConfigurationOption,    ref System.object ConfigurationNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_SuppressionStateChangeNotifyEventHandler(  &   Feature^ Feature, &   System.int NewSuppressionState, &   System.int PreviousSuppressionState, &   System.int ConfigurationOption, &   System.Object^% ConfigurationNames ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Feature*
:   [Feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) that changed suppression state

*NewSuppressionState*
:   New suppression state for the feature as defined by swFeatureSuppressionAction\_e

*PreviousSuppressionState*
:   Previous suppression state for the feature as defined by swFeatureSuppressionAction\_e

*ConfigurationOption*
:   Configuration option as defined by swInConfigurationOpts\_e

*ConfigurationNames*
:   Array of configurations in which the suppression state of the feature changes

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SuppressionStateChangeNotify Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swAssemblySuppressionStateChangeNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0
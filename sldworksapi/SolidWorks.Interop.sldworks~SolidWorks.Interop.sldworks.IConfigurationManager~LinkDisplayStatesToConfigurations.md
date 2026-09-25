<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~LinkDisplayStatesToConfigurations.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| LinkDisplayStatesToConfigurations Property (IConfigurationManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html) : LinkDisplayStatesToConfigurations Property (IConfigurationManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to link or unlink display states to or from the active configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property LinkDisplayStatesToConfigurations As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfigurationManager Dim value As System.Boolean   instance.LinkDisplayStatesToConfigurations = value   value = instance.LinkDisplayStatesToConfigurations ``` | |

| C# |  |
| --- | --- |
| ``` System.bool LinkDisplayStatesToConfigurations {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool LinkDisplayStatesToConfigurations {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to keep specific display states linked to the active configuration, false to unlink specific display states and make all display states available to the active configuration

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ConfigurationManager::LinkDisplayStatesToConfigurations.

# ![](dotnetimages/collapse.gif)Example

[Link Display States to Configurations (C#)](Link_Display_States_to_Configurations_Example_CSharp.htm)

[Link Display States to Configurations (VB.NET)](Link_Display_States_to_Configurations_Example_VBNET.htm)

[Link Display States to Configurations (VBA)](Link_Display_States_to_Configurations_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html)

[IConfigurationManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager_members.html)

[IComponent2::ReferencedDisplayState Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ReferencedDisplayState.html)

[IConfiguration::ApplyDisplayState Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~ApplyDisplayState.html)

[IConfiguration::CopyDisplayStateFromConfiguration Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~CopyDisplayStateFromConfiguration.html)

[IConfiguration::CreateDisplayState Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~CreateDisplayState.html)

[IConfiguration::GetDisplayStates Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetDisplayStates.html)

[IConfiguration::IGetDisplayStates Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~IGetDisplayStates.html)

[IModelDocExtension::LinkedDisplayState Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~LinkedDisplayState.html)

[IPartDoc::RemoveAllDisplayStates Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~RemoveAllDisplayStates.html)

[IAssemblyDoc ActiveDisplayStateChangePostNotify Event](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_ActiveDisplayStateChangePostNotifyEventHandler.html)

[IAssemblyDoc ActiveDisplayStateChangePreNotify Event](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_ActiveDisplayStateChangePreNotifyEventHandler.html)

[IPartDoc ActiveDisplayStateChangePostNotify Event](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_ActiveDisplayStateChangePostNotifyEventHandler.html)

[IPartDoc ActiveDisplayStateChangePreNotify Event](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_ActiveDisplayStateChangePreNotifyEventHandler.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 SP03, Revision Number 20.3
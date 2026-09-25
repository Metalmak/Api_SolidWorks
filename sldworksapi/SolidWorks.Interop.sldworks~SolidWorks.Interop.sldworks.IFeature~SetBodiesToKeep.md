<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetBodiesToKeep.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetBodiesToKeep Method (IFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) : SetBodiesToKeep Method (IFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AllBodies*
:   True to keep all bodies, false to not

*BodiesToKeep*
:   Array of bodies to keep

*ConfigOption*
:   Configuration options as defined in swInConfigurationOpts\_e

*ConfigNames*
:   Array of configuration names

Set the bodies to keep and their configurations for features that create multiple bodies in parts and assemblies.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetBodiesToKeep( _    ByVal AllBodies As System.Boolean, _    ByVal BodiesToKeep As System.Object, _    ByVal ConfigOption As System.Integer, _    ByVal ConfigNames As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeature Dim AllBodies As System.Boolean Dim BodiesToKeep As System.Object Dim ConfigOption As System.Integer Dim ConfigNames As System.Object   instance.SetBodiesToKeep(AllBodies, BodiesToKeep, ConfigOption, ConfigNames) ``` | |

| C# |  |
| --- | --- |
| ``` void SetBodiesToKeep(     System.bool AllBodies,    System.object BodiesToKeep,    System.int ConfigOption,    System.object ConfigNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetBodiesToKeep(  &   System.bool AllBodies, &   System.Object^ BodiesToKeep, &   System.int ConfigOption, &   System.Object^ ConfigNames ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AllBodies*
:   True to keep all bodies, false to not

*BodiesToKeep*
:   Array of bodies to keep

*ConfigOption*
:   Configuration options as defined in swInConfigurationOpts\_e

*ConfigNames*
:   Array of configuration names

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Feature::SetBodiesToKeep.

# ![](dotnetimages/collapse.gif)Example

[Cut Body and Keep All Bodies (C#)](Cut_Body_and_Keep_All_Bodies_Example_CSharp.htm)

[Cut Body and Keep All Bodies (VB.NET)](Cut_Body_and_Keep_All_Bodies_Example_VBNET.htm)

[Cut Body and Keep All Bodies (VBA)](Cut_Body_and_Keep_All_Bodies_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

[IFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature_members.html)

[IAssemblyDoc PromptBodiesToKeepNotify Event](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_PromptBodiesToKeepNotifyEventHandler.html)

[IPartDoc PromptBodiesToKeepNotify Event](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_PromptBodiesToKeepNotifyEventHandler.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0
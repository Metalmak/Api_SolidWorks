<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~SetSpeedPakConfigurations.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetSpeedPakConfigurations Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : SetSpeedPakConfigurations Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Config\_opt*
:   Configuration option as defined in swInConfigurationOpts\_e (see **Remarks**)

*Config\_names*
:   Array of the names of the configurations in the selected subassemblies to which to apply SpeedPak; valid only if Config\_opt = swInConfigurationOpts\_e.swSpecifyConfiguration (see **Remarks**)

Sets the configurations in the selected subassemblies to which to apply SpeedPak in this assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSpeedPakConfigurations( _    ByVal Config_opt As System.Integer, _    ByVal Config_names As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim Config_opt As System.Integer Dim Config_names As System.Object Dim value As System.Boolean   value = instance.SetSpeedPakConfigurations(Config_opt, Config_names) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSpeedPakConfigurations(     System.int Config_opt,    System.object Config_names ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSpeedPakConfigurations(  &   System.int Config_opt, &   System.Object^ Config_names ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Config\_opt*
:   Configuration option as defined in swInConfigurationOpts\_e (see **Remarks**)

*Config\_names*
:   Array of the names of the configurations in the selected subassemblies to which to apply SpeedPak; valid only if Config\_opt = swInConfigurationOpts\_e.swSpecifyConfiguration (see **Remarks**)

#### Return Value

True if the specified configurations in the selected subassemblies are applied SpeedPak, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::SetSpeedPakConfigurations.

# ![](dotnetimages/collapse.gif)Remarks

Valid option for Config\_opt is:

* swInConfigurationOpts\_e.swAllConfiguration,* swInConfigurationOpts\_e.swSpecifyConfiguration, or* swInConfigurationOpts\_e.swThisConfiguration

If Config\_names = swInConfigurationOpts\_e.swAllConfiguration or swInConfigurationOpts\_e.swThisConfiguration, then pass Nothing or null.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::CreateSpeedPak Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CreateSpeedPak.html)

[IAssemblyDoc::SetSpeedPakToParent Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~SetSpeedPakToParent.html)

[IAssemblyDoc::UpdateSpeedPak Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~UpdateSpeedPak.html)

[IAssemblyDoc::UseSpeedPak Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~UseSpeedPak.html)

[IAssemblyDoc::IsSpeedPak Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsSpeedPak.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0
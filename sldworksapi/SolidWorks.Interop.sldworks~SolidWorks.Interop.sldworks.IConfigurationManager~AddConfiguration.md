<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddConfiguration.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddConfiguration Method (IConfigurationManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html) : AddConfiguration Method (IConfigurationManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   Name of the configuration

*Comment*
:   Comment displayed in Configuration Properties

*AlternateName*
:   Alternate configuration name (i.e., user-specified name); used if swConfigOption\_UseAlternateName is set to true

*Options*
:   Combination of one or more Boolean configuration options as defined in swConfigurationOptions2\_e (see **Remarks**)

*ParentConfigName*
:   Name of parent configuration

*Description*
:   Text that identifies the configuration

Obsolete. Superseded by [IConfigurationManager::AddConfiguration2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddConfiguration2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddConfiguration( _    ByVal Name As System.String, _    ByVal Comment As System.String, _    ByVal AlternateName As System.String, _    ByVal Options As System.Integer, _    ByVal ParentConfigName As System.String, _    ByVal Description As System.String _ ) As Configuration ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfigurationManager Dim Name As System.String Dim Comment As System.String Dim AlternateName As System.String Dim Options As System.Integer Dim ParentConfigName As System.String Dim Description As System.String Dim value As Configuration   value = instance.AddConfiguration(Name, Comment, AlternateName, Options, ParentConfigName, Description) ``` | |

| C# |  |
| --- | --- |
| ``` Configuration AddConfiguration(     System.string Name,    System.string Comment,    System.string AlternateName,    System.int Options,    System.string ParentConfigName,    System.string Description ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Configuration^ AddConfiguration(  &   System.String^ Name, &   System.String^ Comment, &   System.String^ AlternateName, &   System.int Options, &   System.String^ ParentConfigName, &   System.String^ Description ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Name of the configuration

*Comment*
:   Comment displayed in Configuration Properties

*AlternateName*
:   Alternate configuration name (i.e., user-specified name); used if swConfigOption\_UseAlternateName is set to true

*Options*
:   Combination of one or more Boolean configuration options as defined in swConfigurationOptions2\_e (see **Remarks**)

*ParentConfigName*
:   Name of parent configuration

*Description*
:   Text that identifies the configuration

#### Return Value

Newly created [configuration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfiguration.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ConfigurationManager::AddConfiguration.

# ![](dotnetimages/collapse.gif)Example

[Set Dimensions to Mid-Tolerance (VBA)](Set_Dimensions_to_Mid-Tolerance_Example_VB.htm)

[Add Derived Configurations (VBA)](Add_Derived_Configurations_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The Options argument can be a combination of any of the following values:

* swConfigOption\_SuppressByDefault - True if you want to suppress newly added features and mates in this configuration, false if not* swConfigOption\_HideByDefault - True if you want newly added components to be hidden, false if not* swConfigOption\_MinFeatureManager - True if you want newly added components to only display their component name in the FeatureManager design tree, false if you want newly added components to display their name and each of their features in the FeatureManager design tree

# ![](dotnetimages/collapse.gif)See Also

####

[IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html)

[IConfigurationManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager_members.html)

[IAssembly::AddComponentConfiguration Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddComponentConfiguration.html)

[IComponent2::Name2 Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Name2.html)

[IConfiguration::AlternateName Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~AlternateName.html)

[IConfiguration::GetParent Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetParent.html)

[IConfiguration::GetChildren Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetChildren.html)

[IConfiguration::IGetChildren Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~IGetChildren.html)

[IConfiguration::Name Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~Name.html)

[IConfigurationManager::ActiveConfiguration Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~ActiveConfiguration.html)

[IModelDoc2::AddConfiguration3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~AddConfiguration3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 SP1, Revision Number 11.1
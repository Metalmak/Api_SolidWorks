<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddConfiguration2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddConfiguration2 Method (IConfigurationManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html) : AddConfiguration2 Method (IConfigurationManager) |

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
:   Alternate configuration name (i.e., user-specified name); used if Options is set to swConfigurationOptions2\_e\_UseAlternateName

*Options*
:   Combination of one or more configuration options as defined in swConfigurationOptions2\_e (see **Remarks**)

*ParentConfigName*
:   Name of parent configuration

*Description*
:   Text that identifies the configuration

*Rebuild*
:   True to rebuild the model after adding this configuration, false to not

Creates a new configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddConfiguration2( _    ByVal Name As System.String, _    ByVal Comment As System.String, _    ByVal AlternateName As System.String, _    ByVal Options As System.Integer, _    ByVal ParentConfigName As System.String, _    ByVal Description As System.String, _    ByVal Rebuild As System.Boolean _ ) As Configuration ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfigurationManager Dim Name As System.String Dim Comment As System.String Dim AlternateName As System.String Dim Options As System.Integer Dim ParentConfigName As System.String Dim Description As System.String Dim Rebuild As System.Boolean Dim value As Configuration   value = instance.AddConfiguration2(Name, Comment, AlternateName, Options, ParentConfigName, Description, Rebuild) ``` | |

| C# |  |
| --- | --- |
| ``` Configuration AddConfiguration2(     System.string Name,    System.string Comment,    System.string AlternateName,    System.int Options,    System.string ParentConfigName,    System.string Description,    System.bool Rebuild ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Configuration^ AddConfiguration2(  &   System.String^ Name, &   System.String^ Comment, &   System.String^ AlternateName, &   System.int Options, &   System.String^ ParentConfigName, &   System.String^ Description, &   System.bool Rebuild ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Name of the configuration

*Comment*
:   Comment displayed in Configuration Properties

*AlternateName*
:   Alternate configuration name (i.e., user-specified name); used if Options is set to swConfigurationOptions2\_e\_UseAlternateName

*Options*
:   Combination of one or more configuration options as defined in swConfigurationOptions2\_e (see **Remarks**)

*ParentConfigName*
:   Name of parent configuration

*Description*
:   Text that identifies the configuration

*Rebuild*
:   True to rebuild the model after adding this configuration, false to not

#### Return Value

Newly created [configuration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfiguration.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ConfigurationManager::AddConfiguration2.

# ![](dotnetimages/collapse.gif)Example

[Work with Configurations (VBA)](Work_with_Configurations_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The Options argument can be a combination of any of the following values:

* swConfigOption\_SuppressByDefault* swConfigOption\_HideByDefault* swConfigOption\_MinFeatureManager* swConfigOption\_UseAlternateName

# ![](dotnetimages/collapse.gif)See Also

####

[IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html)

[IConfigurationManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager_members.html)

[IAssemblyDoc::AddComponentConfiguration Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddComponentConfiguration.html)

[IModelDoc2::AddConfiguration3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~AddConfiguration3.html)

[IConfiguration::GetChildren Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetChildren.html)

[IConfiguration::GetParent Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~GetParent.html)

[IConfiguration::Name Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~Name.html)

[IConfigurationManager::ActiveConfiguration Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~ActiveConfiguration.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0
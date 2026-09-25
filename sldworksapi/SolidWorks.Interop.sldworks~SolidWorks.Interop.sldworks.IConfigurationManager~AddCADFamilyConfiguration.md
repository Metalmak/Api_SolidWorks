<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager~AddCADFamilyConfiguration.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddCADFamilyConfiguration Method (IConfigurationManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html) : AddCADFamilyConfiguration Method (IConfigurationManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   Name of the configuration to add

*Description*
:   Details about the configuration

*IsPhysicalProduct*
:   True to add a parent configuration (Physical Product), false to add a derived configuration (Representation)

*RepresentationParentName*
:   Parent Physical Product name of derived configuration (Representation); valid only if IsPhysicalProduct is false

*ConfigOptions*
:   Configuration options as defined by swCADFamilyCfgOptions\_e

*ChildCompDisplayOption*
:   Child component display option as defined in swChildComponentInBOMOption\_e

*Rebuild*
:   True to rebuild the model after adding this configuration, false to not

Adds the specified configuration to SOLIDWORKS Connected.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddCADFamilyConfiguration( _    ByVal Name As System.String, _    ByVal Description As System.String, _    ByVal IsPhysicalProduct As System.Boolean, _    ByVal RepresentationParentName As System.String, _    ByVal ConfigOptions As System.Integer, _    ByVal ChildCompDisplayOption As System.Integer, _    ByVal Rebuild As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfigurationManager Dim Name As System.String Dim Description As System.String Dim IsPhysicalProduct As System.Boolean Dim RepresentationParentName As System.String Dim ConfigOptions As System.Integer Dim ChildCompDisplayOption As System.Integer Dim Rebuild As System.Boolean Dim value As System.Object   value = instance.AddCADFamilyConfiguration(Name, Description, IsPhysicalProduct, RepresentationParentName, ConfigOptions, ChildCompDisplayOption, Rebuild) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddCADFamilyConfiguration(     System.string Name,    System.string Description,    System.bool IsPhysicalProduct,    System.string RepresentationParentName,    System.int ConfigOptions,    System.int ChildCompDisplayOption,    System.bool Rebuild ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddCADFamilyConfiguration(  &   System.String^ Name, &   System.String^ Description, &   System.bool IsPhysicalProduct, &   System.String^ RepresentationParentName, &   System.int ConfigOptions, &   System.int ChildCompDisplayOption, &   System.bool Rebuild ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Name of the configuration to add

*Description*
:   Details about the configuration

*IsPhysicalProduct*
:   True to add a parent configuration (Physical Product), false to add a derived configuration (Representation)

*RepresentationParentName*
:   Parent Physical Product name of derived configuration (Representation); valid only if IsPhysicalProduct is false

*ConfigOptions*
:   Configuration options as defined by swCADFamilyCfgOptions\_e

*ChildCompDisplayOption*
:   Child component display option as defined in swChildComponentInBOMOption\_e

*Rebuild*
:   True to rebuild the model after adding this configuration, false to not

#### Return Value

[IConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ConfigurationManager::AddCADFamilyConfiguration.

# ![](dotnetimages/collapse.gif)See Also

####

[IConfigurationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager.html)

[IConfigurationManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfigurationManager_members.html)

[IConfiguration::Get3DExperienceType Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~Get3DExperienceType.html)

[IConfiguration::Set3DExperienceType Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~Set3DExperienceType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30
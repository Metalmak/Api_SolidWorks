<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~GetActiveGroundPlane.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetActiveGroundPlane Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : GetActiveGroundPlane Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Config\_opt*
:   Configurations from which to retrieve active ground planes as defined in swInConfigurationOpts\_e:

    * swThisConfiguration* swAllConfigurations* swSpecifyConfiguration

    (see **Remarks**)

*Config\_names*
:   Array of the names of configurations from which to retrieve active ground planes; valid only if Config\_opt is set to swInConfiguration\_e.swSpecifyConfiguration (see **Remarks**)

Gets the active ground plane for the specified configurations.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetActiveGroundPlane( _    ByVal Config_opt As System.Integer, _    ByVal Config_names As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim Config_opt As System.Integer Dim Config_names As System.Object Dim value As System.Object   value = instance.GetActiveGroundPlane(Config_opt, Config_names) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetActiveGroundPlane(     System.int Config_opt,    System.object Config_names ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetActiveGroundPlane(  &   System.int Config_opt, &   System.Object^ Config_names ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Config\_opt*
:   Configurations from which to retrieve active ground planes as defined in swInConfigurationOpts\_e:

    * swThisConfiguration* swAllConfigurations* swSpecifyConfiguration

    (see **Remarks**)

*Config\_names*
:   Array of the names of configurations from which to retrieve active ground planes; valid only if Config\_opt is set to swInConfiguration\_e.swSpecifyConfiguration (see **Remarks**)

#### Return Value

Array of ground plane [features](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::GetActiveGroundPlane.

# ![](dotnetimages/collapse.gif)Example

[Insert and Activate Ground Plane (VBA)](Insert_Ground_Plane_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

| If Config\_opt is set to swInConfiguration\_e... | Then the returned array contains one active ground plane or null for... |
| --- | --- |
| swAllConfigurations | Each configuration in the assembly. |
| swSpecifyConfiguration | Each configuration in Config\_names. |
| swThisConfiguration | The current configuration. |

To populate config\_names, use [IModelDoc2::GetConfigurationNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetConfigurationNames.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::ActivateGroundPlane Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ActivateGroundPlane.html)

[IFeatureManager::InsertGroundPlane Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertGroundPlane.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0
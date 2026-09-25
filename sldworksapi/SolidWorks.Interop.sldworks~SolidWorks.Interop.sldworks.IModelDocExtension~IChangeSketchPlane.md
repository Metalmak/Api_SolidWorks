<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IChangeSketchPlane.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IChangeSketchPlane Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : IChangeSketchPlane Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Config\_opt*
:   Configurations as defined by swInConfigurationOpts\_e

*Config\_count*
:   Number of configurations

*Config\_names*
:   Array of configuration names

Changes the plane used by a sketch by moving the selected sketch to the selected plane in the specified configurations.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IChangeSketchPlane( _    ByVal Config_opt As System.Integer, _    ByVal Config_count As System.Integer, _    ByRef Config_names As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Config_opt As System.Integer Dim Config_count As System.Integer Dim Config_names As System.String Dim value As System.Boolean   value = instance.IChangeSketchPlane(Config_opt, Config_count, Config_names) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IChangeSketchPlane(     System.int Config_opt,    System.int Config_count,    ref System.string Config_names ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IChangeSketchPlane(  &   System.int Config_opt, &   System.int Config_count, &   System.String^% Config_names ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Config\_opt*
:   Configurations as defined by swInConfigurationOpts\_e

*Config\_count*
:   Number of configurations

*Config\_names*
:   Array of configuration names

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::IChangeSketchPlane.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::ChangeSketchPlane Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ChangeSketchPlane.html)
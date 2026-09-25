<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ISetComponentVisibility.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISetComponentVisibility Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : ISetComponentVisibility Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Visibility*
:   True to show the selected component, false to hide it

*Config\_opt*
:   Configuration option as defined in swInConfigurationOpts\_e

*Config\_count*
:   Number of configurations for the component

*Config\_names*
:   Array of the names of the configurations for the component

Hides or shows the selected component in the specified configurations in this assembly document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ISetComponentVisibility( _    ByVal Visibility As System.Boolean, _    ByVal Config_opt As System.Integer, _    ByVal Config_count As System.Integer, _    ByRef Config_names As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim Visibility As System.Boolean Dim Config_opt As System.Integer Dim Config_count As System.Integer Dim Config_names As System.String   instance.ISetComponentVisibility(Visibility, Config_opt, Config_count, Config_names) ``` | |

| C# |  |
| --- | --- |
| ``` void ISetComponentVisibility(     System.bool Visibility,    System.int Config_opt,    System.int Config_count,    ref System.string Config_names ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ISetComponentVisibility(  &   System.bool Visibility, &   System.int Config_opt, &   System.int Config_count, &   System.String^% Config_names ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Visibility*
:   True to show the selected component, false to hide it

*Config\_opt*
:   Configuration option as defined in swInConfigurationOpts\_e

*Config\_count*
:   Number of configurations for the component

*Config\_names*
:   Array of the names of the configurations for the component

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::ISetComponentVisibility.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IComponent2::GetVisibility Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetVisibility.html)

[IComponent2::ISetVisibility Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~ISetVisibility.html)

[IComponent2::Visible Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Visible.html)

[IComponent2::SetVisibility Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetVisibility.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12
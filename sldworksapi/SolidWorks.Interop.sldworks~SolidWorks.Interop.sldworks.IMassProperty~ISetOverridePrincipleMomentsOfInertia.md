<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~ISetOverridePrincipleMomentsOfInertia.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISetOverridePrincipleMomentsOfInertia Method (IMassProperty) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMassProperty Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty.html) : ISetOverridePrincipleMomentsOfInertia Method (IMassProperty) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Value*
:   * in-process, unmanaged C++: Pointer to an array of three doubles of the principal moments of inertia: **[** Px, Py, Pz **]*** VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*Config\_option*
:   Configuration option as defined in swInConfigurationOpts\_e

*Config\_numbers*
:   Number of configurations

*Config\_names*
:   * in-process, unmanaged C++: Pointer to an array of configuration names of size Config\_numbers; valid only if Config\_option = swInConfigurationOpts\_e.swSpecifyConfiguration* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Overrides the principal moments of inertia of the model currently being edited in this part or assembly document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ISetOverridePrincipleMomentsOfInertia( _    ByRef Value As System.Double, _    ByVal Config_option As System.Integer, _    ByVal Config_numbers As System.Integer, _    ByRef Config_names As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMassProperty Dim Value As System.Double Dim Config_option As System.Integer Dim Config_numbers As System.Integer Dim Config_names As System.String Dim value As System.Boolean   value = instance.ISetOverridePrincipleMomentsOfInertia(Value, Config_option, Config_numbers, Config_names) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ISetOverridePrincipleMomentsOfInertia(     ref System.double Value,    System.int Config_option,    System.int Config_numbers,    ref System.string Config_names ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ISetOverridePrincipleMomentsOfInertia(  &   System.double% Value, &   System.int Config_option, &   System.int Config_numbers, &   System.String^% Config_names ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Value*
:   * in-process, unmanaged C++: Pointer to an array of three doubles of the principal moments of inertia: **[** Px, Py, Pz **]*** VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*Config\_option*
:   Configuration option as defined in swInConfigurationOpts\_e

*Config\_numbers*
:   Number of configurations

*Config\_names*
:   * in-process, unmanaged C++: Pointer to an array of configuration names of size Config\_numbers; valid only if Config\_option = swInConfigurationOpts\_e.swSpecifyConfiguration* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)See Also

####

[IMassProperty Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty.html)

[IMassProperty Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty_members.html)

[IMassProperty::SetOverridePrincipleMomentsOfInertia Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~SetOverridePrincipleMomentsOfInertia.html)

[IMassProperty::OverrideMomentsOfInertia Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~OverrideMomentsOfInertia.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0
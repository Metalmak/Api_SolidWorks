<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~ISetOverrideMassValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISetOverrideMassValue Method (IMassProperty) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMassProperty Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty.html) : ISetOverrideMassValue Method (IMassProperty) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Value*
:   Override mass value (see **Remarks**)

*Config\_option*
:   Configuration option as defined in swInConfigurationOpts\_e

*Config\_numbers*
:   Number of configurations

*Config\_names*
:   * in-process, unmanaged C++: Pointer to an array of configuration names of size Config\_numbers (see **Remarks**)* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Overrides the mass of the model currently being edited in this part or assembly document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ISetOverrideMassValue( _    ByVal Value As System.Double, _    ByVal Config_option As System.Integer, _    ByVal Config_numbers As System.Integer, _    ByRef Config_names As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMassProperty Dim Value As System.Double Dim Config_option As System.Integer Dim Config_numbers As System.Integer Dim Config_names As System.String Dim value As System.Boolean   value = instance.ISetOverrideMassValue(Value, Config_option, Config_numbers, Config_names) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ISetOverrideMassValue(     System.double Value,    System.int Config_option,    System.int Config_numbers,    ref System.string Config_names ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ISetOverrideMassValue(  &   System.double Value, &   System.int Config_option, &   System.int Config_numbers, &   System.String^% Config_names ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Value*
:   Override mass value (see **Remarks**)

*Config\_option*
:   Configuration option as defined in swInConfigurationOpts\_e

*Config\_numbers*
:   Number of configurations

*Config\_names*
:   * in-process, unmanaged C++: Pointer to an array of configuration names of size Config\_numbers (see **Remarks**)* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

#### Return Value

True if the mass value is overridden, false if not

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| If... | Then... |
| You are editing a subcomponent | you are overriding the mass for this subcomponent and not for the top-level model. |
| Value > 0  Value < 0 | mass is overridden.  mass is calculated. |
| Config\_option = swInConfigurationOpts\_e.swSpecifyConfiguration | Config\_names is used. |

# ![](dotnetimages/collapse.gif)See Also

####

[IMassProperty Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty.html)

[IMassProperty Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty_members.html)

[IMassProperty::SetOverrideMassValue Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~SetOverrideMassValue.html)

[IMassProperty::OverrideMass Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~OverrideMass.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0
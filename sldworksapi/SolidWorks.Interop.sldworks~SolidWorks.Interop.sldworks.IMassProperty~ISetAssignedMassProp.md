<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~ISetAssignedMassProp.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISetAssignedMassProp Method (IMassProperty) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMassProperty Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty.html) : ISetAssignedMassProp Method (IMassProperty) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Mass*
:   Value for mass

*Center\_x*
:   x coordinate for center of gravity

*Center\_y*
:   y coordinate for center of gravity

*Center\_z*
:   z coordinate for center of gravity

*Config\_opt*
:   Configuration options as defined in swInConfigurationOpts\_e

*ConfigNum*
:   Number of configurations

*Config\_names*
:   * in-process, unmanaged C++: Pointer to an array of configuration names of size ConfigNum* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Sets the mass and center of gravity for the specified configurations for this model being edited in this part or assembly document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ISetAssignedMassProp( _    ByVal Mass As System.Double, _    ByVal Center_x As System.Double, _    ByVal Center_y As System.Double, _    ByVal Center_z As System.Double, _    ByVal Config_opt As System.Integer, _    ByVal ConfigNum As System.Integer, _    ByRef Config_names As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMassProperty Dim Mass As System.Double Dim Center_x As System.Double Dim Center_y As System.Double Dim Center_z As System.Double Dim Config_opt As System.Integer Dim ConfigNum As System.Integer Dim Config_names As System.String Dim value As System.Boolean   value = instance.ISetAssignedMassProp(Mass, Center_x, Center_y, Center_z, Config_opt, ConfigNum, Config_names) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ISetAssignedMassProp(     System.double Mass,    System.double Center_x,    System.double Center_y,    System.double Center_z,    System.int Config_opt,    System.int ConfigNum,    ref System.string Config_names ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ISetAssignedMassProp(  &   System.double Mass, &   System.double Center_x, &   System.double Center_y, &   System.double Center_z, &   System.int Config_opt, &   System.int ConfigNum, &   System.String^% Config_names ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Mass*
:   Value for mass

*Center\_x*
:   x coordinate for center of gravity

*Center\_y*
:   y coordinate for center of gravity

*Center\_z*
:   z coordinate for center of gravity

*Config\_opt*
:   Configuration options as defined in swInConfigurationOpts\_e

*ConfigNum*
:   Number of configurations

*Config\_names*
:   * in-process, unmanaged C++: Pointer to an array of configuration names of size ConfigNum* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

#### Return Value

True if the mass and center of gravity are set, false if not

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| If... | Then... |
| You are editing a subcomponent | you are setting the mass for this subcomponent and not for the top-level model. |
| You specify a value < 0 for mass | mass is calculated; it is not user-defined. |
| Config\_opt is set to swSpecifyConfiguration | Config\_names is used. |

# ![](dotnetimages/collapse.gif)See Also

####

[IMassProperty Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty.html)

[IMassProperty Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty_members.html)

[IMassProperty::SetAssignedMassProp Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~SetAssignedMassProp.html)

[IMassProperty::IGetCenterOfMass Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~IGetCenterOfMass.html)

[IMassProperty::CenterOfMass Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~CenterOfMass.html)

[IMassProperty::Mass Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~Mass.html)

[IMassProperty::UserAssigned Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~UserAssigned.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0
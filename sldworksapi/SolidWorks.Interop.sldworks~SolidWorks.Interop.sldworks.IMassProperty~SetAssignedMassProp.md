<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~SetAssignedMassProp.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetAssignedMassProp Method (IMassProperty) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMassProperty Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty.html) : SetAssignedMassProp Method (IMassProperty) |

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

*Config\_names*
:   Array of the configuration names

Sets the mass and center of gravity for the specified configurations for this model being edited in this part or assembly document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetAssignedMassProp( _    ByVal Mass As System.Double, _    ByVal Center_x As System.Double, _    ByVal Center_y As System.Double, _    ByVal Center_z As System.Double, _    ByVal Config_opt As System.Integer, _    ByVal Config_names As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMassProperty Dim Mass As System.Double Dim Center_x As System.Double Dim Center_y As System.Double Dim Center_z As System.Double Dim Config_opt As System.Integer Dim Config_names As System.Object Dim value As System.Boolean   value = instance.SetAssignedMassProp(Mass, Center_x, Center_y, Center_z, Config_opt, Config_names) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetAssignedMassProp(     System.double Mass,    System.double Center_x,    System.double Center_y,    System.double Center_z,    System.int Config_opt,    System.object Config_names ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetAssignedMassProp(  &   System.double Mass, &   System.double Center_x, &   System.double Center_y, &   System.double Center_z, &   System.int Config_opt, &   System.Object^ Config_names ) ``` | |

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

*Config\_names*
:   Array of the configuration names

#### Return Value

True if the mass and center of gravity are set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MassProperty::SetAssignedMassProp.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| If... | Then... |
| You are editing a subcomponent | you are setting the mass for this subcomponent and not for the top-level model. |
| You specify a value < 0 for Mass | mass is calculated; it is not user-defined. |
| Config\_opt is set to swSpecifyConfiguration | Config\_names is used. |

# ![](dotnetimages/collapse.gif)See Also

####

[IMassProperty Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty.html)

[IMassProperty Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty_members.html)

[IMassProperty::ISetAssignedMassProp Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~ISetAssignedMassProp.html)

[IMassProperty::Mass Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~Mass.html)

[IMassProperty::UserAssigned Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~UserAssigned.html)

[IMassProperty::IGetCenterOfMass Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~IGetCenterOfMass.html)

[IMassProperty::CenterOfMass Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~CenterOfMass.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0
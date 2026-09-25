<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~SetOverrideMomentsOfInertiaValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetOverrideMomentsOfInertiaValue Method (IMassProperty) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMassProperty Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty.html) : SetOverrideMomentsOfInertiaValue Method (IMassProperty) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ReferenceFrame*
:   Frame of reference as defined in swMomentsOfInertiaReferenceFrame\_e

*CoordinateSystemName*
:   Name of coordinate system; valid only if ReferenceFrame = swMomentsOfInertiaReferenceFrame\_e.swMomentsOfInertiaReferenceFrame\_UserCoordinateSystem

*Value*
:   Array of nine doubles: [ Lxx, Lxy, Lxz, Lyx, Lyy, Lyz, Lzx, Lzy, Lzz ]

*Config\_option*
:   Configuration option as defined in swInConfigurationOpts\_e

*Config\_names*
:   Array of configuration names; valid only if Config\_option = swInConfigurationOpts\_e.swSpecifyConfiguration

Overrides the moments of inertia of the model currently being edited in this part or assembly document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetOverrideMomentsOfInertiaValue( _    ByVal ReferenceFrame As System.Integer, _    ByVal CoordinateSystemName As System.String, _    ByVal Value As System.Object, _    ByVal Config_option As System.Integer, _    ByVal Config_names As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMassProperty Dim ReferenceFrame As System.Integer Dim CoordinateSystemName As System.String Dim Value As System.Object Dim Config_option As System.Integer Dim Config_names As System.Object Dim value As System.Boolean   value = instance.SetOverrideMomentsOfInertiaValue(ReferenceFrame, CoordinateSystemName, Value, Config_option, Config_names) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetOverrideMomentsOfInertiaValue(     System.int ReferenceFrame,    System.string CoordinateSystemName,    System.object Value,    System.int Config_option,    System.object Config_names ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetOverrideMomentsOfInertiaValue(  &   System.int ReferenceFrame, &   System.String^ CoordinateSystemName, &   System.Object^ Value, &   System.int Config_option, &   System.Object^ Config_names ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ReferenceFrame*
:   Frame of reference as defined in swMomentsOfInertiaReferenceFrame\_e

*CoordinateSystemName*
:   Name of coordinate system; valid only if ReferenceFrame = swMomentsOfInertiaReferenceFrame\_e.swMomentsOfInertiaReferenceFrame\_UserCoordinateSystem

*Value*
:   Array of nine doubles: [ Lxx, Lxy, Lxz, Lyx, Lyy, Lyz, Lzx, Lzy, Lzz ]

*Config\_option*
:   Configuration option as defined in swInConfigurationOpts\_e

*Config\_names*
:   Array of configuration names; valid only if Config\_option = swInConfigurationOpts\_e.swSpecifyConfiguration

#### Return Value

True if the moments of inertia are overridden, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MassProperty::SetOverrideMomentsOfInertiaValue.

# ![](dotnetimages/collapse.gif)Example

[Get and Override Mass Properties (VBA)](Get_Mass_Properties_using_MassProperty_Object_Example_VB.htm)

[Get and Override Mass Properties (VB.NET)](Get_Mass_Properties_Using_IMassProperty_Example_VBNET.htm)

[Get and Override Mass Properties (C#)](Get_Mass_Properties_Using_IMassProperty_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IMassProperty Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty.html)

[IMassProperty Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty_members.html)

[IMassProperty::ISetOverrideMomentsOfInertiaValue Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~ISetOverrideMomentsOfInertiaValue.html)

[IMassProperty::OverrideMomentsOfInertia Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty~OverrideMomentsOfInertia.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0
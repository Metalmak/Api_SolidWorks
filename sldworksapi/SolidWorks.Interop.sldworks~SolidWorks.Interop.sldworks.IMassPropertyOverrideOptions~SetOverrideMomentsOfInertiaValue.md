<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions~SetOverrideMomentsOfInertiaValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetOverrideMomentsOfInertiaValue Method (IMassPropertyOverrideOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMassPropertyOverrideOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions.html) : SetOverrideMomentsOfInertiaValue Method (IMassPropertyOverrideOptions) |

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

*Value*
:   Array of nine doubles: [ Lxx, Lxy, Lxz, Lyx, Lyy, Lyz, Lzx, Lzy, Lzz ]

*CoordinateSystemName*
:   Name of coordinate system; valid only if ReferenceFrame = swMomentsOfInertiaReferenceFrame\_e.swMomentsOfInertiaReferenceFrame\_UserCoordinateSystem

Overrides the calculated moments of inertia of the model currently being edited.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetOverrideMomentsOfInertiaValue( _    ByVal ReferenceFrame As System.Integer, _    ByVal Value As System.Object, _    ByVal CoordinateSystemName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMassPropertyOverrideOptions Dim ReferenceFrame As System.Integer Dim Value As System.Object Dim CoordinateSystemName As System.String Dim value As System.Boolean   value = instance.SetOverrideMomentsOfInertiaValue(ReferenceFrame, Value, CoordinateSystemName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetOverrideMomentsOfInertiaValue(     System.int ReferenceFrame,    System.object Value,    System.string CoordinateSystemName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetOverrideMomentsOfInertiaValue(  &   System.int ReferenceFrame, &   System.Object^ Value, &   System.String^ CoordinateSystemName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ReferenceFrame*
:   Frame of reference as defined in swMomentsOfInertiaReferenceFrame\_e

*Value*
:   Array of nine doubles: [ Lxx, Lxy, Lxz, Lyx, Lyy, Lyz, Lzx, Lzy, Lzz ]

*CoordinateSystemName*
:   Name of coordinate system; valid only if ReferenceFrame = swMomentsOfInertiaReferenceFrame\_e.swMomentsOfInertiaReferenceFrame\_UserCoordinateSystem

#### Return Value

True if the moments of inertia are successfully overridden, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MassPropertyOverrideOptions::SetOverrideMomentsOfInertiaValue.

# ![](dotnetimages/collapse.gif)Example

See the [IMassProperty2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty2.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [IMassPropertyOverrideOptions::OverrideMomentsOfInertia](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions~OverrideMomentsOfInertia.html) is set to true.

# ![](dotnetimages/collapse.gif)See Also

####

[IMassPropertyOverrideOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions.html)

[IMassPropertyOverrideOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions_members.html)

[IMassProperty2::GetMomentOfInertia Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty2~GetMomentOfInertia.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0
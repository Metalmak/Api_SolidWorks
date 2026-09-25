<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions~GetOverrideMomentsOfInertiaValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetOverrideMomentsOfInertiaValue Method (IMassPropertyOverrideOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMassPropertyOverrideOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions.html) : GetOverrideMomentsOfInertiaValue Method (IMassPropertyOverrideOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IsReferenceFrameSet*
:   True if reference frame is set, false if not

*CoordinateSystemName*
:   Name of coordinate system

Gets the override moments of inertia.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetOverrideMomentsOfInertiaValue( _    ByRef IsReferenceFrameSet As System.Boolean, _    ByRef CoordinateSystemName As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMassPropertyOverrideOptions Dim IsReferenceFrameSet As System.Boolean Dim CoordinateSystemName As System.String Dim value As System.Object   value = instance.GetOverrideMomentsOfInertiaValue(IsReferenceFrameSet, CoordinateSystemName) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetOverrideMomentsOfInertiaValue(     out System.bool IsReferenceFrameSet,    out System.string CoordinateSystemName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetOverrideMomentsOfInertiaValue(  &   [Out] System.bool IsReferenceFrameSet, &   [Out] System.String^ CoordinateSystemName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IsReferenceFrameSet*
:   True if reference frame is set, false if not

*CoordinateSystemName*
:   Name of coordinate system

#### Return Value

Array of nine doubles: [ Lxx, Lxy, Lxz, Lyx, Lyy, Lyz, Lzx, Lzy, Lzz ]

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MassPropertyOverrideOptions::GetOverrideMomentsOfInertiaValue.

# ![](dotnetimages/collapse.gif)See Also

####

[IMassPropertyOverrideOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions.html)

[IMassPropertyOverrideOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions_members.html)

[IMassPropertyOverrideOptions::SetOverrideMomentsOfInertiaValue Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions~SetOverrideMomentsOfInertiaValue.html)

[IMassPropertyOverrideOptions::OverrideMomentsOfInertia Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions~OverrideMomentsOfInertia.html)

[IMassProperty2::GetMomentOfInertia Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty2~GetMomentOfInertia.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0
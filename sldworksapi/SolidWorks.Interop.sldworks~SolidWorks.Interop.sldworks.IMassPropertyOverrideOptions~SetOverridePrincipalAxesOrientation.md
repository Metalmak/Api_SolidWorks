<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions~SetOverridePrincipalAxesOrientation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetOverridePrincipalAxesOrientation Method (IMassPropertyOverrideOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMassPropertyOverrideOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions.html) : SetOverridePrincipalAxesOrientation Method (IMassPropertyOverrideOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Axis*
:   One of the following principal axes:

    * 0 = X axis* 1 = Y axis* 2 = Z axis

*Value*
:   An array of three doubles of the x, y, and z coordinates of Axis

*AutoCorrect*
:   True to generate orthogonal axes, false to not

Overrides the orientation of the specified principal axis of inertia of the model currently being edited.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetOverridePrincipalAxesOrientation( _    ByVal Axis As System.Integer, _    ByVal Value As System.Object, _    ByVal AutoCorrect As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMassPropertyOverrideOptions Dim Axis As System.Integer Dim Value As System.Object Dim AutoCorrect As System.Boolean Dim value As System.Boolean   value = instance.SetOverridePrincipalAxesOrientation(Axis, Value, AutoCorrect) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetOverridePrincipalAxesOrientation(     System.int Axis,    System.object Value,    System.bool AutoCorrect ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetOverridePrincipalAxesOrientation(  &   System.int Axis, &   System.Object^ Value, &   System.bool AutoCorrect ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Axis*
:   One of the following principal axes:

    * 0 = X axis* 1 = Y axis* 2 = Z axis

*Value*
:   An array of three doubles of the x, y, and z coordinates of Axis

*AutoCorrect*
:   True to generate orthogonal axes, false to not

#### Return Value

True if the principal axis orientation successfully overridden, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MassPropertyOverrideOptions::SetOverridePrincipalAxesOrientation.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [IMassPropertyOverrideOptions::OverrideMomentsOfInertia](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions~OverrideMomentsOfInertia.html) is set to true.

# ![](dotnetimages/collapse.gif)See Also

####

[IMassPropertyOverrideOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions.html)

[IMassPropertyOverrideOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions_members.html)

[IMassProperty2::PrincipalAxesOfInertia Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty2~PrincipalAxesOfInertia.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0
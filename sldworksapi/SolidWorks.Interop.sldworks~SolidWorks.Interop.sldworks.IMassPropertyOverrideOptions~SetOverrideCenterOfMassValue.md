<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions~SetOverrideCenterOfMassValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetOverrideCenterOfMassValue Method (IMassPropertyOverrideOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMassPropertyOverrideOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions.html) : SetOverrideCenterOfMassValue Method (IMassPropertyOverrideOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Value*
:   Array of three doubles of the x, y, and z coordinates of the center of mass

*CoordinateSystemName*
:   Name of the coordinate system in which the center of mass is defined

Overrides the calculated center of mass of the model currently being edited.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetOverrideCenterOfMassValue( _    ByVal Value As System.Object, _    ByVal CoordinateSystemName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMassPropertyOverrideOptions Dim Value As System.Object Dim CoordinateSystemName As System.String Dim value As System.Boolean   value = instance.SetOverrideCenterOfMassValue(Value, CoordinateSystemName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetOverrideCenterOfMassValue(     System.object Value,    System.string CoordinateSystemName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetOverrideCenterOfMassValue(  &   System.Object^ Value, &   System.String^ CoordinateSystemName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Value*
:   Array of three doubles of the x, y, and z coordinates of the center of mass

*CoordinateSystemName*
:   Name of the coordinate system in which the center of mass is defined

#### Return Value

True if the center of mass is successfully overridden, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MassPropertyOverrideOptions::SetOverrideCenterOfMassValue.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [IMassPropertyOverrideOptions::OverrideCenterOfMass](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions~OverrideCenterOfMass.html) is set to true.

# ![](dotnetimages/collapse.gif)See Also

####

[IMassPropertyOverrideOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions.html)

[IMassPropertyOverrideOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassPropertyOverrideOptions_members.html)

[IMassProperty2::CenterOfMass Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMassProperty2~CenterOfMass.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0
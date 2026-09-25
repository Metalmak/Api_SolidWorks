<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetValues Method (ICWDynamicInitialCondition) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicInitialCondition Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition.html) : SetValues Method (ICWDynamicInitialCondition) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DVal1*
:   Value along direction 1 (if direction reference is a face or plane) or along a radial direction (if direction reference is a cylindrical face or axis); valid only if BDir1 = 1 in [ICWDynamicInitialCondition::GetDirections](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicInitialCondition~GetDirections.html)

*DVal2*
:   Value along direction 2 (if direction reference is a face or plane) or along a circumferential direction (if direction reference is a cylindrical face or axis); valid only if BDir2 = 1 in ICWDynamicInitialCondition::GetDirections

*DVal3*
:   Value along the normal to the plane (if direction reference is a face or plane), or along an axial direction (if direction reference is a cylindrical face or axis), or along an edge (if direction reference is an edge); valid only if BDir3 = 1 in ICWDynamicInitialCondition::GetDirections

Sets the values in each direction.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetValues( _    ByVal DVal1 As System.Double, _    ByVal DVal2 As System.Double, _    ByVal DVal3 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicInitialCondition Dim DVal1 As System.Double Dim DVal2 As System.Double Dim DVal3 As System.Double   instance.SetValues(DVal1, DVal2, DVal3) ``` | |

| C# |  |
| --- | --- |
| ``` void SetValues(     System.double DVal1,    System.double DVal2,    System.double DVal3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetValues(  &   System.double DVal1, &   System.double DVal2, &   System.double DVal3 ) ``` | |

#### Parameters

*DVal1*
:   Value along direction 1 (if direction reference is a face or plane) or along a radial direction (if direction reference is a cylindrical face or axis); valid only if BDir1 = 1 in [ICWDynamicInitialCondition::GetDirections](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicInitialCondition~GetDirections.html)

*DVal2*
:   Value along direction 2 (if direction reference is a face or plane) or along a circumferential direction (if direction reference is a cylindrical face or axis); valid only if BDir2 = 1 in ICWDynamicInitialCondition::GetDirections

*DVal3*
:   Value along the normal to the plane (if direction reference is a face or plane), or along an axial direction (if direction reference is a cylindrical face or axis), or along an edge (if direction reference is an edge); valid only if BDir3 = 1 in ICWDynamicInitialCondition::GetDirections

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDynamicInitialCondition::SetValues.

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWDynamicInitialCondition::SetDirectionEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetDirectionEntity.html) to set the direction reference for this initial condition.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicInitialCondition Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition.html)

[ICWDynamicInitialCondition Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition_members.html)

[ICWDynamicInitialCondition::GetValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0
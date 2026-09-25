<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetDirections.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetDirections Method (ICWDynamicInitialCondition) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicInitialCondition Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition.html) : GetDirections Method (ICWDynamicInitialCondition) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BDir1*
:   1 if initial condition is applied along direction 1 (if direction reference is a plane or face) or in a radial direction (if direction reference is a cylindrical face or axis), 0 if not (see **Remarks**)

*BDir2*
:   1 if initial condition is applied along direction 2 (if direction reference is a plane or face) or in a circumferential direction (if direction reference is a cylindrical face or axis), 0 if not (see **Remarks**)

*BDir3*
:   1 if initial condition is applied along the normal (if direction reference is a plane or face), or in an axial direction (if direction reference is a cylindrical face or axis), or along an edge (if direction reference is an edge); 0 if not (see **Remarks**)

Obsolete. Superseded by [ICWDynamicInitialCondition::GetDirections2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetDirections2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetDirections( _    ByRef BDir1 As System.Integer, _    ByRef BDir2 As System.Integer, _    ByRef BDir3 As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicInitialCondition Dim BDir1 As System.Integer Dim BDir2 As System.Integer Dim BDir3 As System.Integer   instance.GetDirections(BDir1, BDir2, BDir3) ``` | |

| C# |  |
| --- | --- |
| ``` void GetDirections(     out System.int BDir1,    out System.int BDir2,    out System.int BDir3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetDirections(  &   [Out] System.int BDir1, &   [Out] System.int BDir2, &   [Out] System.int BDir3 ) ``` | |

#### Parameters

*BDir1*
:   1 if initial condition is applied along direction 1 (if direction reference is a plane or face) or in a radial direction (if direction reference is a cylindrical face or axis), 0 if not (see **Remarks**)

*BDir2*
:   1 if initial condition is applied along direction 2 (if direction reference is a plane or face) or in a circumferential direction (if direction reference is a cylindrical face or axis), 0 if not (see **Remarks**)

*BDir3*
:   1 if initial condition is applied along the normal (if direction reference is a plane or face), or in an axial direction (if direction reference is a cylindrical face or axis), or along an edge (if direction reference is an edge); 0 if not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDynamicInitialCondition::GetDirections.

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWDynamicInitialCondition::SetDirectionEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetDirectionEntity.html) to set the direction reference for this initial condition.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicInitialCondition Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition.html)

[ICWDynamicInitialCondition Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition_members.html)

[ICWDynamicInitialCondition::SetDirections Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~SetDirections.html)

[ICWDynamicInitialCondition::GetReverseDirections Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetReverseDirections.html)

[ICWDynamicInitialCondition::GetValues Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicInitialCondition~GetValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0
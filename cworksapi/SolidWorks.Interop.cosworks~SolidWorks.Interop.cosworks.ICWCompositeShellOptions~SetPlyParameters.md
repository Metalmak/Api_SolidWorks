<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~SetPlyParameters.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetPlyParameters Method (ICWCompositeShellOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWCompositeShellOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions.html) : SetPlyParameters Method (ICWCompositeShellOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NPly*
:   Index of ply (see **Remarks**)

*DThickness*
:   Thickness of ply

*DAngle*
:   Angle of ply (see **Remarks**)

*PMaterial*
:   [ICWMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

Obsolete. Superseded by [ICWCompositeShellOptions::SetPlyParameters2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~SetPlyParameters2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPlyParameters( _    ByVal NPly As System.Integer, _    ByVal DThickness As System.Double, _    ByVal DAngle As System.Double, _    ByVal PMaterial As CWMaterial _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWCompositeShellOptions Dim NPly As System.Integer Dim DThickness As System.Double Dim DAngle As System.Double Dim PMaterial As CWMaterial Dim value As System.Integer   value = instance.SetPlyParameters(NPly, DThickness, DAngle, PMaterial) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetPlyParameters(     System.int NPly,    System.double DThickness,    System.double DAngle,    CWMaterial PMaterial ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetPlyParameters(  &   System.int NPly, &   System.double DThickness, &   System.double DAngle, &   CWMaterial^ PMaterial ) ``` | |

#### Parameters

*NPly*
:   Index of ply (see **Remarks**)

*DThickness*
:   Thickness of ply

*DAngle*
:   Angle of ply (see **Remarks**)

*PMaterial*
:   [ICWMaterial](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

#### Return Value

Error code as defined in [swsCompositeShellOptionsError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCompositeShellOptionsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWCompositeShellOptions::SetPlyParameters.

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWCompositeShellOptions::GetTotalPlies](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~GetTotalPlies.html) to set NPly.

| If [ICWCompositeShellOptions::PlyRelativeAngle](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~PlyRelativeAngle.html) is set to... | Then DAngle's value is... |
| --- | --- |
| 1 | Relative to the angle of ply 1 |
| 0 | Absolute |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWCompositeShellOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions.html)

[ICWCompositeShellOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions_members.html)

[ICWCompositeShellOptions::GetPlyParameters Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~GetPlyParameters.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP3
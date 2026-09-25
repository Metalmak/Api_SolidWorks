<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetStressStrainCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetStressStrainCurve Method (ICWMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html) : SetStressStrainCurve Method (ICWMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VarCurveData*
:   Array of stress-strain curve data

*ErrorCode*
:   Error as defined in [swsMaterialStressStrainCurveError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMaterialStressStrainCurveError_e.html)

Sets the stress-strain curve data.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetStressStrainCurve( _    ByVal VarCurveData As System.Object, _    ByRef ErrorCode As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMaterial Dim VarCurveData As System.Object Dim ErrorCode As System.Integer   instance.SetStressStrainCurve(VarCurveData, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` void SetStressStrainCurve(     System.object VarCurveData,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetStressStrainCurve(  &   System.Object^ VarCurveData, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*VarCurveData*
:   Array of stress-strain curve data

*ErrorCode*
:   Error as defined in [swsMaterialStressStrainCurveError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMaterialStressStrainCurveError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMaterial::SetStressStrainCurve.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

[ICWMaterial Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial_members.html)

[ICWMaterial::GetStressStrainCurve Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetStressStrainCurve.html)
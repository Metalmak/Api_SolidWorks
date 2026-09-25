<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetFatigueSNCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetFatigueSNCurve Method (ICWMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html) : SetFatigueSNCurve Method (ICWMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NIndex*
:   0-based S-N curve data index

*DStressRatio*
:   Stress ratio

*VarFatigueSNCurveData*
:   Array of S-N curve data (see Remarks)

*ErrorCode*
:   Error as defined in [swsMaterialFatigueSNCurveError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMaterialSNCurveSource_e.html)

Sets the fatigue S-N curve data for user-defined curve sources.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetFatigueSNCurve( _    ByVal NIndex As System.Integer, _    ByVal DStressRatio As System.Double, _    ByVal VarFatigueSNCurveData As System.Object, _    ByRef ErrorCode As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMaterial Dim NIndex As System.Integer Dim DStressRatio As System.Double Dim VarFatigueSNCurveData As System.Object Dim ErrorCode As System.Integer   instance.SetFatigueSNCurve(NIndex, DStressRatio, VarFatigueSNCurveData, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFatigueSNCurve(     System.int NIndex,    System.double DStressRatio,    System.object VarFatigueSNCurveData,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFatigueSNCurve(  &   System.int NIndex, &   System.double DStressRatio, &   System.Object^ VarFatigueSNCurveData, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NIndex*
:   0-based S-N curve data index

*DStressRatio*
:   Stress ratio

*VarFatigueSNCurveData*
:   Array of S-N curve data (see Remarks)

*ErrorCode*
:   Error as defined in [swsMaterialFatigueSNCurveError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMaterialSNCurveSource_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMaterial::SetFatigueSNCurve.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWMaterial::SNCurveSource](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SNCurveSource.html) is set to [swsMaterialSNCurveSource\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMaterialSNCurveSource_e.html).swsMaterialSNCurveSourceUserDefined.

VarFatigueSNCurveData:

> **[** *n, x1, y1, x2, y2, x3, y3,...xn, yn* **]**

where:

* n = number of xi,yi pairs

  * x1 = number of cycles for point 1

    * y1 = alternating stress for point 1

      * ...

        * xn = number of cycles for point n

          * yn = alternating stress for point n

See the SOLIDWORKS Help topic, **Material Dialog Box - Fatigue SN Curves Tab**, for more information about S-N curve equations.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

[ICWMaterial Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial_members.html)

[ICWMaterial::GetFatigueSNCurve Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetFatigueSNCurve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0
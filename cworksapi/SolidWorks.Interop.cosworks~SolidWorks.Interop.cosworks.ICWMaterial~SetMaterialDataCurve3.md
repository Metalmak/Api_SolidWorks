<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetMaterialDataCurve3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetMaterialDataCurve3 Method (ICWMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html) : SetMaterialDataCurve3 Method (ICWMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NIndex*
:   0-based index of material data curve

*BUseCurve*
:   * -1 or true = Use material data curve* 0 or false = Do not use material data curve

*VarCurveData*
:   Array of material curve data (see Remarks)

*ErrorCode*
:   Error as defined in [swsMaterialDataCurveError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMaterialDataCurveError_e.html)

Sets the material data curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetMaterialDataCurve3( _    ByVal NIndex As System.Integer, _    ByVal BUseCurve As System.Boolean, _    ByVal VarCurveData As System.Object, _    ByRef ErrorCode As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMaterial Dim NIndex As System.Integer Dim BUseCurve As System.Boolean Dim VarCurveData As System.Object Dim ErrorCode As System.Integer   instance.SetMaterialDataCurve3(NIndex, BUseCurve, VarCurveData, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMaterialDataCurve3(     System.int NIndex,    System.bool BUseCurve,    System.object VarCurveData,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMaterialDataCurve3(  &   System.int NIndex, &   System.bool BUseCurve, &   System.Object^ VarCurveData, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NIndex*
:   0-based index of material data curve

*BUseCurve*
:   * -1 or true = Use material data curve* 0 or false = Do not use material data curve

*VarCurveData*
:   Array of material curve data (see Remarks)

*ErrorCode*
:   Error as defined in [swsMaterialDataCurveError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMaterialDataCurveError_e.html)

# ![](dotnetimages/collapse.gif)Remarks

Array of material curve data:

> **[** *n, x1, y1, x2, y2, x3, y3,...xn, yn* **]**

where:

* n = number of xi,yi pairs

  * x1 = X property value for point 1

    * y1 = Y property value for point 1

      * ...

        * xn = X property value for point n

          * yn = Y property value for point n

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

[ICWMaterial Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30
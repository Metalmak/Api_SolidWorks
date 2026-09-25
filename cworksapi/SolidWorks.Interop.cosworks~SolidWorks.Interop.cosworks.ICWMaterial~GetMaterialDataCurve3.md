<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetMaterialDataCurve3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetMaterialDataCurve3 Method (ICWMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html) : GetMaterialDataCurve3 Method (ICWMaterial) |

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
:   * -1 or true = Uses material data curve* 0 or false = Does not use material data curve

    (see **Remarks**)

Gets the material data curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMaterialDataCurve3( _    ByVal NIndex As System.Integer, _    ByRef BUseCurve As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMaterial Dim NIndex As System.Integer Dim BUseCurve As System.Boolean Dim value As System.Object   value = instance.GetMaterialDataCurve3(NIndex, BUseCurve) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetMaterialDataCurve3(     System.int NIndex,    out System.bool BUseCurve ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetMaterialDataCurve3(  &   System.int NIndex, &   [Out] System.bool BUseCurve ) ``` | |

#### Parameters

*NIndex*
:   0-based index of material data curve

*BUseCurve*
:   * -1 or true = Uses material data curve* 0 or false = Does not use material data curve

    (see **Remarks**)

#### Return Value

Array of material curve data (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMaterial::GetMaterialDataCurve3.

# ![](dotnetimages/collapse.gif)Remarks

This method returns a boolean or integer in out parameter BUseCurve, depending on its prior declaration.

If out parameter BUseCurve is cast as a:

* Boolean, true or false is returned.* Long or integer, -1 (=true) or 0 (=false) is returned.

Array of material curve data:

> **[** *n, x1, y1, x2, y2, x3, y3,...xn, yn* **]**

where:

* n = number of xi,yi pairs

  * x1 = X property value for point 1

    * y1 = Y property value for point 1

      * ...

        * xn = X property value for point n

          * yn = Y property value for point n

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

[ICWMaterial Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2021 SP04
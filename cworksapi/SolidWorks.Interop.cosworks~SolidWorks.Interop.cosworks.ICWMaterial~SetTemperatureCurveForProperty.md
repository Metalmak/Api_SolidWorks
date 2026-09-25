<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetTemperatureCurveForProperty.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetTemperatureCurveForProperty Method (ICWMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html) : SetTemperatureCurveForProperty Method (ICWMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SPropName*
:   Property name

*VarCurveData*
:   Array of temperature data (see Remarks)

*ErrorCode*
:   Error as defined in [swsMaterialTemperatureCurveForPropertyError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMaterialTemperatureCurveForPropertyError_e.html)

Sets the temperature curve data for the material property.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetTemperatureCurveForProperty( _    ByVal SPropName As System.String, _    ByVal VarCurveData As System.Object, _    ByRef ErrorCode As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMaterial Dim SPropName As System.String Dim VarCurveData As System.Object Dim ErrorCode As System.Integer   instance.SetTemperatureCurveForProperty(SPropName, VarCurveData, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` void SetTemperatureCurveForProperty(     System.string SPropName,    System.object VarCurveData,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetTemperatureCurveForProperty(  &   System.String^ SPropName, &   System.Object^ VarCurveData, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*SPropName*
:   Property name

*VarCurveData*
:   Array of temperature data (see Remarks)

*ErrorCode*
:   Error as defined in [swsMaterialTemperatureCurveForPropertyError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMaterialTemperatureCurveForPropertyError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMaterial::SetTemperatureCurveForProperty.

# ![](dotnetimages/collapse.gif)Remarks

Array of temperature data:

> **[** *n, x1, y1, x2, y2, x3, y3,...xn, yn* **]**

where:

* n = number of xi,yi pairs

  * x1 =  temperature value for point 1

    * y1 =  property value for point 1

      * ...

        * xn = temperature value for point n

          * yn = property value for point n

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

[ICWMaterial Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial_members.html)

[ICWMaterial::GetTemperatureCurveForProperty Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetTemperatureCurveForProperty.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0
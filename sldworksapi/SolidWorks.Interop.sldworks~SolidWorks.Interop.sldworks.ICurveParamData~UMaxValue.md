<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurveParamData~UMaxValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| UMaxValue Property (ICurveParamData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurveParamData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurveParamData.html) : UMaxValue Property (ICurveParamData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the maximum U parameter value.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property UMaxValue As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurveParamData Dim value As System.Double   value = instance.UMaxValue ``` | |

| C# |  |
| --- | --- |
| ``` System.double UMaxValue {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double UMaxValue {    System.double get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Maximum U parameter value

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CurveParamData::UMaxValue.

# ![](dotnetimages/collapse.gif)Example

[Get Edge Curve Parameterization (C#)](Get_Edge_Curve_Parameterization_Example_CSharp.htm)

[Get Edge Curve Parameterization (VB.NET)](Get_Edge_Curve_Parameterization_Example_VBNET.htm)

[Get Edge Curve Parameterization (VBA)](Get_Edge_Curve_Parameterization_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The minimum U parameter must always be smaller than the maximum U parameter.

If the curve and edge are in opposite directions ([ICurveParamData::Sense](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurveParamData~Sense.html) returns false) and the minimum U parameter is larger than the maximum U parameter, then the parameters are in negative parameter space. For example, if ICurveParamData::Sense is false, minimum U parameter is 10, and maximum U parameter is 5, then [ICurveParamData::UMinValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICurveParamData~UMinValue.html) = -10 and ICurveParamData::UMaxValue = -5. To normalize the values in positive parameter space, swap the two U parameter values and then negate them, so that the values of the minimum U parameter is 5 and the maximum U parameter is 10.

If the curve is closed and the curve starts and ends at the same point, then ICurveParamData::UMinValue and ICurveParamData::UMaxValue are a period apart.

# ![](dotnetimages/collapse.gif)See Also

####

[ICurveParamData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurveParamData.html)

[ICurveParamData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurveParamData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0
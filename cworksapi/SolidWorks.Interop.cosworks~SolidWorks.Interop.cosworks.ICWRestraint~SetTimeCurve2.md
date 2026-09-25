<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~SetTimeCurve2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetTimeCurve2 Method (ICWRestraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html) : SetTimeCurve2 Method (ICWRestraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VarCurveData*
:   Array of time curve data (see **Remarks**)

*ErrorCode*
:   Error as defined in [swsTimeCurveError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTimeCurveError_e.html)

Sets the time curve data for this restraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetTimeCurve2( _    ByVal VarCurveData As System.Object, _    ByRef ErrorCode As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRestraint Dim VarCurveData As System.Object Dim ErrorCode As System.Integer Dim value As System.Boolean   value = instance.SetTimeCurve2(VarCurveData, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetTimeCurve2(     System.object VarCurveData,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetTimeCurve2(  &   System.Object^ VarCurveData, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*VarCurveData*
:   Array of time curve data (see **Remarks**)

*ErrorCode*
:   Error as defined in [swsTimeCurveError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTimeCurveError_e.html)

#### Return Value

-1 or true if time curve set, 0 or false if not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRestraint::SetTimeCurve2.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for nonlinear studies and if [ICWRestraint::RestraintType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint~RestraintType.html) is not set to:

* [swsRestraintType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRestraintType_e.html).swsRestraintTypeFixed,* swsRestraintType\_e.swsRestraintTypeImmovable, or* swsRestraintType\_e.swsRestraintTypeSymmetric.

This method returns a boolean value that can be cast to an integer: -1 = true, 0 = false.

Array of time curve data:

> **[** *n, x1, y1, x2, y2, x3, y3,...xn, yn* **]**

where:

* n = number of pairs of data points

  * xi = time value at the *ith* data point

    * yi = property value associated with time xi

Time curves are used to specify feature variation with respect to time in transient studies.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRestraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html)

[ICWRestraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2021 SP04
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~SetEquationParameters.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetEquationParameters Method (ISketchSpline) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchSpline Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline.html) : SetEquationParameters Method (ISketchSpline) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*YExpression*
:   Equation for y (see **Remarks**)

*RangeStart*
:   Start value of x (see **Remarks**)

*RangeEnd*
:   End value of x (see **Remarks**)

*IsAngleRange*
:   True if the range and x value represent an angle (in radians), false if not

*RotationAngle*
:   Rotation angle (in radians) for the curve

*XOffset*
:   Offset in x for f(x), where x = 0 (see **Remarks**)

*YOffset*
:   Offset in y for f(x), where x = 0 (see **Remarks**)

*LockStart*
:   True to lock the start point (RangeStart) of the curve, false to not

*LockEnd*
:   True to lock the end point (RangeEnd) of the curve, false to not

Obsolete. Superseded by [ISketchSpline::SetEquationParameters2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSpline~SetEquationParameters2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetEquationParameters( _    ByVal YExpression As System.String, _    ByVal RangeStart As System.Double, _    ByVal RangeEnd As System.Double, _    ByVal IsAngleRange As System.Boolean, _    ByVal RotationAngle As System.Double, _    ByVal XOffset As System.Double, _    ByVal YOffset As System.Double, _    ByVal LockStart As System.Boolean, _    ByVal LockEnd As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchSpline Dim YExpression As System.String Dim RangeStart As System.Double Dim RangeEnd As System.Double Dim IsAngleRange As System.Boolean Dim RotationAngle As System.Double Dim XOffset As System.Double Dim YOffset As System.Double Dim LockStart As System.Boolean Dim LockEnd As System.Boolean Dim value As System.Boolean   value = instance.SetEquationParameters(YExpression, RangeStart, RangeEnd, IsAngleRange, RotationAngle, XOffset, YOffset, LockStart, LockEnd) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetEquationParameters(     System.string YExpression,    System.double RangeStart,    System.double RangeEnd,    System.bool IsAngleRange,    System.double RotationAngle,    System.double XOffset,    System.double YOffset,    System.bool LockStart,    System.bool LockEnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetEquationParameters(  &   System.String^ YExpression, &   System.double RangeStart, &   System.double RangeEnd, &   System.bool IsAngleRange, &   System.double RotationAngle, &   System.double XOffset, &   System.double YOffset, &   System.bool LockStart, &   System.bool LockEnd ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*YExpression*
:   Equation for y (see **Remarks**)

*RangeStart*
:   Start value of x (see **Remarks**)

*RangeEnd*
:   End value of x (see **Remarks**)

*IsAngleRange*
:   True if the range and x value represent an angle (in radians), false if not

*RotationAngle*
:   Rotation angle (in radians) for the curve

*XOffset*
:   Offset in x for f(x), where x = 0 (see **Remarks**)

*YOffset*
:   Offset in y for f(x), where x = 0 (see **Remarks**)

*LockStart*
:   True to lock the start point (RangeStart) of the curve, false to not

*LockEnd*
:   True to lock the end point (RangeEnd) of the curve, false to not

#### Return Value

True if the equation-driven curve's parameters are set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchSpline::SetEquationParameters.

# ![](dotnetimages/collapse.gif)Example

[Create Equation-driven Curve (C#)](Create_Equation-driven_Curve_Example_CSharp.htm)

[Create Equation-driven Curve (VB.NET)](Create_Equation-driven_Curve_Example_VBNET.htm)

[Create Equation-driven Curve (VBA)](Create_Equation-driven_Curve_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

**YExpression:**

  Any function that you can define as a 2D function in the following form:

y-in-the-sketch = f(x-in-the-sketch)

  will appear as a curve in the sketch. For example:

y = sin(x)

**RangeStart** and **RangeEnd**

You cannot specify string values for RangeStart and RangeEnd; you must specify double values.

**XOffset:**

  In the equation:

y = sin(x) [x=0 to 2Pi]

  the start point (0,0) is moved by XOffset in the x direction.

**YOffset:**

In the equation:

y = sin(x) [x=0 to 2Pi]

  the start point (0,0) is moved by YOffset in the y direction.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchSpline Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline.html)

[ISketchSpline Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline_members.html)

[ISketchManager::CreateEquationSpline Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateEquationSpline.html)

[ISketchSpline::GetEquationParameters Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSpline~GetEquationParameters.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0
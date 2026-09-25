<!-- source: emodelapi/eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~SetMeasureUnits.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| SetMeasureUnits Method (IEModelMarkupControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelMarkupControl Namespace](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl_namespace.html) > [IEModelMarkupControl Interface](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html) : SetMeasureUnits Method (IEModelMarkupControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DistanceUnit*
:   Distance unit as defined in [EMVDistanceUnit](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.EMVDistanceUnit.html)

*AngleUnit*
:   Angle unit as defined in [EMVAngleUnit](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.EMVAngleUnit.html)

Sets measurement units.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetMeasureUnits( _    ByVal DistanceUnit As EMVDistanceUnit, _    ByVal AngleUnit As EMVAngleUnit _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelMarkupControl Dim DistanceUnit As EMVDistanceUnit Dim AngleUnit As EMVAngleUnit   instance.SetMeasureUnits(DistanceUnit, AngleUnit) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMeasureUnits(     EMVDistanceUnit DistanceUnit,    EMVAngleUnit AngleUnit ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMeasureUnits(  &   EMVDistanceUnit DistanceUnit, &   EMVAngleUnit AngleUnit ) ``` | |

#### Parameters

*DistanceUnit*
:   Distance unit as defined in [EMVDistanceUnit](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.EMVDistanceUnit.html)

*AngleUnit*
:   Angle unit as defined in [EMVAngleUnit](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.EMVAngleUnit.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelMarkupControl::SetMeasureUnits.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelMarkupControl Interface](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html)

[IEModelMarkupControl Members](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2017 SP3
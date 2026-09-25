<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~SelectByRay.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| SelectByRay Method (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : SelectByRay Method (IEModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StartX*
:   x coordinate of start point

*StartY*
:   y coordinate of start point

*StartZ*
:   z coordinate of start point

*DirectionX*
:   x coordinate of direction vector

*DirectionY*
:   y coordinate of direction vector

*DirectionZ*
:   y coordinate of direction vector

Selects the first component intersected by a ray that starts at the specified point in the specified direction vector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SelectByRay( _    ByVal StartX As System.Single, _    ByVal StartY As System.Single, _    ByVal StartZ As System.Single, _    ByVal DirectionX As System.Single, _    ByVal DirectionY As System.Single, _    ByVal DirectionZ As System.Single _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim StartX As System.Single Dim StartY As System.Single Dim StartZ As System.Single Dim DirectionX As System.Single Dim DirectionY As System.Single Dim DirectionZ As System.Single   instance.SelectByRay(StartX, StartY, StartZ, DirectionX, DirectionY, DirectionZ) ``` | |

| C# |  |
| --- | --- |
| ``` void SelectByRay(     System.float StartX,    System.float StartY,    System.float StartZ,    System.float DirectionX,    System.float DirectionY,    System.float DirectionZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SelectByRay(  &   System.float StartX, &   System.float StartY, &   System.float StartZ, &   System.float DirectionX, &   System.float DirectionY, &   System.float DirectionZ ) ``` | |

#### Parameters

*StartX*
:   x coordinate of start point

*StartY*
:   y coordinate of start point

*StartZ*
:   z coordinate of start point

*DirectionX*
:   x coordinate of direction vector

*DirectionY*
:   y coordinate of direction vector

*DirectionZ*
:   y coordinate of direction vector

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::SelectByRay.

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [IEModelViewControl::GetSelectedComponentName](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~GetSelectedComponentName.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2014 SP0
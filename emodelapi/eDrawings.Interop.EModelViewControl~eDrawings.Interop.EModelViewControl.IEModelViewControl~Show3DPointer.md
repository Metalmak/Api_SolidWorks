<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~Show3DPointer.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| Show3DPointer Method (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : Show3DPointer Method (IEModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*show*
:   True to show the 3D Pointer, false to hide it

*StartX*
:   x coordinate of the position of the sphere and the start point of the line

*StartY*
:   y coordinate of the position of the sphere and the start point of the line

*StartZ*
:   z coordinate of the position of the sphere and the start point of the line

*EndX*
:   x coordinate of the end point of the line

*EndY*
:   y coordinate of the end point of the line

*EndZ*
:   z coordinate of the end point of the line

Shows or hides a 3D pointer in the active view in the graphics area.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Show3DPointer( _    ByVal show As System.Boolean, _    ByVal StartX As System.Single, _    ByVal StartY As System.Single, _    ByVal StartZ As System.Single, _    ByVal EndX As System.Single, _    ByVal EndY As System.Single, _    ByVal EndZ As System.Single _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim show As System.Boolean Dim StartX As System.Single Dim StartY As System.Single Dim StartZ As System.Single Dim EndX As System.Single Dim EndY As System.Single Dim EndZ As System.Single   instance.Show3DPointer(show, StartX, StartY, StartZ, EndX, EndY, EndZ) ``` | |

| C# |  |
| --- | --- |
| ``` void Show3DPointer(     System.bool show,    System.float StartX,    System.float StartY,    System.float StartZ,    System.float EndX,    System.float EndY,    System.float EndZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Show3DPointer(  &   System.bool show, &   System.float StartX, &   System.float StartY, &   System.float StartZ, &   System.float EndX, &   System.float EndY, &   System.float EndZ ) ``` | |

#### Parameters

*show*
:   True to show the 3D Pointer, false to hide it

*StartX*
:   x coordinate of the position of the sphere and the start point of the line

*StartY*
:   y coordinate of the position of the sphere and the start point of the line

*StartZ*
:   z coordinate of the position of the sphere and the start point of the line

*EndX*
:   x coordinate of the end point of the line

*EndY*
:   y coordinate of the end point of the line

*EndZ*
:   z coordinate of the end point of the line

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::Show3DPointer.

# ![](dotnetimages/collapse.gif)Remarks

The [3D pointer](3DPointer.gif) shown by this method is not the same 3D pointer available in the eDrawings user interface.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2014 SP0
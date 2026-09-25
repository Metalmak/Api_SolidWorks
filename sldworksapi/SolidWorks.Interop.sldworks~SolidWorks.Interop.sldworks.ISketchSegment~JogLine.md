<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~JogLine.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| JogLine Method (ISketchSegment) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html) : JogLine Method (ISketchSegment) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XOnLine*
:   x coordinate where to begin the jog on the selected line

*YOnLine*
:   y coordinate where to begin the jog on the selected line

*ZOnLine*
:   z coordinate where to begin the jog on the selected line

*XOnJog*
:   x coordinate of the width and depth of the jog

*YOnJog*
:   y coordinate of the width and depth of the jog

*ZOnJog*
:   z coordinate of the width and depth of the jog

Creates rectangular jog on the specified line.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub JogLine( _    ByVal XOnLine As System.Double, _    ByVal YOnLine As System.Double, _    ByVal ZOnLine As System.Double, _    ByVal XOnJog As System.Double, _    ByVal YOnJog As System.Double, _    ByVal ZOnJog As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchSegment Dim XOnLine As System.Double Dim YOnLine As System.Double Dim ZOnLine As System.Double Dim XOnJog As System.Double Dim YOnJog As System.Double Dim ZOnJog As System.Double   instance.JogLine(XOnLine, YOnLine, ZOnLine, XOnJog, YOnJog, ZOnJog) ``` | |

| C# |  |
| --- | --- |
| ``` void JogLine(     System.double XOnLine,    System.double YOnLine,    System.double ZOnLine,    System.double XOnJog,    System.double YOnJog,    System.double ZOnJog ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void JogLine(  &   System.double XOnLine, &   System.double YOnLine, &   System.double ZOnLine, &   System.double XOnJog, &   System.double YOnJog, &   System.double ZOnJog ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XOnLine*
:   x coordinate where to begin the jog on the selected line

*YOnLine*
:   y coordinate where to begin the jog on the selected line

*ZOnLine*
:   z coordinate where to begin the jog on the selected line

*XOnJog*
:   x coordinate of the width and depth of the jog

*YOnJog*
:   y coordinate of the width and depth of the jog

*ZOnJog*
:   z coordinate of the width and depth of the jog

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchSegment::JogLine.

# ![](dotnetimages/collapse.gif)Example

[Insert Explode Line Sketch and Jog Line (VB.NET)](Insert_Explode_Line_Sketch_and_Jog_Line_Example_VBNET.htm)

[Insert Explode Line Sketch and Jog Line (VBA)](Insert_Explode_Line_Sketch_and_Jog_Line_Example_VB.htm)

[Insert Explode Line Sketch and Jog Line (C#)](Insert_Explode_Line_Sketch_and_Jog_Line_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html)

[ISketchSegment Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment_members.html)

[ISketchManager::InsertExplodeLineSketch Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~InsertExplodeLineSketch.html)

[ISketchManager::Insert3DSketch Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~Insert3DSketch.html)

[ISketch::InsertRouteLine Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~InsertRouteLine.html)

[ISketchManager::CreateLine Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateLine.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertLinearNotePattern.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertLinearNotePattern Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : InsertLinearNotePattern Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumX*
:   Total number of instances along the x axis, including the seed

*NumY*
:   Total number of instances along the y axis, including the seed

*SpacingX*
:   Spacing between pattern instances along the x axis

*SpacingY*
:   Spacing between pattern instances along the y axis

*AngleX*
:   Angle for direction 1 relative to the x axis

*AngleY*
:   Angle for direction 2 relative to the y axis

*DeleteInstances*
:   Number of instances to delete, passed as a string in the format "(a) (b) (c) "

Inserts a linear note pattern using the selected [note](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertLinearNotePattern( _    ByVal NumX As System.Integer, _    ByVal NumY As System.Integer, _    ByVal SpacingX As System.Double, _    ByVal SpacingY As System.Double, _    ByVal AngleX As System.Double, _    ByVal AngleY As System.Double, _    ByVal DeleteInstances As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim NumX As System.Integer Dim NumY As System.Integer Dim SpacingX As System.Double Dim SpacingY As System.Double Dim AngleX As System.Double Dim AngleY As System.Double Dim DeleteInstances As System.String Dim value As System.Boolean   value = instance.InsertLinearNotePattern(NumX, NumY, SpacingX, SpacingY, AngleX, AngleY, DeleteInstances) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertLinearNotePattern(     System.int NumX,    System.int NumY,    System.double SpacingX,    System.double SpacingY,    System.double AngleX,    System.double AngleY,    System.string DeleteInstances ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertLinearNotePattern(  &   System.int NumX, &   System.int NumY, &   System.double SpacingX, &   System.double SpacingY, &   System.double AngleX, &   System.double AngleY, &   System.String^ DeleteInstances ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumX*
:   Total number of instances along the x axis, including the seed

*NumY*
:   Total number of instances along the y axis, including the seed

*SpacingX*
:   Spacing between pattern instances along the x axis

*SpacingY*
:   Spacing between pattern instances along the y axis

*AngleX*
:   Angle for direction 1 relative to the x axis

*AngleY*
:   Angle for direction 2 relative to the y axis

*DeleteInstances*
:   Number of instances to delete, passed as a string in the format "(a) (b) (c) "

#### Return Value

True if the linear note pattern is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::InsertLinearNotePattern.

# ![](dotnetimages/collapse.gif)Example

[Insert Linear and Circular Note Patterns (C#)](Insert_Linear_and_Circular_Note_Patterns_Example_CSharp.htm)

[Insert Linear and Circular Note Patterns (VB.NET)](Insert_Linear_and_Circular_Note_Patterns_Example_VBNET.htm)

[Insert Linear and Circular Note Patterns (VBA)](Insert_Linear_and_Circular_Note_Patterns_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::InsertCircularNotePattern Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertCircularNotePattern.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertCircularNotePattern.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertCircularNotePattern Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : InsertCircularNotePattern Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ArcRadius*
:   Radius for the circular note pattern

*ArcAngle*
:   Angle relative to the notes being patterned

*PatternNum*
:   Total number of pattern instances, including the seed geometry

*PatternSpacing*
:   Spacing between pattern instances in radians

*PatternRotate*
:   True to rotate the pattern, false to not

*DeleteInstances*
:   Number of instances to delete, passed as a string formatted as "(a) (b) (c) "

Inserts a circular note pattern using the selected [note](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertCircularNotePattern( _    ByVal ArcRadius As System.Double, _    ByVal ArcAngle As System.Double, _    ByVal PatternNum As System.Integer, _    ByVal PatternSpacing As System.Double, _    ByVal PatternRotate As System.Boolean, _    ByVal DeleteInstances As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim ArcRadius As System.Double Dim ArcAngle As System.Double Dim PatternNum As System.Integer Dim PatternSpacing As System.Double Dim PatternRotate As System.Boolean Dim DeleteInstances As System.String Dim value As System.Boolean   value = instance.InsertCircularNotePattern(ArcRadius, ArcAngle, PatternNum, PatternSpacing, PatternRotate, DeleteInstances) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertCircularNotePattern(     System.double ArcRadius,    System.double ArcAngle,    System.int PatternNum,    System.double PatternSpacing,    System.bool PatternRotate,    System.string DeleteInstances ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertCircularNotePattern(  &   System.double ArcRadius, &   System.double ArcAngle, &   System.int PatternNum, &   System.double PatternSpacing, &   System.bool PatternRotate, &   System.String^ DeleteInstances ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ArcRadius*
:   Radius for the circular note pattern

*ArcAngle*
:   Angle relative to the notes being patterned

*PatternNum*
:   Total number of pattern instances, including the seed geometry

*PatternSpacing*
:   Spacing between pattern instances in radians

*PatternRotate*
:   True to rotate the pattern, false to not

*DeleteInstances*
:   Number of instances to delete, passed as a string formatted as "(a) (b) (c) "

#### Return Value

True if the circular note pattern is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::InsertCircularNotePattern.

# ![](dotnetimages/collapse.gif)Example

[Insert Linear and Circular Note Patterns (C#)](Insert_Linear_and_Circular_Note_Patterns_Example_CSharp.htm)

[Insert Linear and Circular Note Patterns (VB.NET)](Insert_Linear_and_Circular_Note_Patterns_Example_VBNET.htm)

[Insert Linear and Circular Note Patterns (VBA)](Insert_Linear_and_Circular_Note_Patterns_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::InsertLinearNotePattern Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertLinearNotePattern.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0
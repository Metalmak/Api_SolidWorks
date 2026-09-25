<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertNewNote2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertNewNote2 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : InsertNewNote2 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UpperText*
:   Upper text string to be put in the note

*LowerText*
:   Unused; pass an empty string

*NoLeader*
:   True does not add a leader line, false does

*BentLeader*
:   True adds a bent leader line, false does not

*ArrowStyle*
:   Arrowhead type as defined in swArrowStyle\_e

*LeaderSide*
:   Leader line side as defined in swLeaderSide\_e

*Angle*
:   Text angle

*BalloonStyle*
:   Balloon style type as defined in swBalloonStyle\_e

*BalloonFit*
:   Balloon fit type as defined in swBalloonFit\_e

*UpperNoteContent*
:   Unused; set to 0

*LowerNoteContent*
:   Unused; set to 0

Creates a new note in this drawing.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertNewNote2( _    ByVal UpperText As System.String, _    ByVal LowerText As System.String, _    ByVal NoLeader As System.Boolean, _    ByVal BentLeader As System.Boolean, _    ByVal ArrowStyle As System.Short, _    ByVal LeaderSide As System.Short, _    ByVal Angle As System.Double, _    ByVal BalloonStyle As System.Short, _    ByVal BalloonFit As System.Short, _    ByVal UpperNoteContent As System.Short, _    ByVal LowerNoteContent As System.Short _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim UpperText As System.String Dim LowerText As System.String Dim NoLeader As System.Boolean Dim BentLeader As System.Boolean Dim ArrowStyle As System.Short Dim LeaderSide As System.Short Dim Angle As System.Double Dim BalloonStyle As System.Short Dim BalloonFit As System.Short Dim UpperNoteContent As System.Short Dim LowerNoteContent As System.Short   instance.InsertNewNote2(UpperText, LowerText, NoLeader, BentLeader, ArrowStyle, LeaderSide, Angle, BalloonStyle, BalloonFit, UpperNoteContent, LowerNoteContent) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertNewNote2(     System.string UpperText,    System.string LowerText,    System.bool NoLeader,    System.bool BentLeader,    System.short ArrowStyle,    System.short LeaderSide,    System.double Angle,    System.short BalloonStyle,    System.short BalloonFit,    System.short UpperNoteContent,    System.short LowerNoteContent ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertNewNote2(  &   System.String^ UpperText, &   System.String^ LowerText, &   System.bool NoLeader, &   System.bool BentLeader, &   System.short ArrowStyle, &   System.short LeaderSide, &   System.double Angle, &   System.short BalloonStyle, &   System.short BalloonFit, &   System.short UpperNoteContent, &   System.short LowerNoteContent ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UpperText*
:   Upper text string to be put in the note

*LowerText*
:   Unused; pass an empty string

*NoLeader*
:   True does not add a leader line, false does

*BentLeader*
:   True adds a bent leader line, false does not

*ArrowStyle*
:   Arrowhead type as defined in swArrowStyle\_e

*LeaderSide*
:   Leader line side as defined in swLeaderSide\_e

*Angle*
:   Text angle

*BalloonStyle*
:   Balloon style type as defined in swBalloonStyle\_e

*BalloonFit*
:   Balloon fit type as defined in swBalloonFit\_e

*UpperNoteContent*
:   Unused; set to 0

*LowerNoteContent*
:   Unused; set to 0

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::InsertNewNote2.

# ![](dotnetimages/collapse.gif)Example

Contact SOLIDWORKS API Support to obtain **Insert Note Leader at Sketch Point (VBA, VB.NET, and C#)**.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::CreateCompoundNote Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateCompoundNote.html)

[IDrawingDoc::CreateText2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~CreateText2.html)

[IDrawingDoc::ICreateCompoundNote Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateCompoundNote.html)

[IDrawingDoc::ICreateText2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateText2.html)

[IDrawingDoc::NewNote Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~NewNote.html)

[IDrawingDoc::InsertRevisionSymbol Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertRevisionSymbol.html)

[IDrawingDoc::InsertCircularNotePattern Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertCircularNotePattern.html)

[IDrawingDoc::InsertLinearNotePattern Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertLinearNotePattern.html)
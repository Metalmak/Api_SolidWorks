<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertNewNote.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertNewNote Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : InsertNewNote Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Text*

*NoLeader*

*BalloonNote*

*BentLeader*

*ArrowStyle*

*LeaderSide*

Obsolete. Superseded by [IDrawingDoc::InsertNewNote2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~InsertNewNote2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertNewNote( _    ByVal Text As System.String, _    ByVal NoLeader As System.Boolean, _    ByVal BalloonNote As System.Boolean, _    ByVal BentLeader As System.Boolean, _    ByVal ArrowStyle As System.Short, _    ByVal LeaderSide As System.Short _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Text As System.String Dim NoLeader As System.Boolean Dim BalloonNote As System.Boolean Dim BentLeader As System.Boolean Dim ArrowStyle As System.Short Dim LeaderSide As System.Short   instance.InsertNewNote(Text, NoLeader, BalloonNote, BentLeader, ArrowStyle, LeaderSide) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertNewNote(     System.string Text,    System.bool NoLeader,    System.bool BalloonNote,    System.bool BentLeader,    System.short ArrowStyle,    System.short LeaderSide ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertNewNote(  &   System.String^ Text, &   System.bool NoLeader, &   System.bool BalloonNote, &   System.bool BentLeader, &   System.short ArrowStyle, &   System.short LeaderSide ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Text*

*NoLeader*

*BalloonNote*

*BentLeader*

*ArrowStyle*

*LeaderSide*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::InsertNewNote.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)
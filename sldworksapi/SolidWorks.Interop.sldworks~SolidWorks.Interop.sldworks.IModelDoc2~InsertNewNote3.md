<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertNewNote3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertNewNote3 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertNewNote3 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UpperText*
:   Upper-text string to be put in the note

*NoLeader*
:   True for no leaderline, false if not

*BentLeader*
:   True for a bent leaderline, false if not

*ArrowStyle*
:   Arrowhead type as defined in swArrowStyle\_e

*LeaderSide*
:   Leaderline side as defined in swLeaderSide\_e

*Angle*
:   Text angle

*BalloonStyle*
:   Balloon style type as defined in swBalloonStyle\_e

*BalloonFit*
:   Balloon fit type as defined in swBalloonFit\_e

*SmartArrow*
:   If true then the arrow style specified in Options > Detailing is used for the arrows, if false then the ArrowStyle argument is used

Creates a new note.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertNewNote3( _    ByVal UpperText As System.String, _    ByVal NoLeader As System.Boolean, _    ByVal BentLeader As System.Boolean, _    ByVal ArrowStyle As System.Short, _    ByVal LeaderSide As System.Short, _    ByVal Angle As System.Double, _    ByVal BalloonStyle As System.Short, _    ByVal BalloonFit As System.Short, _    ByVal SmartArrow As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim UpperText As System.String Dim NoLeader As System.Boolean Dim BentLeader As System.Boolean Dim ArrowStyle As System.Short Dim LeaderSide As System.Short Dim Angle As System.Double Dim BalloonStyle As System.Short Dim BalloonFit As System.Short Dim SmartArrow As System.Boolean   instance.InsertNewNote3(UpperText, NoLeader, BentLeader, ArrowStyle, LeaderSide, Angle, BalloonStyle, BalloonFit, SmartArrow) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertNewNote3(     System.string UpperText,    System.bool NoLeader,    System.bool BentLeader,    System.short ArrowStyle,    System.short LeaderSide,    System.double Angle,    System.short BalloonStyle,    System.short BalloonFit,    System.bool SmartArrow ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertNewNote3(  &   System.String^ UpperText, &   System.bool NoLeader, &   System.bool BentLeader, &   System.short ArrowStyle, &   System.short LeaderSide, &   System.double Angle, &   System.short BalloonStyle, &   System.short BalloonFit, &   System.bool SmartArrow ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UpperText*
:   Upper-text string to be put in the note

*NoLeader*
:   True for no leaderline, false if not

*BentLeader*
:   True for a bent leaderline, false if not

*ArrowStyle*
:   Arrowhead type as defined in swArrowStyle\_e

*LeaderSide*
:   Leaderline side as defined in swLeaderSide\_e

*Angle*
:   Text angle

*BalloonStyle*
:   Balloon style type as defined in swBalloonStyle\_e

*BalloonFit*
:   Balloon fit type as defined in swBalloonFit\_e

*SmartArrow*
:   If true then the arrow style specified in Options > Detailing is used for the arrows, if false then the ArrowStyle argument is used

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertNewNote3.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::IInsertNote Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IInsertNote.html)

[IModelDoc2::InsertNote Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertNote.html)

[INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html)

[IDrawingDoc::InsertNewNote2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertNewNote2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0
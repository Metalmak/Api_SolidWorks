<!-- source: emodelapi/eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~ShowCommentx64.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| ShowCommentx64 Method (IEModelMarkupControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelMarkupControl Namespace](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl_namespace.html) > [IEModelMarkupControl Interface](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html) : ShowCommentx64 Method (IEModelMarkupControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CommentIDx64*
:   ID of markup comment to display on 64-bit systems

Displays the specified markup comment on 64-bit systems.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowCommentx64( _    ByVal CommentIDx64 As System.Long _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelMarkupControl Dim CommentIDx64 As System.Long   instance.ShowCommentx64(CommentIDx64) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowCommentx64(     System.long CommentIDx64 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowCommentx64(  &   System.int64 CommentIDx64 ) ``` | |

#### Parameters

*CommentIDx64*
:   ID of markup comment to display on 64-bit systems

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelMarkupControl::ShowCommentx64.

# ![](dotnetimages/collapse.gif)Remarks

Call [IEModelMarkupControl::CommentIDx64](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~CommentIDx64.html) before calling this method to determine the ID of the markup comment.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelMarkupControl Interface](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html)

[IEModelMarkupControl Members](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl_members.html)

[IEModelMarkupControl::ShowComment Method](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~ShowComment.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2011 SP01
<!-- source: emodelapi/eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~ShowComment.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| ShowComment Method (IEModelMarkupControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelMarkupControl Namespace](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl_namespace.html) > [IEModelMarkupControl Interface](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html) : ShowComment Method (IEModelMarkupControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CommentID*
:   ID of markup comment to display

Displays the specified markup comment.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowComment( _    ByVal CommentID As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelMarkupControl Dim CommentID As System.Integer   instance.ShowComment(CommentID) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowComment(     System.int CommentID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowComment(  &   System.int CommentID ) ``` | |

#### Parameters

*CommentID*
:   ID of markup comment to display

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelMarkupControl::ShowComment.

# ![](dotnetimages/collapse.gif)Example

See the [IEModelMarkupControl](eDrawings.Interop.EModelMarkupControl.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Call [IEModelMarkupControl::CommentID](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~CommentID.html) before calling this method to determine the ID of the markup comment.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelMarkupControl Interface](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html)

[IEModelMarkupControl Members](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl_members.html)

[IEModelMarkupControl::CommentName Property](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~CommentName.html)

[IEModelMarkupControl::ShowCommentx64 Method](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~ShowCommentx64.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2005 SP0
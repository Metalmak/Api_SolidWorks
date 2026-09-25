<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IMessageBarHandler~OnUserResponseB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnUserResponseB Method (IMessageBarHandler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IMessageBarHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IMessageBarHandler.html) : OnUserResponseB Method (IMessageBarHandler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DoNotShowAgain*
:   True to check "Don't Show Again", false to not

Called by SOLIDWORKS when the user selects the second response control.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnUserResponseB( _    ByVal DoNotShowAgain As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMessageBarHandler Dim DoNotShowAgain As System.Boolean   instance.OnUserResponseB(DoNotShowAgain) ``` | |

| C# |  |
| --- | --- |
| ``` void OnUserResponseB(     System.bool DoNotShowAgain ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnUserResponseB(  &   System.bool DoNotShowAgain ) ``` | |

#### Parameters

*DoNotShowAgain*
:   True to check "Don't Show Again", false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MessageBarHandler::OnUserResponseB.

# ![](dotnetimages/collapse.gif)Example

See the [IMessageBarHandler](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IMessageBarHandler.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IMessageBarHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IMessageBarHandler.html)

[IMessageBarHandler Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IMessageBarHandler_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30
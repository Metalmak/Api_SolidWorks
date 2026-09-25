<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView6~OnCancel.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| OnCancel Method (IEdmCardView6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardView6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView6.html) : OnCancel Method (IEdmCardView6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Rolls back all changes made in the card view after it is cancelled.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub OnCancel() ``` | |

| C# |  |
| --- | --- |
| ``` void OnCancel() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnCancel(); ``` | |

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCardView6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Call this method when the card view is cancelled. This method ensures that all serial numbers generated in the card (by right-clicking in edit boxes linked to serial numbers) are pushed back to the database so they can be reused. If you do not call this method, serial numbers are not restored to the database, and gaps in the serial number series occur.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardView6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView6.html)

[IEdmCardView6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0
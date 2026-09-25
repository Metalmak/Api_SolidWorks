<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5~Refresh.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Refresh Method (IEdmObject5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmObject5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5.html) : Refresh Method (IEdmObject5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Re-reads cached properties from the database.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Refresh() ``` | |

| C# |  |
| --- | --- |
| ``` void Refresh() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Refresh(); ``` | |

# ![](dotnetimages/collapse.gif)Remarks

In a multi-user implementation, the object may change as you are working on it. Call this method to ensure that you are seeing the latest state of the object.

For performance reasons, some object properties might be cached in the object itself. This method ensures that cached properties are re-read from the database.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_EDM\_DATABASE\_ACCESS: General error accessing the database.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmObject5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5.html)

[IEdmObject5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional
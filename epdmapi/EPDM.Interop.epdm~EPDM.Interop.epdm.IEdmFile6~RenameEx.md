<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile6~RenameEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| RenameEx Method (IEdmFile6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile6.html) : RenameEx Method (IEdmFile6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*bsNewName*
:   New file name

*lFlags*
:   0; reserved

Changes the name of this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub RenameEx( _    ByVal lParentWnd As System.Integer, _    ByVal bsNewName As System.String, _    ByVal lFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void RenameEx(     System.int lParentWnd,    System.string bsNewName,    System.int lFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RenameEx(  &   System.int lParentWnd, &   System.String^ bsNewName, &   System.int lFlags ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*bsNewName*
:   New file name

*lFlags*
:   0; reserved

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile6.html)

[IEdmFile6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0
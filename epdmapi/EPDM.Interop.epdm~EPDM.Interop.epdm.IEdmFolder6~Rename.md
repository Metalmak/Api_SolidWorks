<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6~Rename.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rename Method (IEdmFolder6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6.html) : Rename Method (IEdmFolder6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*bsNewName*
:   New name of the folder

*lFlags*
:   0; reserved for future use

Renames this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rename( _    ByVal lParentWnd As System.Integer, _    ByVal bsNewName As System.String, _    ByVal lFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Rename(     System.int lParentWnd,    System.string bsNewName,    System.int lFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rename(  &   System.int lParentWnd, &   System.String^ bsNewName, &   System.int lFlags ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*bsNewName*
:   New name of the folder

*lFlags*
:   0; reserved for future use

# ![](dotnetimages/collapse.gif)Remarks

If this folder contains files with external references, this method could take an extended period of time to rewrite the include paths.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6.html)

[IEdmFolder6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0
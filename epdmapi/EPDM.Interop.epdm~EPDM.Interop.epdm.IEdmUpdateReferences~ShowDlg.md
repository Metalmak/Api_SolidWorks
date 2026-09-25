<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUpdateReferences~ShowDlg.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ShowDlg Method (IEdmUpdateReferences) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUpdateReferences Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUpdateReferences.html) : ShowDlg Method (IEdmUpdateReferences) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*lFlags*
:   Must be 0; reserved for future use

*lFolderID*
:   ID of the active folder; 0 to ignore

Displays the command dialog box for all of the files added to the batch with [IEdmUpdateReferences::AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUpdateReferences~AddFile.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub ShowDlg( _    ByVal lParentWnd As System.Integer, _    Optional ByVal lFlags As System.Integer, _    Optional ByVal lFolderID As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowDlg(     System.int lParentWnd,    System.int lFlags,    System.int lFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowDlg(  &   System.int lParentWnd, &   System.int lFlags, &   System.int lFolderID ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*lFlags*
:   Must be 0; reserved for future use

*lFolderID*
:   ID of the active folder; 0 to ignore

# ![](dotnetimages/collapse.gif)Example

[Update References (C#)](Update_References_Example_CSharp.htm)

[Update References (VB.NET)](Update_References_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUpdateReferences Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUpdateReferences.html)

[IEdmUpdateReferences Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUpdateReferences_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011
<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs~ShowEditReferencesDlg.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ShowEditReferencesDlg Method (IEdmAddCustomRefs) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddCustomRefs Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs.html) : ShowEditReferencesDlg Method (IEdmAddCustomRefs) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoFileIdArray*
:   Array of IDs of the files to edit

*lParentWnd*
:   Parent window handle

Displays the Edit User-Defined File References dialog box that allows the user to edit the existing file references.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function ShowEditReferencesDlg( _    ByRef ppoFileIdArray() As System.Integer, _    ByVal lParentWnd As System.Integer _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ShowEditReferencesDlg(     ref System.int[] ppoFileIdArray,    System.int lParentWnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ShowEditReferencesDlg(  &   System.array<int>^% ppoFileIdArray, &   System.int lParentWnd ) ``` | |

#### Parameters

*ppoFileIdArray*
:   Array of IDs of the files to edit

*lParentWnd*
:   Parent window handle

#### Return Value

True if the user modified the file references, false if no changes were made

# ![](dotnetimages/collapse.gif)Example

[Add Custom File Reference (VB.NET)](Add_Custom_File_Reference_Example_VBNET.htm)

[Add Custom File Reference (C#)](Add_Custom_File_Reference_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddCustomRefs Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs.html)

[IEdmAddCustomRefs Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional
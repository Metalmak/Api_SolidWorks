<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs~CreateTree.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateTree Method (IEdmAddCustomRefs) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddCustomRefs Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs.html) : CreateTree Method (IEdmAddCustomRefs) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lEdmCreateReferenceFlags*
:   Combination of [EdmCreateReferenceFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCreateReferenceFlags.html) bits

Computes the file reference tree.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateTree( _    ByVal lEdmCreateReferenceFlags As System.Integer _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateTree(     System.int lEdmCreateReferenceFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateTree(  &   System.int lEdmCreateReferenceFlags ) ``` | |

#### Parameters

*lEdmCreateReferenceFlags*
:   Combination of [EdmCreateReferenceFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCreateReferenceFlags.html) bits

#### Return Value

True if there are file references, false if not

# ![](dotnetimages/collapse.gif)Example

[Add Custom File Reference (VB.NET)](Add_Custom_File_Reference_Example_VBNET.htm)

[Add Custom File Reference (C#)](Add_Custom_File_Reference_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If this method returns true, call [IEdmAddCustomRefs::ShowDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs~ShowDlg.html) to display and edit the file references.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddCustomRefs Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs.html)

[IEdmAddCustomRefs Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional
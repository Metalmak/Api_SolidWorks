<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs~CreateReferences.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateReferences Method (IEdmAddCustomRefs) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddCustomRefs Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs.html) : CreateReferences Method (IEdmAddCustomRefs) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Creates the custom file references in the file vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateReferences() As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateReferences() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateReferences(); ``` | |

#### Return Value

True if any file was created, false if no files were created

# ![](dotnetimages/collapse.gif)Example

[Add Custom File Reference (VB.NET)](Add_Custom_File_Reference_Example_VBNET.htm)

[Add Custom File Reference (C#)](Add_Custom_File_Reference_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must call one of the following methods to add a file reference to another file:

* [IEdmAddCustomRefs::AddReferencesClipboard](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs~AddReferencesClipboard.html)* [IEdmAddCustomRefs2::AddReferencesID2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs2~AddReferencesID2.html)* [IEdmAddCustomRefs2::AddReferencesPath2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs2~AddReferencesPath2.html)

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddCustomRefs Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs.html)

[IEdmAddCustomRefs Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional
<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetFirstFolderPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstFolderPosition Method (IEdmFile5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) : GetFirstFolderPosition Method (IEdmFile5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Starts an enumeration of the parent folders of this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstFolderPosition() As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstFolderPosition() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstFolderPosition(); ``` | |

#### Return Value

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the first parent folder

# ![](dotnetimages/collapse.gif)Example

[Batch Add Files and Folders to Vault (VB.NET)](Batch_Add_Files_and_Folders_Example_VBNET.htm)

[Batch Add Files and Folders to Vault (C#)](Batch_Add_Files_and_Folders_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Files can be shared between several folders in SOLIDWORKS PDM Professional. Call [IEdmFolder5::AddFileShared](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFileShared.html) to share a file between several folders.

After calling this method to get the postion of the first parent folder in the list, call [IEdmFile5::GetNextFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetNextFolder.html) to get the parent folders.

C++ programmers not using smart-pointer wrapper functions must release the returned pointer to IEdmPos5.

See [Return Codes](ReturnCodes.htm) for the complete list of potential success and error codes. The following are just a few examples:

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[IEdmFile5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2
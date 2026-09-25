<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetReferenceTree.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetReferenceTree Method (IEdmFile5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) : GetReferenceTree Method (IEdmFile5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentFolderID*
:   ID of the file's parent folder (see **Remarks**)

*lVersionNo*
:   Version of the file for which to get references; 0 to get the latest version

Gets an interface to the files that reference or are referenced by this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetReferenceTree( _    ByVal lParentFolderID As System.Integer, _    Optional ByVal lVersionNo As System.Integer _ ) As IEdmReference5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmReference5 GetReferenceTree(     System.int lParentFolderID,    System.int lVersionNo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmReference5^ GetReferenceTree(  &   System.int lParentFolderID, &   System.int lVersionNo ) ``` | |

#### Parameters

*lParentFolderID*
:   ID of the file's parent folder (see **Remarks**)

*lVersionNo*
:   Version of the file for which to get references; 0 to get the latest version

#### Return Value

[IEdmReference5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html)

# ![](dotnetimages/collapse.gif)Example

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Some file types, such as files from AutoCAD, SOLIDWORKS, MS Word, etc., contain references to other files. You can also set up your own references via SOLIDWORKS PDM Professional's User Defined File References dialog box. SOLIDWORKS PDM Professional manages all of these references for you, and they appear in the check-in dialog box in the form of a reference tree.

To specify lParentFolderID, inspect all of the parent folders of this file by calling [IEdmFile5::GetFirstFolderPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetFirstFolderPosition.html) and [IEdmFile5::GetNextFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetNextFolder.html).

Use IEdmReference5 that is returned in ppoRetRoot to enumerate referenced files and referencing files and set up user-defined references.

C++ programmers not using smart-pointer wrapper functions must release the returned interface, IEdmReference5.

See [Return Codes](ReturnCodes.htm) for the complete list of potential success and error codes. The following are just a few examples:

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[IEdmFile5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2
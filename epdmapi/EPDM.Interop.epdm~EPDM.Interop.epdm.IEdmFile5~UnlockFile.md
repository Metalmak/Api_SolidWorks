<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~UnlockFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| UnlockFile Method (IEdmFile5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) : UnlockFile Method (IEdmFile5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*bsComment*
:   Version comment to show in the history dialog box

*lEdmUnlockFlags*
:   Optional combination of [EdmUnlockFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockFlag.html) bits; default is EdmUnlockFlag.EdmUnlock\_Simple

*poIEdmRefCallback*
:   Optional Nothing or null

Checks in this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub UnlockFile( _    ByVal lParentWnd As System.Integer, _    ByVal bsComment As System.String, _    Optional ByVal lEdmUnlockFlags As System.Integer, _    Optional ByVal poIEdmRefCallback As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void UnlockFile(     System.int lParentWnd,    System.string bsComment,    System.int lEdmUnlockFlags,    System.object poIEdmRefCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void UnlockFile(  &   System.int lParentWnd, &   System.String^ bsComment, &   System.int lEdmUnlockFlags, &   System.Object^ poIEdmRefCallback ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*bsComment*
:   Version comment to show in the history dialog box

*lEdmUnlockFlags*
:   Optional combination of [EdmUnlockFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockFlag.html) bits; default is EdmUnlockFlag.EdmUnlock\_Simple

*poIEdmRefCallback*
:   Optional Nothing or null

# ![](dotnetimages/collapse.gif)Example

[Add Custom File Reference (VB.NET)](Add_Custom_File_Reference_Example_VBNET.htm)

[Add Custom File Reference (C#)](Add_Custom_File_Reference_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If the file or its file data card contents have changed, this method creates a new version.

[IEdmBatchUnlock](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) is more efficient than this interface for checking in multiple files.

See [Return Codes](ReturnCodes.htm) for the complete list of potential success and error codes. The following are just a few examples:

* S\_OK: The method successfully executed.* S\_FALSE: The method successfully executed, but as no file is modified, SOLIDWORKS PDM Professional did not create a new version.* E\_EDM\_FILE\_NOT\_LOCKED\_BY\_YOU: The file is not checked out by the logged-in user.* E\_EDM\_LOCKED\_ON\_OTHER\_COMPUTER: The file is not checked out on the client machine where you tried to check it in.* E\_EDM\_FILE\_NOT\_FOUND: The file is not part of the vault.* E\_EDM\_LOCAL\_FILE\_NOT\_FOUND: There is no copy of the file in the cache folder on the client machine.* E\_EDM\_FILE\_SHARE\_ERROR: The file is open exclusively in another program.* E\_EDM\_CANCELLED\_BY\_USER: Not implemented.* E\_EDM\_INVALID\_FILE: The file format is not recognized, and you have specified to not check in such files.* E\_EDM\_MISSING\_MANDATORY\_VALUE: The file lacks a value for a required file data card variable.* E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN: One of the loaded [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreUndoLock hooks did not permit the operation.* E\_EDM\_FILE\_NOT\_REGENERATED: The file needs to be rebuilt.* E\_EDM\_NO\_WORKFLOW: The document does not meet the conditions of any workflow.* E\_EDM\_CIRCULAR\_XREF: A cyclic file reference was detected.* E\_EDM\_SWDRW\_SETTO\_USE\_INDEPENDENT\_REV\_TABLE: An independent type revision setting is used in the drawing.* E\_EDM\_NO\_DOCTYPE: The document does not meet the conditions of any category.* E\_EDM\_LOCKED\_IN\_OTHER\_FOLDER: The file is checked out in another folder.* E\_EDM\_FILE\_NAME\_NOT\_GLOBALLY\_UNIQUE: The file name is not unique.* E\_EDM\_TOOLBOX\_FILE\_LOCATED\_IN\_NONTOOLBOX\_FOLDER: Toolbox file must be located in a Toolbox folder.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[IEdmFile5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html)

[IEdmFile5::LockFile Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~LockFile.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2
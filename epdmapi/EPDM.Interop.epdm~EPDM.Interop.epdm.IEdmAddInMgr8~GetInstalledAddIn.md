<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8~GetInstalledAddIn.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetInstalledAddIn Method (IEdmAddInMgr8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddInMgr8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8.html) : GetInstalledAddIn Method (IEdmAddInMgr8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oNameOrID*
:   ID or name of the add-in

*bsExtractPath*
:   Path to the folder to which to extract files; ignored if empty

*poAddIn*
:   [EdmAddInInfo2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo2.html) structure; information about the add-in

*ppoFiles*
:   Array of [EdmAddInFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfo.html) structures, one for each file extracted from the add-in

*ppoCmds*
:   Array of [EdmAddInMenuInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo.html) structures, one for each menu command implemented by the add-in

Extracts files and information from the specified add-in.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetInstalledAddIn( _    ByVal oNameOrID As System.Object, _    ByVal bsExtractPath As System.String, _    ByRef poAddIn As EdmAddInInfo2, _    ByRef ppoFiles() As EdmAddInFileInfo, _    ByRef ppoCmds() As EdmAddInMenuInfo _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetInstalledAddIn(     System.object oNameOrID,    System.string bsExtractPath,    out EdmAddInInfo2 poAddIn,    out EdmAddInFileInfo[] ppoFiles,    out EdmAddInMenuInfo[] ppoCmds ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetInstalledAddIn(  &   System.Object^ oNameOrID, &   System.String^ bsExtractPath, &   [Out] EdmAddInInfo2 poAddIn, &   [Out] array<EdmAddInFileInfo>^ ppoFiles, &   [Out] array<EdmAddInMenuInfo>^ ppoCmds ) ``` | |

#### Parameters

*oNameOrID*
:   ID or name of the add-in

*bsExtractPath*
:   Path to the folder to which to extract files; ignored if empty

*poAddIn*
:   [EdmAddInInfo2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo2.html) structure; information about the add-in

*ppoFiles*
:   Array of [EdmAddInFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfo.html) structures, one for each file extracted from the add-in

*ppoCmds*
:   Array of [EdmAddInMenuInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo.html) structures, one for each menu command implemented by the add-in

# ![](dotnetimages/collapse.gif)Example

See the [IEdmAddInMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_ID: oNameOrID specified an ID that was not found.* E\_EDM\_INVALID\_NAME: oNameOrID specified a name that was not found.* E\_EDM\_FOLDER\_NOT\_FOUND: bsExtractPath contained a path to a missing folder.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddInMgr8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8.html)

[IEdmAddInMgr8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8_members.html)

[IEdmAddInMgr8::ExtractInstalledAddIn Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8~ExtractInstalledAddIn.html)

[IEdmAddInMgr7::GetInstalledAddIns Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr7~GetInstalledAddIns.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010
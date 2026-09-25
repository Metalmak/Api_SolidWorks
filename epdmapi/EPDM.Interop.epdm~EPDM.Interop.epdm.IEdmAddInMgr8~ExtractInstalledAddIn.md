<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8~ExtractInstalledAddIn.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ExtractInstalledAddIn Method (IEdmAddInMgr8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddInMgr8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8.html) : ExtractInstalledAddIn Method (IEdmAddInMgr8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oNameOrID*
:   ID or name of the add-in from which to extract files

*bsExtractPath*
:   Path to the folder to which to extract files; ignored if empty

*ppoFiles*
:   Array of [EdmAddInFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfo.html) structures, one structure for each extracted file

Extracts files from the specified add-in and places them in the specified folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub ExtractInstalledAddIn( _    ByVal oNameOrID As System.Object, _    ByVal bsExtractPath As System.String, _    ByRef ppoFiles() As EdmAddInFileInfo _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void ExtractInstalledAddIn(     System.object oNameOrID,    System.string bsExtractPath,    out EdmAddInFileInfo[] ppoFiles ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ExtractInstalledAddIn(  &   System.Object^ oNameOrID, &   System.String^ bsExtractPath, &   [Out] array<EdmAddInFileInfo>^ ppoFiles ) ``` | |

#### Parameters

*oNameOrID*
:   ID or name of the add-in from which to extract files

*bsExtractPath*
:   Path to the folder to which to extract files; ignored if empty

*ppoFiles*
:   Array of [EdmAddInFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfo.html) structures, one structure for each extracted file

# ![](dotnetimages/collapse.gif)Remarks

This method performs a subset of the functionality of [IEdmAddInMgr8::GetInstalledAddIn](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8~GetInstalledAddIn.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_ID: oNameOrID specified an ID that was not found.* E\_EDM\_INVALID\_NAME: oNameOrID specified a name that was not found.* E\_EDM\_FOLDER\_NOT\_FOUND: bsExtractPath contained a path to a missing folder.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddInMgr8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8.html)

[IEdmAddInMgr8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010
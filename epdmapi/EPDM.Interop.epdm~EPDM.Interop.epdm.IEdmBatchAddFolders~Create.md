<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders~Create.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Create Method (IEdmBatchAddFolders) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchAddFolders Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders.html) : Create Method (IEdmBatchAddFolders) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lHwnd*
:   Parent window handle that is passed to add-ins that are notified about folders added to the vault

*ppoRetFolders*
:   Array of [EdmFolderInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfo.html) structures; one structure for each folder added

*lEdmBatchCreateFolderFlags*
:   Combination of [EdmBatchCreateFolderFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchCreateFolderFlag.html) bits

Creates all the folders that were added to the batch using [IEdmBatchAddFolders::AddFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders~AddFolder.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Create( _    ByVal lHwnd As System.Integer, _    ByRef ppoRetFolders() As EdmFolderInfo, _    Optional ByVal lEdmBatchCreateFolderFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Create(     System.int lHwnd,    out EdmFolderInfo[] ppoRetFolders,    System.int lEdmBatchCreateFolderFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Create(  &   System.int lHwnd, &   [Out] array<EdmFolderInfo>^ ppoRetFolders, &   System.int lEdmBatchCreateFolderFlags ) ``` | |

#### Parameters

*lHwnd*
:   Parent window handle that is passed to add-ins that are notified about folders added to the vault

*ppoRetFolders*
:   Array of [EdmFolderInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfo.html) structures; one structure for each folder added

*lEdmBatchCreateFolderFlags*
:   Combination of [EdmBatchCreateFolderFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchCreateFolderFlag.html) bits

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchAddFolders](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_COULD\_NOT\_CREATE\_LOCAL\_FOLDER: The folders were created in the vault but could not be created in the local cache.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchAddFolders Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders.html)

[IEdmBatchAddFolders Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional
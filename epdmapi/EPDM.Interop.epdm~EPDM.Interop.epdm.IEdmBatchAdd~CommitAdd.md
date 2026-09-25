<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd~CommitAdd.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CommitAdd Method (IEdmBatchAdd) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchAdd Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html) : CommitAdd Method (IEdmBatchAdd) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lHwnd*
:   Parent window handle that is passed to add-ins that are notified about files and folders added to the vault

*ppoRetFiles*
:   Array of [EdmFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo.html) structures, one structure for each file and folder

*lEdmBatchAddFlags*
:   Combination of [EdmBatchAddFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchAddFlag.html) bits

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) or [IEdmCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html) to provide the caller with more information

Adds all files and folders in the batch to the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CommitAdd( _    ByVal lHwnd As System.Integer, _    ByRef ppoRetFiles() As EdmFileInfo, _    Optional ByVal lEdmBatchAddFlags As System.Integer, _    Optional ByVal poCallback As System.Object _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int CommitAdd(     System.int lHwnd,    out EdmFileInfo[] ppoRetFiles,    System.int lEdmBatchAddFlags,    System.object poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CommitAdd(  &   System.int lHwnd, &   [Out] array<EdmFileInfo>^ ppoRetFiles, &   System.int lEdmBatchAddFlags, &   System.Object^ poCallback ) ``` | |

#### Parameters

*lHwnd*
:   Parent window handle that is passed to add-ins that are notified about files and folders added to the vault

*ppoRetFiles*
:   Array of [EdmFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFileInfo.html) structures, one structure for each file and folder

*lEdmBatchAddFlags*
:   Combination of [EdmBatchAddFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchAddFlag.html) bits

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) or [IEdmCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html) to provide the caller with more information

#### Return Value

0 for success; See ppoRetFiles' EdmFileInfo.mhResult for each file added to the vault to get individual result codes

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchAdd Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html)

[IEdmBatchAdd Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional
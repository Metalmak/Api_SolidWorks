<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock~GetFileList.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFileList Method (IEdmBatchUnlock) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchUnlock Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) : GetFileList Method (IEdmBatchUnlock) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lEdmUnlockFileListFlags*
:   Combination of [EdmUnlockFileListFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockFileListFlag.html) bits

Gets the list of files to be unlocked.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFileList( _    ByVal lEdmUnlockFileListFlags As System.Integer _ ) As EdmSelectionList5 ``` | |

| C# |  |
| --- | --- |
| ``` EdmSelectionList5 GetFileList(     System.int lEdmUnlockFileListFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmSelectionList5^ GetFileList(  &   System.int lEdmUnlockFileListFlags ) ``` | |

#### Parameters

*lEdmUnlockFileListFlags*
:   Combination of [EdmUnlockFileListFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockFileListFlag.html) bits

#### Return Value

[IEdmSelectionList5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchUnlock](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

See the [IEdmBatchUnlock](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) remarks for information about using this method.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchUnlock Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html)

[IEdmBatchUnlock Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional
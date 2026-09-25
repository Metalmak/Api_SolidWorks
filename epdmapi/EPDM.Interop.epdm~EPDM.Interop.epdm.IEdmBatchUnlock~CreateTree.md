<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock~CreateTree.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateTree Method (IEdmBatchUnlock) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchUnlock Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) : CreateTree Method (IEdmBatchUnlock) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*lEdmUnlockBuildTreeFlags*
:   Combination of [EdmUnlockBuildTreeFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockBuildTreeFlags.html) bits

*poCallback*
:   [IEdmUnlockOpCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html); optional callback that you can implement to receive more information about the unlock operation

Creates the file reference tree.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateTree( _    ByVal lParentWnd As System.Integer, _    ByVal lEdmUnlockBuildTreeFlags As System.Integer, _    Optional ByVal poCallback As IEdmUnlockOpCallback _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateTree(     System.int lParentWnd,    System.int lEdmUnlockBuildTreeFlags,    IEdmUnlockOpCallback poCallback ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateTree(  &   System.int lParentWnd, &   System.int lEdmUnlockBuildTreeFlags, &   IEdmUnlockOpCallback^ poCallback ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*lEdmUnlockBuildTreeFlags*
:   Combination of [EdmUnlockBuildTreeFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockBuildTreeFlags.html) bits

*poCallback*
:   [IEdmUnlockOpCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUnlockOpCallback.html); optional callback that you can implement to receive more information about the unlock operation

#### Return Value

True if at least one file is valid for the operation, false if no files are valid for the operation

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
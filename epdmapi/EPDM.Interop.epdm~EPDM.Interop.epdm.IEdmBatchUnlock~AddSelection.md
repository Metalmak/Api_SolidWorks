<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock~AddSelection.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddSelection Method (IEdmBatchUnlock) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchUnlock Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) : AddSelection Method (IEdmBatchUnlock) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poVault*
:   [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html); vault to which the files belong

*ppoSelection*
:   Array of [IEdmSelItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2.html) structures; one structure for each file to unlock

Specifies the batch of files to be unlocked.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddSelection( _    ByVal poVault As EdmVault5, _    ByRef ppoSelection() As EdmSelItem _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddSelection(     EdmVault5 poVault,    ref EdmSelItem[] ppoSelection ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddSelection(  &   EdmVault5^ poVault, &   array<EdmSelItem>^% ppoSelection ) ``` | |

#### Parameters

*poVault*
:   [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html); vault to which the files belong

*ppoSelection*
:   Array of [IEdmSelItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem2.html) structures; one structure for each file to unlock

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchUnlock](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

See the [IEdmBatchUnlock](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) remarks for information about using this method.

When you call this method, SOLIDWORKS PDM Professional automatically adds the file's references to the unlock file set.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchUnlock Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html)

[IEdmBatchUnlock Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.3 of SOLIDWORKS PDM Professional
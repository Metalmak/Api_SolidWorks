<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration~AddSelection.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddSelection Method (IEdmBatchItemGeneration) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchItemGeneration Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration.html) : AddSelection Method (IEdmBatchItemGeneration) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poVault*
:   [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html); vault in which to create the new items

*ppoSelection*
:   Array of [EdmSelItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem.html) structures, one structure for each file from which to generate an item

Obsolete. Superseded by [IEdmBatchItemGeneration2::AddSelection2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration2~AddSelection2.html).

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
:   [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html); vault in which to create the new items

*ppoSelection*
:   Array of [EdmSelItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem.html) structures, one structure for each file from which to generate an item

# ![](dotnetimages/collapse.gif)Example

See the example in the [IEdmBatchItemGeneration](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration.html) topic.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchItemGeneration Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration.html)

[IEdmBatchItemGeneration Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010
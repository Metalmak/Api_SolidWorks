<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11~RecoverDeletedItems.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| RecoverDeletedItems Method (IEdmFolder11) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11.html) : RecoverDeletedItems Method (IEdmFolder11) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poDeletedItems*
:   Array of [EdmDeletedItems](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems.html)

Restores the specified deleted items in the recycle bin to this folder in the vault view.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub RecoverDeletedItems( _    ByVal poDeletedItems() As EdmDeletedItems _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void RecoverDeletedItems(     EdmDeletedItems[] poDeletedItems ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RecoverDeletedItems(  &   array<EdmDeletedItems>^ poDeletedItems ) ``` | |

#### Parameters

*poDeletedItems*
:   Array of [EdmDeletedItems](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmFolder11](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Use [IEdmFolder11::GetDeletedItems](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11~GetDeletedItems.html) to populate poDeletedItems.

Note that you cannot use this method to recover items that have been completely destroyed using [IEdmFolder7::DestroyDeletedItems](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder7~DestroyDeletedItems.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11.html)

[IEdmFolder11 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11_members.html)

[IEdmFolder5::DeleteFile Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~DeleteFile.html)

[IEdmFolder5::DeleteFolder Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~DeleteFolder.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018
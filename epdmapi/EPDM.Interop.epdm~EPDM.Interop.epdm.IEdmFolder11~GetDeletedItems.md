<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11~GetDeletedItems.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetDeletedItems Method (IEdmFolder11) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11.html) : GetDeletedItems Method (IEdmFolder11) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poDeletedItems*
:   Array of [EdmDeletedItems](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems.html)

*bRecursive*
:   True to recursively restore subfolder contents, false to not

Gets items deleted from this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetDeletedItems( _    ByRef poDeletedItems() As EdmDeletedItems, _    Optional ByVal bRecursive As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetDeletedItems(     out EdmDeletedItems[] poDeletedItems,    System.bool bRecursive ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetDeletedItems(  &   [Out] array<EdmDeletedItems>^ poDeletedItems, &   System.bool bRecursive ) ``` | |

#### Parameters

*poDeletedItems*
:   Array of [EdmDeletedItems](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDeletedItems.html)

*bRecursive*
:   True to recursively restore subfolder contents, false to not

# ![](dotnetimages/collapse.gif)Example

See the [IEdmFolder11](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Use [IEdmFolder11::RecoverDeletedItems](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11~RecoverDeletedItems.html) to restore poDeletedItems to the vault view.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11.html)

[IEdmFolder11 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018
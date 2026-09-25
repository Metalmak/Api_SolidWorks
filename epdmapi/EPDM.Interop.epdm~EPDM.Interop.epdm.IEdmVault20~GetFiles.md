<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault20~GetFiles.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFiles Method (IEdmVault20) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault20 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault20.html) : GetFiles Method (IEdmVault20) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poDocsIDs*
:   Array of [EdmDocIDs](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDocIDs.html)

Gets the specified files in this vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFiles( _    ByVal poDocsIDs() As EdmDocIDs _ ) As System.Object() ``` | |

| C# |  |
| --- | --- |
| ``` System.object[] GetFiles(     EdmDocIDs[] poDocsIDs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.array<Object^>^ GetFiles(  &   array<EdmDocIDs>^ poDocsIDs ) ``` | |

#### Parameters

*poDocsIDs*
:   Array of [EdmDocIDs](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDocIDs.html)

#### Return Value

Array of [IEdmFile5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)s

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault20 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault20.html)

[IEdmVault20 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault20_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2019
<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem2~GetUpdatedPaths.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetUpdatedPaths Method (IEdmRefItem2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRefItem2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem2.html) : GetUpdatedPaths Method (IEdmRefItem2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoUpdatedPathArr*
:   Array of [EdmUpdatedRefPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUpdatedRefPath.html)s

Gets the old and new paths of references that have been moved or renamed by another client.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetUpdatedPaths( _    ByRef ppoUpdatedPathArr() As EdmUpdatedRefPath _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetUpdatedPaths(     out EdmUpdatedRefPath[] ppoUpdatedPathArr ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetUpdatedPaths(  &   [Out] array<EdmUpdatedRefPath>^ ppoUpdatedPathArr ) ``` | |

#### Parameters

*ppoUpdatedPathArr*
:   Array of [EdmUpdatedRefPath](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUpdatedRefPath.html)s

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRefItem2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem2.html)

[IEdmRefItem2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2021 SP04
<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom~GetVersions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetVersions Method (IEdmBom) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom.html) : GetVersions Method (IEdmBom) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoVersions*
:   Array of [EdmBomVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomVersion.html) structures; one structure for each BOM version; the structure of the oldest version is at the beginning of the array

Gets the versions of this BOM.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetVersions( _    ByRef ppoVersions() As EdmBomVersion _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetVersions(     out EdmBomVersion[] ppoVersions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetVersions(  &   [Out] array<EdmBomVersion>^ ppoVersions ) ``` | |

#### Parameters

*ppoVersions*
:   Array of [EdmBomVersion](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomVersion.html) structures; one structure for each BOM version; the structure of the oldest version is at the beginning of the array

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBom](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom.html)

[IEdmBom Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009
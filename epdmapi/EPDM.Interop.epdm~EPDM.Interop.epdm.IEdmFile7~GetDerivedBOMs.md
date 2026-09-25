<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7~GetDerivedBOMs.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetDerivedBOMs Method (IEdmFile7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7.html) : GetDerivedBOMs Method (IEdmFile7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoBoms*
:   Array of [EdmBomInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomInfo.html)s

Gets the derived Bills of Materials for this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetDerivedBOMs( _    ByRef ppoBoms() As EdmBomInfo _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetDerivedBOMs(     out EdmBomInfo[] ppoBoms ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetDerivedBOMs(  &   [Out] array<EdmBomInfo>^ ppoBoms ) ``` | |

#### Parameters

*ppoBoms*
:   Array of [EdmBomInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomInfo.html)s

# ![](dotnetimages/collapse.gif)Example

See the [IEdmFile7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

A derived Bill of Materials is also known as a named or saved Bill of Materials.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7.html)

[IEdmFile7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009
<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars~GetRefVars.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetRefVars Method (IEdmBatchRefVars) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchRefVars Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars.html) : GetRefVars Method (IEdmBatchRefVars) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoVars*
:   Array of [EdmRefVar structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar.html)s; one structure for each reference variable whose value you want to retrieve

Gets the values of the specified reference variables.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetRefVars( _    ByRef ppoVars() As EdmRefVar _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetRefVars(     out EdmRefVar[] ppoVars ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetRefVars(  &   [Out] array<EdmRefVar>^ ppoVars ) ``` | |

#### Parameters

*ppoVars*
:   Array of [EdmRefVar structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar.html)s; one structure for each reference variable whose value you want to retrieve

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchRefVars](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method updates the moValue and mhResult members of the EdmRefVar structures. mlParentVersion = 0 gets the values from the latest version you have permission to read.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchRefVars Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars.html)

[IEdmBatchRefVars Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars_members.html)

[IEdmBatchRefVars::SetRefVars Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars~SetRefVars.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010
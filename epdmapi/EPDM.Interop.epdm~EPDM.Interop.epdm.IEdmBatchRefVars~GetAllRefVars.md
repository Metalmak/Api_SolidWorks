<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars~GetAllRefVars.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetAllRefVars Method (IEdmBatchRefVars) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchRefVars Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars.html) : GetAllRefVars Method (IEdmBatchRefVars) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoVars*
:   Array of [EdmRefVar structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar.html)s; one structure for each reference variable

*lParentFileID*
:   ID of parent file for which to get reference variables

*lParentFileVersion*
:   Version number of parent file for which to get reference variables; 0 gets the latest version if the parent file is checked in and the checked-out version if it is checked out

*lChildFileID*
:   ID of the referenced child file; 0 gets variables for all child references

*bsParentConfig*
:   Configuration of parent file for which to get reference variables; "" gets all configurations

*bsChildConfig*
:   Configuration of parent file for which to get reference variables; "" is ignored

Gets all of the values for the specified reference variables.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetAllRefVars( _    ByRef ppoVars() As EdmRefVar, _    ByVal lParentFileID As System.Integer, _    Optional ByVal lParentFileVersion As System.Integer, _    Optional ByVal lChildFileID As System.Integer, _    Optional ByVal bsParentConfig As System.String, _    Optional ByVal bsChildConfig As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetAllRefVars(     out EdmRefVar[] ppoVars,    System.int lParentFileID,    System.int lParentFileVersion,    System.int lChildFileID,    System.string bsParentConfig,    System.string bsChildConfig ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetAllRefVars(  &   [Out] array<EdmRefVar>^ ppoVars, &   System.int lParentFileID, &   System.int lParentFileVersion, &   System.int lChildFileID, &   System.String^ bsParentConfig, &   System.String^ bsChildConfig ) ``` | |

#### Parameters

*ppoVars*
:   Array of [EdmRefVar structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefVar.html)s; one structure for each reference variable

*lParentFileID*
:   ID of parent file for which to get reference variables

*lParentFileVersion*
:   Version number of parent file for which to get reference variables; 0 gets the latest version if the parent file is checked in and the checked-out version if it is checked out

*lChildFileID*
:   ID of the referenced child file; 0 gets variables for all child references

*bsParentConfig*
:   Configuration of parent file for which to get reference variables; "" gets all configurations

*bsChildConfig*
:   Configuration of parent file for which to get reference variables; "" is ignored

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchRefVars](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchRefVars Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars.html)

[IEdmBatchRefVars Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010
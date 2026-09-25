<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8~GetCAFInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetCAFInfo Method (IEdmAddInMgr8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddInMgr8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8.html) : GetCAFInfo Method (IEdmAddInMgr8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsCAFPath*
:   Path to the \*.CAF from which to get information

*bsExtractPath*
:   Path to the folder to which to extract files; ignored if empty

*poAddIn*
:   [EdmAddInInfo2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo2.html) structure; information about the add-in

*ppoFiles*
:   Array of [EdmAddInFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfo.html) structures, one for each file extracted from the add-in

*ppoCmds*
:   Array of [EdmAddInMenuInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo.html) structures, one for each menu command implemented by the add-in

Extracts files and information from an add-in that is stored in a \*.CAF that pre-dates SOLIDWORKS PDM Professional 2010.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetCAFInfo( _    ByVal bsCAFPath As System.String, _    ByVal bsExtractPath As System.String, _    ByRef poAddIn As EdmAddInInfo2, _    ByRef ppoFiles() As EdmAddInFileInfo, _    ByRef ppoCmds() As EdmAddInMenuInfo _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetCAFInfo(     System.string bsCAFPath,    System.string bsExtractPath,    out EdmAddInInfo2 poAddIn,    out EdmAddInFileInfo[] ppoFiles,    out EdmAddInMenuInfo[] ppoCmds ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetCAFInfo(  &   System.String^ bsCAFPath, &   System.String^ bsExtractPath, &   [Out] EdmAddInInfo2 poAddIn, &   [Out] array<EdmAddInFileInfo>^ ppoFiles, &   [Out] array<EdmAddInMenuInfo>^ ppoCmds ) ``` | |

#### Parameters

*bsCAFPath*
:   Path to the \*.CAF from which to get information

*bsExtractPath*
:   Path to the folder to which to extract files; ignored if empty

*poAddIn*
:   [EdmAddInInfo2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo2.html) structure; information about the add-in

*ppoFiles*
:   Array of [EdmAddInFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfo.html) structures, one for each file extracted from the add-in

*ppoCmds*
:   Array of [EdmAddInMenuInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInMenuInfo.html) structures, one for each menu command implemented by the add-in

# ![](dotnetimages/collapse.gif)Example

See the [IEdmAddInMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_FILE\_NOT\_FOUND: The specified \*.CAF file was not found.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddInMgr8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8.html)

[IEdmAddInMgr8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010
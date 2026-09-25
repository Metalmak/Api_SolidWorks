<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5~SetCardSource.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetCardSource Method (IEdmFolderData5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolderData5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5.html) : SetCardSource Method (IEdmFolderData5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lCardID*
:   ID of card to use

*bsExtensions*
:   Semicolon-delimited list of extensions; e.g., "DOC;XLS"

Sets the specified file card ID to use for the specified file extensions.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetCardSource( _    ByVal lCardID As System.Integer, _    Optional ByVal bsExtensions As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetCardSource(     System.int lCardID,    System.string bsExtensions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetCardSource(  &   System.int lCardID, &   System.String^ bsExtensions ) ``` | |

#### Parameters

*lCardID*
:   ID of card to use

*bsExtensions*
:   Semicolon-delimited list of extensions; e.g., "DOC;XLS"

# ![](dotnetimages/collapse.gif)Example

See the [IEdmFolderData5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolderData5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5.html)

[IEdmFolderData5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolderData5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2
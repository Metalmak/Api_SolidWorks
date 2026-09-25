<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory~AddFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFile Method (IEdmHistory) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmHistory Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory.html) : AddFile Method (IEdmHistory) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of file to add

Adds a file to the history listing.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFile( _    ByVal lFileID As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFile(     System.int lFileID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFile(  &   System.int lFileID ) ``` | |

#### Parameters

*lFileID*
:   ID of file to add

# ![](dotnetimages/collapse.gif)Example

See the [IEdmHistory](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmHistory Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory.html)

[IEdmHistory Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4
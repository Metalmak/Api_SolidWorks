<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~RefreshFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| RefreshFolder Method (IEdmVault5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : RefreshFolder Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsFolderPath*
:   File system path to the folder to refresh

Refreshes the file listing in the specified folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub RefreshFolder( _    ByVal bsFolderPath As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void RefreshFolder(     System.string bsFolderPath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RefreshFolder(  &   System.String^ bsFolderPath ) ``` | |

#### Parameters

*bsFolderPath*
:   File system path to the folder to refresh

# ![](dotnetimages/collapse.gif)Example

[Execute Template (C#)](Execute_Template_Example_CSharp.htm)

[Execute Template (VB.NET)](Execute_Template_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you use API methods to add, check out, or change the state of a file, the API does not automatically refresh its folder in File Explorer. That would be inefficient when processing a large number of files. If you check in a file using the API and browse to its folder using File Explorer, it appears to the user that the file is still checked out. This folder can be refreshed by one of the following techniques:

* Calling this method* Pressing F5* Navigating to a different folder and back again

There is no way to force a refresh on other machines.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2
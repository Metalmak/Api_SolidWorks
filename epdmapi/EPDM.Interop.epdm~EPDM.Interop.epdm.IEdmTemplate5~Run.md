<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5~Run.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Run Method (IEdmTemplate5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTemplate5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5.html) : Run Method (IEdmTemplate5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hParentWnd*
:   Parent window handle

*lCurrentFolderID*
:   ID of folder in which to run this template

Executes this template in the specified folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function Run( _    ByVal hParentWnd As System.Integer, _    ByVal lCurrentFolderID As System.Integer _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int Run(     System.int hParentWnd,    System.int lCurrentFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Run(  &   System.int hParentWnd, &   System.int lCurrentFolderID ) ``` | |

#### Parameters

*hParentWnd*
:   Parent window handle

*lCurrentFolderID*
:   ID of folder in which to run this template

#### Return Value

User-interface refresh flags as defined in [EdmRefreshFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefreshFlag.html)

# ![](dotnetimages/collapse.gif)Example

[Execute Template (C#)](Execute_Template_Example_CSharp.htm)

[Execute Template (VB.NET)](Execute_Template_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is extended by [IEdmTemplate53::RunEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate53~RunEx.html) which returns information about all of the files and folders created by the template.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTemplate5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5.html)

[IEdmTemplate5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2
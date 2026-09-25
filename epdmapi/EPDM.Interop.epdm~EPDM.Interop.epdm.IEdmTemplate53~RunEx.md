<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate53~RunEx.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| RunEx Method (IEdmTemplate53) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTemplate53 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate53.html) : RunEx Method (IEdmTemplate53) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hParentWnd*
:   Parent window handle

*lCurrentFolderID*
:   ID of the folder in which to execute this template

*ppoRetData*
:   Array of [IEdmData](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData.html) interfaces; one interface for each object created by this template

Executes this template in the specified folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function RunEx( _    ByVal hParentWnd As System.Integer, _    ByVal lCurrentFolderID As System.Integer, _    ByRef ppoRetData() As System.Object _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int RunEx(     System.int hParentWnd,    System.int lCurrentFolderID,    out System.object[] ppoRetData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int RunEx(  &   System.int hParentWnd, &   System.int lCurrentFolderID, &   [Out] System.array<Object^>^ ppoRetData ) ``` | |

#### Parameters

*hParentWnd*
:   Parent window handle

*lCurrentFolderID*
:   ID of the folder in which to execute this template

*ppoRetData*
:   Array of [IEdmData](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData.html) interfaces; one interface for each object created by this template

#### Return Value

User-interface refresh flags as defined in [EdmRefleshFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefreshFlag.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmTemplate53](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate53.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method executes this template like [IEdmTemplate5::Run](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5~Run.html) does, but it also returns information about all of the files, folders, and variables created by this template.

If your application needs to be backward compatible with SOLIDWORKS PDM Professional 5.2, use IEdmTemplate5::Run instead of this method.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTemplate53 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate53.html)

[IEdmTemplate53 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate53_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.3
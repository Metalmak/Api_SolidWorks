<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2~GetRevisionNumbers.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetRevisionNumbers Method (IEdmRevisionMgr2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevisionMgr2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2.html) : GetRevisionNumbers Method (IEdmRevisionMgr2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oIDorEmpty*
:   ID of revision number to get or null to get all revision numbers in the vault

*ppoRetData*
:   Array of [EdmRevNo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevNo.html) structures; one structure for each revision number

Gets the specified revision number in the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetRevisionNumbers( _    ByVal oIDorEmpty As System.Object, _    ByRef ppoRetData() As EdmRevNo _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetRevisionNumbers(     System.object oIDorEmpty,    out EdmRevNo[] ppoRetData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetRevisionNumbers(  &   System.Object^ oIDorEmpty, &   [Out] array<EdmRevNo>^ ppoRetData ) ``` | |

#### Parameters

*oIDorEmpty*
:   ID of revision number to get or null to get all revision numbers in the vault

*ppoRetData*
:   Array of [EdmRevNo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevNo.html) structures; one structure for each revision number

# ![](dotnetimages/collapse.gif)Example

[Find Revisions Using Component (C#)](Find_Revisions_Using_Component_Example_CSharp.htm)

[Find Revisions Using Component (VB.NET)](Find_Revisions_Using_Component_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevisionMgr2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2.html)

[IEdmRevisionMgr2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007 SP03
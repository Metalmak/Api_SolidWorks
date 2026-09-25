<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2~GetRevisionNumberComponents2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetRevisionNumberComponents2 Method (IEdmRevisionMgr2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevisionMgr2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2.html) : GetRevisionNumberComponents2 Method (IEdmRevisionMgr2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oNameIDorEmpty*
:   Name or ID of revision number component to retrieve, null to retrieve all components (see **Remarks**)

*ppoRetData*
:   Array of [EdmRevComponent2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2.html) structures; one structure for each revision number component

Gets the specified revision number components in the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetRevisionNumberComponents2( _    ByVal oNameIDorEmpty As System.Object, _    ByRef ppoRetData() As EdmRevComponent2 _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetRevisionNumberComponents2(     System.object oNameIDorEmpty,    out EdmRevComponent2[] ppoRetData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetRevisionNumberComponents2(  &   System.Object^ oNameIDorEmpty, &   [Out] array<EdmRevComponent2>^ ppoRetData ) ``` | |

#### Parameters

*oNameIDorEmpty*
:   Name or ID of revision number component to retrieve, null to retrieve all components (see **Remarks**)

*ppoRetData*
:   Array of [EdmRevComponent2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevComponent2.html) structures; one structure for each revision number component

# ![](dotnetimages/collapse.gif)Example

[Find Revisions Using Component (C#)](Find_Revisions_Using_Component_Example_CSharp.htm)

[Find Revisions Using Component (VB.NET)](Find_Revisions_Using_Component_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

If oNameIDorEmpty is a positive integer, it is interpreted as the ID of the component to retrieve. If it is a negative integer, it is interpreted as a revision number, and all components with that revision number are returned.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevisionMgr2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2.html)

[IEdmRevisionMgr2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007 SP03
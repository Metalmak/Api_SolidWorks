<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5~GetAddInInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetAddInInfo Method (IEdmAddInMgr5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddInMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5.html) : GetAddInInfo Method (IEdmAddInMgr5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsPath*
:   Path to the DLL about which to get information

*poReserved*
:   Null only

*poInfo*
:   [EdmAddInInfo structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo.html); returned add-in information

Obsolete. Superseded by [IEdmAddInMgr6::GetAddInInfo2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr6~GetAddInInfo2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetAddInInfo( _    ByVal bsPath As System.String, _    ByRef poReserved As System.Object, _    ByRef poInfo As EdmAddInInfo _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetAddInInfo(     System.string bsPath,    ref System.object poReserved,    out EdmAddInInfo poInfo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetAddInInfo(  &   System.String^ bsPath, &   System.Object^% poReserved, &   [Out] EdmAddInInfo poInfo ) ``` | |

#### Parameters

*bsPath*
:   Path to the DLL about which to get information

*poReserved*
:   Null only

*poInfo*
:   [EdmAddInInfo structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo.html); returned add-in information

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddInMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5.html)

[IEdmAddInMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional
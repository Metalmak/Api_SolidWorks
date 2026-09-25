<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr6~GetAddInInfo2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetAddInInfo2 Method (IEdmAddInMgr6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddInMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr6.html) : GetAddInInfo2 Method (IEdmAddInMgr6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsPath*
:   Path to the DLL about which to get information

*oReserved*
:   Must be empty

*poInfo*
:   [EdmAddInInfo2 structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo2.html); returned add-in information

Gets information about an add-in.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetAddInInfo2( _    ByVal bsPath As System.String, _    ByVal oReserved As System.Object, _    ByRef poInfo As EdmAddInInfo2 _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetAddInInfo2(     System.string bsPath,    System.object oReserved,    out EdmAddInInfo2 poInfo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetAddInInfo2(  &   System.String^ bsPath, &   System.Object^ oReserved, &   [Out] EdmAddInInfo2 poInfo ) ``` | |

#### Parameters

*bsPath*
:   Path to the DLL about which to get information

*oReserved*
:   Must be empty

*poInfo*
:   [EdmAddInInfo2 structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo2.html); returned add-in information

# ![](dotnetimages/collapse.gif)Example

See the [IEdmAddInMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method supersedes [IEdmAddInMgr5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5~GetAddInInfo.html) which returned less information about the add-in.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddInMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr6.html)

[IEdmAddInMgr6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr6_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional
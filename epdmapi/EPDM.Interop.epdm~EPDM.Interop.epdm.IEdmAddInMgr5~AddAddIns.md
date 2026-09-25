<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5~AddAddIns.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddAddIns Method (IEdmAddInMgr5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddInMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5.html) : AddAddIns Method (IEdmAddInMgr5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsPathList*
:   Linefeed-separated list of path and file names of add-in files

*lEdmAddAddInFlags*
:   Add-in option as defined in [EdmAddAddInFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddAddInFlags.html)

*poReserved*
:   Nothing or null

Installs add-ins in SOLIDWORKS PDM Professional.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddAddIns( _    ByVal bsPathList As System.String, _    ByVal lEdmAddAddInFlags As System.Integer, _    ByRef poReserved As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddAddIns(     System.string bsPathList,    System.int lEdmAddAddInFlags,    ref System.object poReserved ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddAddIns(  &   System.String^ bsPathList, &   System.int lEdmAddAddInFlags, &   System.Object^% poReserved ) ``` | |

#### Parameters

*bsPathList*
:   Linefeed-separated list of path and file names of add-in files

*lEdmAddAddInFlags*
:   Add-in option as defined in [EdmAddAddInFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddAddInFlags.html)

*poReserved*
:   Nothing or null

# ![](dotnetimages/collapse.gif)Example

See the [IEdmAddInMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddInMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5.html)

[IEdmAddInMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5_members.html)

[IEdmAddInMgr9::RemoveAddIn Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr9~RemoveAddIn.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional
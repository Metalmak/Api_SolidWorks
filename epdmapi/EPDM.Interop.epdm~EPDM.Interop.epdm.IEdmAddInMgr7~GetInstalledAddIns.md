<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr7~GetInstalledAddIns.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetInstalledAddIns Method (IEdmAddInMgr7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddInMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr7.html) : GetInstalledAddIns Method (IEdmAddInMgr7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoAddIns*
:   Array of [EdmAddInInfo2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo2.html) structures, one structure for each add-in

Gets information about all of the add-ins that have been installed in the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetInstalledAddIns( _    ByRef ppoAddIns() As EdmAddInInfo2 _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetInstalledAddIns(     out EdmAddInInfo2[] ppoAddIns ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetInstalledAddIns(  &   [Out] array<EdmAddInInfo2>^ ppoAddIns ) ``` | |

#### Parameters

*ppoAddIns*
:   Array of [EdmAddInInfo2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo2.html) structures, one structure for each add-in

# ![](dotnetimages/collapse.gif)Example

See the [IEdmAddInMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddInMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr7.html)

[IEdmAddInMgr7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr7_members.html)

[IEdmAddInMgr8::GetInstalledAddIn Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr8~GetInstalledAddIn.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2008
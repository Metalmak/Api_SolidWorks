<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetCustomData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetCustomData Method (IEdmReference5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html) : GetCustomData Method (IEdmReference5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lDataID*
:   User-defined ID of data to get

*poData*
:   Buffer in which to return data

Gets data stored with [IEdmReference5::SetCustomData](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~SetCustomData.html) in this file reference.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetCustomData( _    ByVal lDataID As System.Integer, _    ByRef poData As System.Object _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetCustomData(     System.int lDataID,    out System.object poData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetCustomData(  &   System.int lDataID, &   [Out] System.Object^ poData ) ``` | |

#### Parameters

*lDataID*
:   User-defined ID of data to get

*poData*
:   Buffer in which to return data

#### Return Value

True if the data was found, false if not

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: The data was not found (pbFoundlt returned false).

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html)

[IEdmReference5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5_members.html)

[IEdmReference5::SetCustomData Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~SetCustomData.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional
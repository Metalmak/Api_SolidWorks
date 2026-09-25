<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~SetCustomData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetCustomData Method (IEdmReference5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html) : SetCustomData Method (IEdmReference5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lDataID*
:   User-defined ID of data to store

*poData*
:   Data to store

Stores an arbitrary piece of data in this object.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetCustomData( _    ByVal lDataID As System.Integer, _    ByRef poData As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetCustomData(     System.int lDataID,    ref System.object poData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetCustomData(  &   System.int lDataID, &   System.Object^% poData ) ``` | |

#### Parameters

*lDataID*
:   User-defined ID of data to store

*poData*
:   Data to store

# ![](dotnetimages/collapse.gif)Remarks

The data is only stored in memory and is kept as long as [IEdmReference5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html) is add-referenced. You can get the stored data by calling [IEdmReference5::GetCustomData](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5~GetCustomData.html).

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmReference5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5.html)

[IEdmReference5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional
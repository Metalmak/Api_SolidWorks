<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData~Set.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Set Method (IEdmData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmData Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData.html) : Set Method (IEdmData) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eKey*
:   ID of property to update as defined in [EdmDataPropertyType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDataPropertyType.html)

*poValue*
:   New value of property

Sets one of the data object properties to a new value.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Set( _    ByVal eKey As EdmDataPropertyType, _    ByRef poValue As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Set(     EdmDataPropertyType eKey,    ref System.object poValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Set(  &   EdmDataPropertyType eKey, &   System.Object^% poValue ) ``` | |

#### Parameters

*eKey*
:   ID of property to update as defined in [EdmDataPropertyType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDataPropertyType.html)

*poValue*
:   New value of property

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmData Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData.html)

[IEdmData Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData_members.html)

[IEdmData::Get Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData~Get.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2
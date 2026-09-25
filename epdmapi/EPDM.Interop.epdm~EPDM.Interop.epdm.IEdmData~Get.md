<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData~Get.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Get Method (IEdmData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmData Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData.html) : Get Method (IEdmData) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eKey*
:   ID of property to retrieve as defined in [EdmDataPropertyType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDataPropertyType.html)

Gets a data object property value.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function Get( _    ByVal eKey As EdmDataPropertyType _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object Get(     EdmDataPropertyType eKey ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ Get(  &   EdmDataPropertyType eKey ) ``` | |

#### Parameters

*eKey*
:   ID of property to retrieve as defined in [EdmDataPropertyType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDataPropertyType.html)

#### Return Value

Property value or empty if not found

# ![](dotnetimages/collapse.gif)Example

See the [IEdmData](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

C++ programmers must remember to intialize the VARIANT struct for poValue with a call to VariantInit before calling the routine and release the returned data with a call to VariantClear.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmData Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData.html)

[IEdmData Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData_members.html)

[IEdmData::Set Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmData~Set.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2
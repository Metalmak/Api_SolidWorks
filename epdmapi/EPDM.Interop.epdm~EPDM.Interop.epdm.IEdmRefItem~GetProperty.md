<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem~GetProperty.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetProperty Method (IEdmRefItem) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRefItem Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem.html) : GetProperty Method (IEdmRefItem) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eProperty*
:   Type of property for which to get a value as defined in [EdmRefItemProperty](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefItemProperty.html)

*poValue*
:   Property value

Gets the value of the specified property of this item.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetProperty( _    ByVal eProperty As EdmRefItemProperty, _    ByRef poValue As System.Object _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetProperty(     EdmRefItemProperty eProperty,    out System.object poValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetProperty(  &   EdmRefItemProperty eProperty, &   [Out] System.Object^ poValue ) ``` | |

#### Parameters

*eProperty*
:   Type of property for which to get a value as defined in [EdmRefItemProperty](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefItemProperty.html)

*poValue*
:   Property value

#### Return Value

True if this property can be modified, false if not

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_INVALIDARG: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRefItem Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem.html)

[IEdmRefItem Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4
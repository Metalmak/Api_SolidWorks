<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem~GetRefs.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetRefs Method (IEdmRefItem) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRefItem Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem.html) : GetRefs Method (IEdmRefItem) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eType*
:   Type of reference to get as defined in [EdmRefType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefType.html)

*ppoRetItems*
:   Array of [IEdmRefItem](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem.html)s; one interface pointer for each item reference

Gets the references of this item.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetRefs( _    ByVal eType As EdmRefType, _    ByRef ppoRetItems() As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetRefs(     EdmRefType eType,    out System.object[] ppoRetItems ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetRefs(  &   EdmRefType eType, &   [Out] System.array<Object^>^ ppoRetItems ) ``` | |

#### Parameters

*eType*
:   Type of reference to get as defined in [EdmRefType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefType.html)

*ppoRetItems*
:   Array of [IEdmRefItem](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem.html)s; one interface pointer for each item reference

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRefItem Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem.html)

[IEdmRefItem Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4
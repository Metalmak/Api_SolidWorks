<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum~GetAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetAt Method (IEdmEnum) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnum Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum.html) : GetAt Method (IEdmEnum) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lIndex*
:   Zero-based index of the element to retrieve

Gets the element at the specified position in the list.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetAt( _    ByVal lIndex As System.Integer _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetAt(     System.int lIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetAt(  &   System.int lIndex ) ``` | |

#### Parameters

*lIndex*
:   Zero-based index of the element to retrieve

#### Return Value

Element at the specified position

# ![](dotnetimages/collapse.gif)Remarks

To enumerate a list, call [IEdmEnum::MoveNext](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum~MoveNext.html) and [IEdmEnum::Current](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum~Current.html), both of which are more efficient than this method.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_INVALIDARG: The specified index is outside the range of this list.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnum Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum.html)

[IEdmEnum Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013
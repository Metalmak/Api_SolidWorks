<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem~UpdateReferences.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| UpdateReferences Method (IEdmItem) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmItem Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem.html) : UpdateReferences Method (IEdmItem) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoAddReferences*
:   Array of [EdmItemRef](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef.html) structures; one structure for each item reference to add or update

*ppoRemoveReferences*
:   Array of [EdmItemRef](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef.html) structures; one structure for each item reference to remove

Adds and removes references to and from this item.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub UpdateReferences( _    ByRef ppoAddReferences() As EdmItemRef, _    ByRef ppoRemoveReferences() As EdmItemRef _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void UpdateReferences(     out EdmItemRef[] ppoAddReferences,    out EdmItemRef[] ppoRemoveReferences ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void UpdateReferences(  &   [Out] array<EdmItemRef>^ ppoAddReferences, &   [Out] array<EdmItemRef>^ ppoRemoveReferences ) ``` | |

#### Parameters

*ppoAddReferences*
:   Array of [EdmItemRef](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef.html) structures; one structure for each item reference to add or update

*ppoRemoveReferences*
:   Array of [EdmItemRef](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef.html) structures; one structure for each item reference to remove

# ![](dotnetimages/collapse.gif)Example

See the [IEdmItem](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

It is more efficient to use [IEdmBatchItemReferenceUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemReferenceUpdate.html), if you need to update the references of several items at the same time.

Note that the references in argument ppoRemoveReferences are deleted after references in ppoAddReferences are created or updated. A reference present in both lists is, therefore, updated and then immediately deleted.

See the [Programming Items](Items.htm) topic for more information.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmItem Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem.html)

[IEdmItem Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmItem_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010
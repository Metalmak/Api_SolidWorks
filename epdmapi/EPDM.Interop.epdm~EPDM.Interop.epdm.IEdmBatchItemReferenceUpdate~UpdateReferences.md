<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemReferenceUpdate~UpdateReferences.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| UpdateReferences Method (IEdmBatchItemReferenceUpdate) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchItemReferenceUpdate Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemReferenceUpdate.html) : UpdateReferences Method (IEdmBatchItemReferenceUpdate) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoAddReferences*
:   Array of [EdmItemRef](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef.html) structures; item references to add

*ppoRemoveReferences*
:   Array of [EdmItemRef](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef.html) structures; item references to remove

Adds or removes item references.

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
:   Array of [EdmItemRef](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef.html) structures; item references to add

*ppoRemoveReferences*
:   Array of [EdmItemRef](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef.html) structures; item references to remove

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchItemReferenceUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemReferenceUpdate.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchItemReferenceUpdate Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemReferenceUpdate.html)

[IEdmBatchItemReferenceUpdate Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemReferenceUpdate_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010
<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs2~AddReferencesID2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddReferencesID2 Method (IEdmAddCustomRefs2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddCustomRefs2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs2.html) : AddReferencesID2 Method (IEdmAddCustomRefs2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lRootFile*
:   ID of file to which to add file references

*ppoReferences*
:   Array of [EdmSelItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem.html)s containing file references to add to lRootFile

*plQuantity*
:   Array of times that the files in ppoReferences are referenced in lRootFile

Adds file references by ID and quantity.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddReferencesID2( _    ByVal lRootFile As System.Integer, _    ByRef ppoReferences() As EdmSelItem, _    ByRef plQuantity() As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddReferencesID2(     System.int lRootFile,    ref EdmSelItem[] ppoReferences,    ref System.int[] plQuantity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddReferencesID2(  &   System.int lRootFile, &   array<EdmSelItem>^% ppoReferences, &   System.array<int>^% plQuantity ) ``` | |

#### Parameters

*lRootFile*
:   ID of file to which to add file references

*ppoReferences*
:   Array of [EdmSelItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem.html)s containing file references to add to lRootFile

*plQuantity*
:   Array of times that the files in ppoReferences are referenced in lRootFile

# ![](dotnetimages/collapse.gif)Remarks

This method supersedes [IEdmAddCustomRefs::AddReferencesID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs~AddReferencesID.html), which adds reference files only by ID.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddCustomRefs2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs2.html)

[IEdmAddCustomRefs2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs2_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 2013 of SOLIDWORKS PDM Professional
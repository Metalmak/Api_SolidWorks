<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr~UpdateReferences.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| UpdateReferences Method (IEdmRawReferenceMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRawReferenceMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr.html) : UpdateReferences Method (IEdmRawReferenceMgr) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poReferences*
:   Array of [EdmRawReference](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference.html) structs of the references to update (see **Remarks**)

Updates the include paths for the file references.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub UpdateReferences( _    ByVal poReferences() As EdmRawReference _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void UpdateReferences(     EdmRawReference[] poReferences ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void UpdateReferences(  &   array<EdmRawReference>^ poReferences ) ``` | |

#### Parameters

*poReferences*
:   Array of [EdmRawReference](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference.html) structs of the references to update (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmRawReferenceMgr](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Use [IEdmRawReferenceMgr::GetReferences](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr~GetReferences.html) to get the array of EdmRawReference structs to pass to this method.

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRawReferenceMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr.html)

[IEdmRawReferenceMgr Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional
<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr~GetReferences.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetReferences Method (IEdmRawReferenceMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRawReferenceMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr.html) : GetReferences Method (IEdmRawReferenceMgr) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoReferences*
:   Array of [EdmRawReference](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference.html) structs of the file references

Get a list of all of the file references in the opened file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetReferences( _    ByRef ppoReferences() As EdmRawReference _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetReferences(     out EdmRawReference[] ppoReferences ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetReferences(  &   [Out] array<EdmRawReference>^ ppoReferences ) ``` | |

#### Parameters

*ppoReferences*
:   Array of [EdmRawReference](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference.html) structs of the file references

# ![](dotnetimages/collapse.gif)Example

See the [IEdmRawReferenceMgr](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must call [IEdmRawReferenceMgr::Open](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr~Open.html).

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRawReferenceMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr.html)

[IEdmRawReferenceMgr Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr_members.html)

[IEdmRawReferenceMgr::UpdateReferences Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr~UpdateReferences.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional
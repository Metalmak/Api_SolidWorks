<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3~AddSWBom.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddSWBom Method (IEdmBomMgr3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomMgr3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3.html) : AddSWBom Method (IEdmBomMgr3) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lDocumentID*
:   ID of document

*lProjectID*
:   ID of project where document resides

*lDocRevNr*
:   Version number of document

*poSWBom*
:   [IEdmSWBom](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom.html)

Adds the specified SOLIDWORKS BOM to the specified document.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddSWBom( _    ByVal lDocumentID As System.Integer, _    ByVal lProjectID As System.Integer, _    ByVal lDocRevNr As System.Integer, _    ByVal poSWBom As EdmSWBom _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddSWBom(     System.int lDocumentID,    System.int lProjectID,    System.int lDocRevNr,    EdmSWBom poSWBom ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddSWBom(  &   System.int lDocumentID, &   System.int lProjectID, &   System.int lDocRevNr, &   EdmSWBom^ poSWBom ) ``` | |

#### Parameters

*lDocumentID*
:   ID of document

*lProjectID*
:   ID of project where document resides

*lDocRevNr*
:   Version number of document

*poSWBom*
:   [IEdmSWBom](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBomMgr3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomMgr3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3.html)

[IEdmBomMgr3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2021 SP03
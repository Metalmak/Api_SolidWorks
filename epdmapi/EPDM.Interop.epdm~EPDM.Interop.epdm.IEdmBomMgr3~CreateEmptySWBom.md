<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3~CreateEmptySWBom.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateEmptySWBom Method (IEdmBomMgr3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomMgr3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3.html) : CreateEmptySWBom Method (IEdmBomMgr3) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Creates an empty SOLIDWORKS BOM.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateEmptySWBom() As EdmSWBom ``` | |

| C# |  |
| --- | --- |
| ``` EdmSWBom CreateEmptySWBom() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmSWBom^ CreateEmptySWBom(); ``` | |

#### Return Value

[IEdmSWBom](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBom.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBomMgr3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, call [IEdmBomMgr3::AddSWBom](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3~AddSWBom.html) to add a new SOLIDWORKS BOM to an existing document.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomMgr3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3.html)

[IEdmBomMgr3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2021 SP03
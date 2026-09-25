<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2~CanSeeBomLayout.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CanSeeBomLayout Method (IEdmBomMgr2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomMgr2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2.html) : CanSeeBomLayout Method (IEdmBomMgr2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lLayoutId*
:   BOM layout ID

*lUserID*
:   User ID

Gets whether the specified BOM layout is visible to the specified user.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CanSeeBomLayout( _    ByVal lLayoutId As System.Integer, _    ByVal lUserID As System.Integer _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CanSeeBomLayout(     System.int lLayoutId,    System.int lUserID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CanSeeBomLayout(  &   System.int lLayoutId, &   System.int lUserID ) ``` | |

#### Parameters

*lLayoutId*
:   BOM layout ID

*lUserID*
:   User ID

#### Return Value

True if visible, false if not

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBomMgr2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomMgr2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2.html)

[IEdmBomMgr2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2020
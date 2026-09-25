<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBomColumn~Type.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Type Property (IEdmSWBomColumn) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSWBomColumn Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBomColumn.html) : Type Property (IEdmSWBomColumn) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets or sets the type of this BOM column.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Property Type As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int Type {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int Type {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

0 = Zone

1 = Revision

2 = Description

3 = Date

4 = Approved

5 = User

6 = Configuration quantity

7 = Item number

8 = Part number

-1 = Type not found

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBomMgr3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr3.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSWBomColumn Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBomColumn.html)

[IEdmSWBomColumn Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSWBomColumn_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2021 SP03
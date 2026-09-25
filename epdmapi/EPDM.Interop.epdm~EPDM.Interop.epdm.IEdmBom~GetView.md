<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom~GetView.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetView Method (IEdmBom) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom.html) : GetView Method (IEdmBom) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lVersionNo*
:   Version of the BOM whose view you want

Gets the BOM view for the specified BOM version. The BOM view allows you to read and manipulate the contents of the BOM.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetView( _    Optional ByVal lVersionNo As System.Integer _ ) As EdmBomView ``` | |

| C# |  |
| --- | --- |
| ``` EdmBomView GetView(     System.int lVersionNo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmBomView^ GetView(  &   System.int lVersionNo ) ``` | |

#### Parameters

*lVersionNo*
:   Version of the BOM whose view you want

#### Return Value

[IEdmBomView](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView.html)

# ![](dotnetimages/collapse.gif)Example

[Add Row to Bill of Materials (VB.NET)](Add_Row_to_Bill_of_Materials_Example_VBNET.htm)

[Add Row to Bill of Materials (C#)](Add_Row_to_Bill_of_Materials_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom.html)

[IEdmBom Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009
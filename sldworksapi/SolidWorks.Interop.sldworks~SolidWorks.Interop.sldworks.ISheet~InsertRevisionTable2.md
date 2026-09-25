<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~InsertRevisionTable2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertRevisionTable2 Method (ISheet) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html) : InsertRevisionTable2 Method (ISheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseAnchorPoint*
:   True to insert the revision table at the existing revision table anchor point, false to anchor the table at the point specified by X and Y

*X*
:   X coordinate for the placement of the revision table annotation

*Y*
:   Y coordinate for the placement of this revision table annotation

*AnchorType*
:   Anchor type as defined by swBOMConfigurationAnchorType\_e

*TableTemplate*
:   Path and filename of the template that corresponds to this type of table (see **Remarks**)

*Shape*
:   Revision symbol shape as defined in swRevisionTableSymbolShape\_e

*AutoUpdateZoomCells*
:   True to automatically update zone cells, false to not

Inserts a revision table in this drawing sheet.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertRevisionTable2( _    ByVal UseAnchorPoint As System.Boolean, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal AnchorType As System.Integer, _    ByVal TableTemplate As System.String, _    ByVal Shape As System.Integer, _    ByVal AutoUpdateZoomCells As System.Boolean _ ) As RevisionTableAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheet Dim UseAnchorPoint As System.Boolean Dim X As System.Double Dim Y As System.Double Dim AnchorType As System.Integer Dim TableTemplate As System.String Dim Shape As System.Integer Dim AutoUpdateZoomCells As System.Boolean Dim value As RevisionTableAnnotation   value = instance.InsertRevisionTable2(UseAnchorPoint, X, Y, AnchorType, TableTemplate, Shape, AutoUpdateZoomCells) ``` | |

| C# |  |
| --- | --- |
| ``` RevisionTableAnnotation InsertRevisionTable2(     System.bool UseAnchorPoint,    System.double X,    System.double Y,    System.int AnchorType,    System.string TableTemplate,    System.int Shape,    System.bool AutoUpdateZoomCells ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` RevisionTableAnnotation^ InsertRevisionTable2(  &   System.bool UseAnchorPoint, &   System.double X, &   System.double Y, &   System.int AnchorType, &   System.String^ TableTemplate, &   System.int Shape, &   System.bool AutoUpdateZoomCells ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseAnchorPoint*
:   True to insert the revision table at the existing revision table anchor point, false to anchor the table at the point specified by X and Y

*X*
:   X coordinate for the placement of the revision table annotation

*Y*
:   Y coordinate for the placement of this revision table annotation

*AnchorType*
:   Anchor type as defined by swBOMConfigurationAnchorType\_e

*TableTemplate*
:   Path and filename of the template that corresponds to this type of table (see **Remarks**)

*Shape*
:   Revision symbol shape as defined in swRevisionTableSymbolShape\_e

*AutoUpdateZoomCells*
:   True to automatically update zone cells, false to not

#### Return Value

[Revision table](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionTableAnnotation.html) or null if a revision table already exists

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sheet::InsertRevisionTable2.

# ![](dotnetimages/collapse.gif)Example

[Create Drawing Sheet Zones (VBA)](Create_Drawing_Sheet_Zones_Example_VB.htm)

[Create Drawing Sheet Zones (VB.NET)](Create_Drawing_Sheet_Zones_Example_VBNET.htm)

[Create Drawing Sheet Zones (C#)](Create_Drawing_Sheet_Zones_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

By default, the revision table templates are in install\_dir\lang\language and have a filename extension of .sldrevtbt. The template and table must be of the same type. For example, you must specify TableTemplate with *install\_dir*\lang\English\standard revision block.sldrevtbt if you want to insert the English version of a revision block table.

# ![](dotnetimages/collapse.gif)See Also

####

[ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html)

[ISheet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet_members.html)

[ISheet::RevisionTable Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~RevisionTable.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0
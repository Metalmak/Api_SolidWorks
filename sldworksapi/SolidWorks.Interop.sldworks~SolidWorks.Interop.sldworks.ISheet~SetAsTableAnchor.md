<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SetAsTableAnchor.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetAsTableAnchor Method (ISheet) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html) : SetAsTableAnchor Method (ISheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TableType*
:   Table for which an anchor is required as defined in swTableAnnotationType\_e

Sets the anchor for the specified table at a selected point in the sheet format.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetAsTableAnchor( _    ByVal TableType As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheet Dim TableType As System.Integer Dim value As System.Object   value = instance.SetAsTableAnchor(TableType) ``` | |

| C# |  |
| --- | --- |
| ``` System.object SetAsTableAnchor(     System.int TableType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ SetAsTableAnchor(  &   System.int TableType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TableType*
:   Table for which an anchor is required as defined in swTableAnnotationType\_e

#### Return Value

[ITableAnchor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnchor.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sheet::SetAsTableAnchor.

# ![](dotnetimages/collapse.gif)Example

[Set Table Anchors in Sheet Formats (VBA)](Set_Table_Anchors_Example_VB.htm)

[Set Table Anchors in Sheet Formats (VB.NET)](Set_Table_Anchors_Example_VBNET.htm)

[Set Table Anchors in Sheet Formats (C#)](Set_Table_Anchors_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must call:

1. [IDrawingDoc::EditTemplate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~EditTemplate.html) to edit the sheet format.- [IModelDoc2::EditSketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditSketch.html) to create a sketch.- [ISketchManager::CreatePoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreatePoint.html) to create a sketch point where to position the table anchor.

If an anchor already exists for the table, then this method moves the anchor of that table to the selected position.

After calling this method you must call:

1. [IDrawingDoc::EditSheet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~EditSheet.html)- IModelDoc2::EditSketch- [IModelDoc2::ForceRebuild3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ForceRebuild3.html)

# ![](dotnetimages/collapse.gif)See Also

####

[ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html)

[ISheet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet_members.html)

[ISheet::TableAnchor Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~TableAnchor.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0
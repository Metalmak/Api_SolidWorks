<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~InsertRevisionTable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertRevisionTable Method (ISheet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html) : InsertRevisionTable Method (ISheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseAnchorPoint*
:   If true and the appropriate sheet format anchor point exists, then insert table at this point; if false, then use the values specified for the X and Y arguments as the insertion point

*X*
:   X coordinate for the placement of the revision table annotation

*Y*
:   Y coordinate for the placement of this revision table annotation

*AnchorType*
:   Anchor type as defined by swBOMConfigurationAnchorType\_e

*TableTemplate*
:   Path and filename of the template that you want to use that corresponds to this type of table (see **Remarks**)

Obsolete. Superseded by [ISheet::InsertRevisionTable2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~InsertRevisionTable2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertRevisionTable( _    ByVal UseAnchorPoint As System.Boolean, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal AnchorType As System.Integer, _    ByVal TableTemplate As System.String _ ) As RevisionTableAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheet Dim UseAnchorPoint As System.Boolean Dim X As System.Double Dim Y As System.Double Dim AnchorType As System.Integer Dim TableTemplate As System.String Dim value As RevisionTableAnnotation   value = instance.InsertRevisionTable(UseAnchorPoint, X, Y, AnchorType, TableTemplate) ``` | |

| C# |  |
| --- | --- |
| ``` RevisionTableAnnotation InsertRevisionTable(     System.bool UseAnchorPoint,    System.double X,    System.double Y,    System.int AnchorType,    System.string TableTemplate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` RevisionTableAnnotation^ InsertRevisionTable(  &   System.bool UseAnchorPoint, &   System.double X, &   System.double Y, &   System.int AnchorType, &   System.String^ TableTemplate ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseAnchorPoint*
:   If true and the appropriate sheet format anchor point exists, then insert table at this point; if false, then use the values specified for the X and Y arguments as the insertion point

*X*
:   X coordinate for the placement of the revision table annotation

*Y*
:   Y coordinate for the placement of this revision table annotation

*AnchorType*
:   Anchor type as defined by swBOMConfigurationAnchorType\_e

*TableTemplate*
:   Path and filename of the template that you want to use that corresponds to this type of table (see **Remarks**)

#### Return Value

[Revision table](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionTableAnnotation.html) or null if a revision table on the sheet already exists

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sheet::InsertRevisionTable.

# ![](dotnetimages/collapse.gif)Remarks

By default, the revision table templates are in the <install\_dir>\lang\<language> folder and have a filename extension of .sldrevtbt. The template and table must be of the same type. For example, you would specify C:\Program Files\SOLIDWORKS\lang\English\standard revision block.sldrevtbt for TableTemplate if you wanted to insert an English-version of the revision block table template.

# ![](dotnetimages/collapse.gif)See Also

####

[ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html)

[ISheet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet_members.html)

[ISheet::RevisionTable Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~RevisionTable.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0
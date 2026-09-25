<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertBomTable3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertBomTable3 Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : InsertBomTable3 Method (IView) |

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
:   X coordinate for the placement of the BOM table

*Y*
:   Y coordinate for the placement of the BOM table

*AnchorType*
:   Anchor type as defined by swBomConfigurationAnchorType\_e

*BomType*
:   Type of BOM table as defined by swBomType\_e

*Configuration*
:   Name of the configuration for this BOM table (see Remarks)

*TableTemplate*
:   Path and filename of the template that you want to use that corresponds to this type of table (see Remarks)

*Hidden*
:   True to hide the BOM table, false to show it

Obsolete. Superseded by [IView::InsertBomTable4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~InsertBomTable4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertBomTable3( _    ByVal UseAnchorPoint As System.Boolean, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal AnchorType As System.Integer, _    ByVal BomType As System.Integer, _    ByVal Configuration As System.String, _    ByVal TableTemplate As System.String, _    ByVal Hidden As System.Boolean _ ) As BomTableAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim UseAnchorPoint As System.Boolean Dim X As System.Double Dim Y As System.Double Dim AnchorType As System.Integer Dim BomType As System.Integer Dim Configuration As System.String Dim TableTemplate As System.String Dim Hidden As System.Boolean Dim value As BomTableAnnotation   value = instance.InsertBomTable3(UseAnchorPoint, X, Y, AnchorType, BomType, Configuration, TableTemplate, Hidden) ``` | |

| C# |  |
| --- | --- |
| ``` BomTableAnnotation InsertBomTable3(     System.bool UseAnchorPoint,    System.double X,    System.double Y,    System.int AnchorType,    System.int BomType,    System.string Configuration,    System.string TableTemplate,    System.bool Hidden ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` BomTableAnnotation^ InsertBomTable3(  &   System.bool UseAnchorPoint, &   System.double X, &   System.double Y, &   System.int AnchorType, &   System.int BomType, &   System.String^ Configuration, &   System.String^ TableTemplate, &   System.bool Hidden ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseAnchorPoint*
:   If true and the appropriate sheet format anchor point exists, then insert table at this point; if false, then use the values specified for the X and Y arguments as the insertion point

*X*
:   X coordinate for the placement of the BOM table

*Y*
:   Y coordinate for the placement of the BOM table

*AnchorType*
:   Anchor type as defined by swBomConfigurationAnchorType\_e

*BomType*
:   Type of BOM table as defined by swBomType\_e

*Configuration*
:   Name of the configuration for this BOM table (see Remarks)

*TableTemplate*
:   Path and filename of the template that you want to use that corresponds to this type of table (see Remarks)

*Hidden*
:   True to hide the BOM table, false to show it

#### Return Value

[BOM table annotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableAnnotation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::InsertBomTable3.

# ![](dotnetimages/collapse.gif)Remarks

If BomType is swBomType\_TopLevelOnly, then do not specify Configuration. Instead, use [IBomFeature::GetConfigurations](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomFeature~GetConfigurations.html) or [IBomFeature::IGetConfigurations](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomFeature~IGetConfigurations.html) and [IBomFeature::SetConfigurations](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomFeature~SetConfigurations.html) or [IBomFeature::ISetConfigurations](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomFeature~ISetConfigurations.html) to work with configurations in BOM tables.

If the drawing was created using a configuration other than the Default configuration, then the configuration active at the time the drawing was created is the configuration used in the BOM table when an empty string is specified for the Configuration parameter.

BOM table templates are in the install\_dir\lang\<language> folder and have a filename extension of .sldbomtbt. The template and table must be of the same type. For example, you could specify C:\Program Files\SOLIDWORKS\lang\English\bom-standard.sldbomtbt for TableTemplate if you wanted to insert an English-version of the standard BOM table template.

If the BOM table is a parts-only or indented-style BOM and the Configuration specified is invalid, then the BOM is not created.

NOTE: Use [IView::InsertBomTable](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~InsertBomTable.html) or [IView::IInsertBomTable](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IInsertBomTable.html) to insert a BOM using Microsoft Excel.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetKeepLinkedToBOM Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetKeepLinkedToBOM.html)

[IView::GetKeepLinkedToBOMName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetKeepLinkedToBOMName.html)

[IView::SetKeepLinkedToBOM Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~SetKeepLinkedToBOM.html)

[IModelDocExtension::InsertBomTable2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertBomTable2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision 18.0
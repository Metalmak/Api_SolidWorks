<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertGeneralTableAnnotation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertGeneralTableAnnotation Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : InsertGeneralTableAnnotation Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseAnchorPoint*
:   True to anchor the table by AnchorType and ignore any coordinates specified by X and Y, false to use the coordinates specified by X and Y

*X*
:   X coordinate of this table annotation

*Y*
:   Y coordinate of this table annotation

*AnchorType*
:   Type of anchor as defined in swBOMConfigurationAnchorType\_e; valid only if UseAnchorPoint is true and TableTemplate is empty (see **Remarks**)

*TableTemplate*
:   Path and file name of the general table template to use (see Remarks)

*Rows*
:   Number of rows in the table annotation; valid only if TableTemplate is empty (see **Remarks**)

*Columns*
:   Number of columns in the table annotation; valid only if TableTemplate is empty (see **Remarks**)

Inserts the a general table annotation in this model document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertGeneralTableAnnotation( _    ByVal UseAnchorPoint As System.Boolean, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal AnchorType As System.Integer, _    ByVal TableTemplate As System.String, _    ByVal Rows As System.Integer, _    ByVal Columns As System.Integer _ ) As TableAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim UseAnchorPoint As System.Boolean Dim X As System.Double Dim Y As System.Double Dim AnchorType As System.Integer Dim TableTemplate As System.String Dim Rows As System.Integer Dim Columns As System.Integer Dim value As TableAnnotation   value = instance.InsertGeneralTableAnnotation(UseAnchorPoint, X, Y, AnchorType, TableTemplate, Rows, Columns) ``` | |

| C# |  |
| --- | --- |
| ``` TableAnnotation InsertGeneralTableAnnotation(     System.bool UseAnchorPoint,    System.double X,    System.double Y,    System.int AnchorType,    System.string TableTemplate,    System.int Rows,    System.int Columns ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` TableAnnotation^ InsertGeneralTableAnnotation(  &   System.bool UseAnchorPoint, &   System.double X, &   System.double Y, &   System.int AnchorType, &   System.String^ TableTemplate, &   System.int Rows, &   System.int Columns ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseAnchorPoint*
:   True to anchor the table by AnchorType and ignore any coordinates specified by X and Y, false to use the coordinates specified by X and Y

*X*
:   X coordinate of this table annotation

*Y*
:   Y coordinate of this table annotation

*AnchorType*
:   Type of anchor as defined in swBOMConfigurationAnchorType\_e; valid only if UseAnchorPoint is true and TableTemplate is empty (see **Remarks**)

*TableTemplate*
:   Path and file name of the general table template to use (see Remarks)

*Rows*
:   Number of rows in the table annotation; valid only if TableTemplate is empty (see **Remarks**)

*Columns*
:   Number of columns in the table annotation; valid only if TableTemplate is empty (see **Remarks**)

#### Return Value

[ITableAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::InsertGeneralTableAnnotation.

# ![](dotnetimages/collapse.gif)Example

[Insert General Table in Part (VBA)](Insert_General_Table_in_Part_Example_VB.htm)

[Insert General Table in Part (VB.NET)](Insert_General_Table_in_Part_Example_VBNET.htm)

[Insert General Table in Part (C#)](Insert_General_Table_in_Part_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **If TableTemplate is...** | **Then..** |
| A valid path and file name | AnchorType, Rows, and Columns are ignored, and a general table based on TableTemplate is inserted |
| Empty | General table based only on all of the specified parameters, except TableTemplate, is inserted |

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IDrawingDoc::InsertTableAnnotation2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertTableAnnotation2.html)

[IModelDocExtension::InsertBomTable3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertBomTable3.html)

[IModelDocExtension::InsertTitleBlockTable Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertTitleBlockTable.html)

[IModelDocExtension::GetGeneralTableAnnotation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetGeneralTableAnnotation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0
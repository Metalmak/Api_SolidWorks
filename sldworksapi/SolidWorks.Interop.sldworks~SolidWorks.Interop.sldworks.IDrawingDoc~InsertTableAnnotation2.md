<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertTableAnnotation2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertTableAnnotation2 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : InsertTableAnnotation2 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseAnchorPoint*
:   True to anchor the table to the general table anchor point and ignore any coordinates specified for X and Y, or false to use the coordinates specified for X and Y

*X*
:   X coordinate to insert this table annotation

*Y*
:   Y coordinate to insert this table annotation

*AnchorType*
:   Type of anchor as defined in swBOMConfigurationAnchorType\_e (see **Remarks**)

*TableTemplate*
:   Path and filename of the general table template to use  (see Remarks)

*Rows*
:   Number of rows in the table annotation

*Columns*
:   Number of columns in the table annotation

Inserts a table annotation in this drawing.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertTableAnnotation2( _    ByVal UseAnchorPoint As System.Boolean, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal AnchorType As System.Integer, _    ByVal TableTemplate As System.String, _    ByVal Rows As System.Integer, _    ByVal Columns As System.Integer _ ) As TableAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim UseAnchorPoint As System.Boolean Dim X As System.Double Dim Y As System.Double Dim AnchorType As System.Integer Dim TableTemplate As System.String Dim Rows As System.Integer Dim Columns As System.Integer Dim value As TableAnnotation   value = instance.InsertTableAnnotation2(UseAnchorPoint, X, Y, AnchorType, TableTemplate, Rows, Columns) ``` | |

| C# |  |
| --- | --- |
| ``` TableAnnotation InsertTableAnnotation2(     System.bool UseAnchorPoint,    System.double X,    System.double Y,    System.int AnchorType,    System.string TableTemplate,    System.int Rows,    System.int Columns ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` TableAnnotation^ InsertTableAnnotation2(  &   System.bool UseAnchorPoint, &   System.double X, &   System.double Y, &   System.int AnchorType, &   System.String^ TableTemplate, &   System.int Rows, &   System.int Columns ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseAnchorPoint*
:   True to anchor the table to the general table anchor point and ignore any coordinates specified for X and Y, or false to use the coordinates specified for X and Y

*X*
:   X coordinate to insert this table annotation

*Y*
:   Y coordinate to insert this table annotation

*AnchorType*
:   Type of anchor as defined in swBOMConfigurationAnchorType\_e (see **Remarks**)

*TableTemplate*
:   Path and filename of the general table template to use  (see Remarks)

*Rows*
:   Number of rows in the table annotation

*Columns*
:   Number of columns in the table annotation

#### Return Value

Pointer to the [ITableAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITableAnnotation.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::InsertTableAnnotation2.

# ![](dotnetimages/collapse.gif)Example

[Insert General Table (VBA)](Insert_General_Table_Example_VB.htm)

[Get General Table Feature (C#)](Get_General_Table_Feature_Example_CSharp.htm)

[Get General Table Feature (VB.NET)](Get_General_Table_Feature_Example_VBNET.htm)

[Get General Table Feature (VBA)](Get_General_Table_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **If TableTemplate is...** | **Then..** |
| A valid path and filename | AnchorType and Columns are ignored, and the information from the table template is used instead |
| Empty | General table is inserted based only on the other input arguments |

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IModelDocExtension::InsertGeneralTableAnnotation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertGeneralTableAnnotation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0
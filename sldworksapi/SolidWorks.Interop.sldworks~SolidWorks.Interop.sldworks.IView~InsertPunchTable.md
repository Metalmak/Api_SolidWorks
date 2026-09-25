<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertPunchTable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertPunchTable Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : InsertPunchTable Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseAnchorPoint*
:   If true, and the sheet format anchor point exists, then insert table at the anchor point; if false, then insert the table at the location specified by the X and Y parameters

*X*
:   X coordinate for the anchor of this punch table

*Y*
:   Y coordinate for the anchor of this punch table

*AnchorType*
:   Anchor type as defined by swBomConfigurationAnchorType\_e

*StartValue*
:   Starting value for datum tags; a letter from A to Z, if TableTemplate uses letter tags; a positive integer, if TableTemplate uses number tags (see **Remarks**)

*TableTemplate*
:   Path and filename of the table template that corresponds to the type of table you want to use (see Remarks)

Inserts a punch table in the flat pattern drawing view of a sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertPunchTable( _    ByVal UseAnchorPoint As System.Boolean, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal AnchorType As System.Integer, _    ByVal StartValue As System.String, _    ByVal TableTemplate As System.String _ ) As PunchTableAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim UseAnchorPoint As System.Boolean Dim X As System.Double Dim Y As System.Double Dim AnchorType As System.Integer Dim StartValue As System.String Dim TableTemplate As System.String Dim value As PunchTableAnnotation   value = instance.InsertPunchTable(UseAnchorPoint, X, Y, AnchorType, StartValue, TableTemplate) ``` | |

| C# |  |
| --- | --- |
| ``` PunchTableAnnotation InsertPunchTable(     System.bool UseAnchorPoint,    System.double X,    System.double Y,    System.int AnchorType,    System.string StartValue,    System.string TableTemplate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` PunchTableAnnotation^ InsertPunchTable(  &   System.bool UseAnchorPoint, &   System.double X, &   System.double Y, &   System.int AnchorType, &   System.String^ StartValue, &   System.String^ TableTemplate ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseAnchorPoint*
:   If true, and the sheet format anchor point exists, then insert table at the anchor point; if false, then insert the table at the location specified by the X and Y parameters

*X*
:   X coordinate for the anchor of this punch table

*Y*
:   Y coordinate for the anchor of this punch table

*AnchorType*
:   Anchor type as defined by swBomConfigurationAnchorType\_e

*StartValue*
:   Starting value for datum tags; a letter from A to Z, if TableTemplate uses letter tags; a positive integer, if TableTemplate uses number tags (see **Remarks**)

*TableTemplate*
:   Path and filename of the table template that corresponds to the type of table you want to use (see Remarks)

#### Return Value

[IPunchTableAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPunchTableAnnotation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::InsertPunchTable.

# ![](dotnetimages/collapse.gif)Example

[Insert Punch Table (VBA)](Insert_Punch_Table_Example_VB.htm)

[Insert Punch Table (VB.NET)](Insert_Punch_Table_Example_VBNET.htm)

[Insert Punch Table (C#)](Insert_Punch_Table_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Punch tables contain information about the punches that are created by forming tools in sheet metal parts. This method inserts a punch table with the following information for pre-selected punches:

| Column | Description |
| --- | --- |
| TAG | Datum tag added to each punch in the flat pattern view |
| PUNCH ID | Property of the forming tool or library feature |
| X Location | Distance from the x-axis to the point of insertion of the forming tool in the flat pattern view |
| Y Location | Distance from the y-axis to the point of insertion of the forming tool in the flat pattern view |
| ANGLE | Angle between the x-axis and the forming tool |
| QUANTITY | Number of times that the punch occurs in the flat pattern view |

The locations of the datum tags are relative to a datum origin that is pre-selected in the view.

Before calling this method, call [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select the datum origin, punch edges, and punch faces (for multiple punches) as follows:

| **Selection** | **Mark** |
| --- | --- |
| Datum origin vertex | 1 |
| Punch edges and faces | 2 |
| Datum origin x-axis direction reference | 4 |
| Datum origin y-axis direction reference | 8 |

Specify TableTemplate using a punch table template (**\*.sldpuntbt**) in install\_dir\lang\*language*.

Specify a StartValue that matches the table you want to create. For example, to insert a punch table with letter tags, specify a StartValue with a letter from A to Z.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IPunchTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPunchTable.html)

[IFeatureManager::InsertFormToolFeature Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertFormToolFeature.html)

[IFeatureManager::CreateFormTool Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFormTool.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0
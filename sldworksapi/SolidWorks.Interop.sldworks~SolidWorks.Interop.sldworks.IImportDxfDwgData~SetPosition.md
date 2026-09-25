<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetPosition Method (IImportDxfDwgData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html) : SetPosition Method (IImportDxfDwgData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Sheet*
:   Sheet (layout) name of the input file or an empty string for all sheets

*Positioning*
:   Position as defined in swDwgImportEntitiesPositioning\_e

*X*
:   X coordinate of the origin of the imported drawing

*Y*
:   Y coordinate of the origin of the imported drawing

Sets the position of the entities created in the drawing.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPosition( _    ByVal Sheet As System.String, _    ByVal Positioning As System.Integer, _    ByVal X As System.Double, _    ByVal Y As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IImportDxfDwgData Dim Sheet As System.String Dim Positioning As System.Integer Dim X As System.Double Dim Y As System.Double Dim value As System.Boolean   value = instance.SetPosition(Sheet, Positioning, X, Y) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetPosition(     System.string Sheet,    System.int Positioning,    System.double X,    System.double Y ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetPosition(  &   System.String^ Sheet, &   System.int Positioning, &   System.double X, &   System.double Y ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Sheet*
:   Sheet (layout) name of the input file or an empty string for all sheets

*Positioning*
:   Position as defined in swDwgImportEntitiesPositioning\_e

*X*
:   X coordinate of the origin of the imported drawing

*Y*
:   Y coordinate of the origin of the imported drawing

#### Return Value

True if the position is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ImportDxfDwgData::SetPosition.

# ![](dotnetimages/collapse.gif)Example

[Insert and Position DXF/DWG File in Drawing (C#)](Insert_and_Position_DXF_File_in_Drawing_Example_CSharp.htm)

[Insert and Position DXF/DWG File in Drawing (VB.NET)](Insert_and_Position_DXF_File_in_Drawing_Example_VBNET.htm)

[Insert and Position DXF/DWG File in Drawing (VBA)](Insert_and_Position_DXF_File_in_Drawing_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method only supports importing to a drawing; it does not support importing to a part sketch.

# ![](dotnetimages/collapse.gif)See Also

####

[IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html)

[IImportDxfDwgData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData_members.html)

[IImportDxfDwgData::GetPosition Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetPosition.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetPaperSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetPaperSize Method (IImportDxfDwgData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html) : SetPaperSize Method (IImportDxfDwgData) |

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

*Size*
:   Size as defined in swDwgPaperSizes\_e

*Height*
:   If Size is swDwgPapersUserDefined, then the height of the paper in meters

*Width*
:   If Size is swDwgPapersUserDefined, then the width of the paper in meters

Sets the size of the paper in the drawing.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPaperSize( _    ByVal Sheet As System.String, _    ByVal Size As System.Integer, _    ByVal Height As System.Double, _    ByVal Width As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IImportDxfDwgData Dim Sheet As System.String Dim Size As System.Integer Dim Height As System.Double Dim Width As System.Double Dim value As System.Boolean   value = instance.SetPaperSize(Sheet, Size, Height, Width) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetPaperSize(     System.string Sheet,    System.int Size,    System.double Height,    System.double Width ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetPaperSize(  &   System.String^ Sheet, &   System.int Size, &   System.double Height, &   System.double Width ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Sheet*
:   Sheet (layout) name of the input file or an empty string for all sheets

*Size*
:   Size as defined in swDwgPaperSizes\_e

*Height*
:   If Size is swDwgPapersUserDefined, then the height of the paper in meters

*Width*
:   If Size is swDwgPapersUserDefined, then the width of the paper in meters

#### Return Value

True if paper size is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ImportDxfDwgData::SetPaperSize.

# ![](dotnetimages/collapse.gif)Example

[Import DXF File into Drawing (VBA)](Import_DXF_File_to_Drawing_Example_VB.htm)

[Insert and Position DXF/DWG File in Drawing (VBA)](Insert_and_Position_DXF_File_in_Drawing_Example_VB.htm)

[Insert and Position DXF/DWG File in Drawing (VB.NET)](Insert_and_Position_DXF_File_in_Drawing_Example_VBNET.htm)

[Insert and Position DXF/DWG File in Drawing (C#)](Insert_and_Position_DXF_File_in_Drawing_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method only supports importing to a drawing; it does not support importing to a part sketch.

# ![](dotnetimages/collapse.gif)See Also

####

[IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html)

[IImportDxfDwgData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData_members.html)

[IImportDxfDwgData::GetPaperSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetPaperSize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0
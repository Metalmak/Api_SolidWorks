<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~GetPaperSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetPaperSize Method (IImportDxfDwgData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html) : GetPaperSize Method (IImportDxfDwgData) |

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

Gets the size of the paper for the drawing.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetPaperSize( _    ByVal Sheet As System.String, _    ByRef Size As System.Integer, _    ByRef Height As System.Double, _    ByRef Width As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IImportDxfDwgData Dim Sheet As System.String Dim Size As System.Integer Dim Height As System.Double Dim Width As System.Double   instance.GetPaperSize(Sheet, Size, Height, Width) ``` | |

| C# |  |
| --- | --- |
| ``` void GetPaperSize(     System.string Sheet,    out System.int Size,    out System.double Height,    out System.double Width ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetPaperSize(  &   System.String^ Sheet, &   [Out] System.int Size, &   [Out] System.double Height, &   [Out] System.double Width ) ``` | |

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

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ImportDxfDwgData::GetPaperSize.

# ![](dotnetimages/collapse.gif)Remarks

This method only supports importing to a drawing; it does not support importing to a part sketch.

# ![](dotnetimages/collapse.gif)See Also

####

[IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html)

[IImportDxfDwgData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData_members.html)

[IImportDxfDwgData::SetPaperSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~SetPaperSize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0
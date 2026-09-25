<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData~ImportHatch.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ImportHatch Property (IImportDxfDwgData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html) : ImportHatch Property (IImportDxfDwgData) |

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

Gets or sets whether to import hatch into this part sketch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ImportHatch( _    ByVal Sheet As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IImportDxfDwgData Dim Sheet As System.String Dim value As System.Boolean   instance.ImportHatch(Sheet) = value   value = instance.ImportHatch(Sheet) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ImportHatch(     System.string Sheet ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool ImportHatch {    System.bool get(System.String^ Sheet);    void set (System.String^ Sheet, System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Sheet*
:   Sheet (layout) name of the input file or an empty string for all sheets

#### Property Value

True to import hatch, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ImportDxfDwgData::ImportHatch.

# ![](dotnetimages/collapse.gif)Example

[Import DXF File into Part Sketch (VBA)](Import_DXF_File_into_Part_Sketch_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This property only supports importing to a part sketch; it does not support importing to a drawing.

By default, hatch will be imported.

# ![](dotnetimages/collapse.gif)See Also

####

[IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html)

[IImportDxfDwgData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0
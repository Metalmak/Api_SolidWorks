<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertDimensionOption~DimensionPositionOption2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| DimensionPositionOption2 Property (IDimXpertDimensionOption) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertDimensionOption Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertDimensionOption.html) : DimensionPositionOption2 Property (IDimXpertDimensionOption) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets the reference axis with which to dimension the location of a face with respect to another locating feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property DimensionPositionOption2 As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertDimensionOption Dim value As System.Integer   instance.DimensionPositionOption2 = value   value = instance.DimensionPositionOption2 ``` | |

| C# |  |
| --- | --- |
| ``` System.int DimensionPositionOption2 {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int DimensionPositionOption2 {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Reference axis as defined in [swDimXpertDimensionPositionOption\_e](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.swDimXpertDimensionPositionOption_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertDimensionOption::DimensionPositionOption2.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Location Dimension (VBA)](Get_and_Set_Location_Dimension_Example_VB.htm)

[Get and Set Location Dimension (VB.NET)](Get_and_Set_Location_Dimension_Example_VBNET.htm)

[Get and Set Location Dimension (C#)](Get_and_Set_Location_Dimension_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertDimensionOption Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertDimensionOption.html)

[IDimXpertDimensionOption Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertDimensionOption_members.html)

[IDimXpertPart::InsertLocationDimension Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertLocationDimension.html)

[IDimXpertPart::InsertBasicDimension Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertBasicDimension.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0
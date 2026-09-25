<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertBasicDimension.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| InsertBasicDimension Method (IDimXpertPart) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertPart Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart.html) : InsertBasicDimension Method (IDimXpertPart) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Option*
:   [IDimXpertDimensionOption](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertDimensionOption.html)

Inserts a basic dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertBasicDimension( _    ByVal Option As DimXpertDimensionOption _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertPart Dim Option As DimXpertDimensionOption Dim value As System.Boolean   value = instance.InsertBasicDimension(Option) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertBasicDimension(     DimXpertDimensionOption Option ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertBasicDimension(  &   DimXpertDimensionOption^ Option ) ``` | |

#### Parameters

*Option*
:   [IDimXpertDimensionOption](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertDimensionOption.html)

#### Return Value

True if the basic dimension is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertPart::InsertBasicDimension.

# ![](dotnetimages/collapse.gif)Example

[Insert Basic Dimension (VBA)](Get_and_Set_Basic_Dimension_Example_VB.htm)

[Insert Basic Dimension (VB.NET)](Get_and_Set_Basic_Dimension_Example_VBNET.htm)

[Insert Basic Dimension (C#)](Get_and_Set_Basic_Dimension_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

A DimXpert basic dimension is the distance or angle between selected reference features.

Before calling this method:

1. Call [IDimXpertPart::GetDimOption](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertPart~GetDimOption.html) to get an instance of IDimXpertDimensionOption.- Set:
     * IDimXpertDimensionOption::TextPosition or [IDimXpertDimensionOption::DimensionPositionOption](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertDimensionOption~DimensionPositionOption.html) (if both are set, only DimensionPositionOption is in force) for distance-between dimensions.* [IDimXpertDimensionOption::TextPosition](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertDimensionOption~TextPosition.html) for angle-between dimensions.- Populate Option with the instance of IDimXpertDimensionOption.- Multi-select reference features using IModelDocExtension::SelectByID2:
         1. Origin feature (Append = false)- Tolerance feature (Append = true)

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertPart Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart.html)

[IDimXpertPart Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart_members.html)

[IDimXpertPart::InsertDatum Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertDatum.html)

[IDimXpertPart::InsertLocationDimension Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertLocationDimension.html)

[IDimXpertPart::InsertPattern Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertPattern.html)

[IDimXpertPart::InsertSizeDimension Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertSizeDimension.html)

[IDimXpertPart::AutoDimensionScheme Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~AutoDimensionScheme.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0
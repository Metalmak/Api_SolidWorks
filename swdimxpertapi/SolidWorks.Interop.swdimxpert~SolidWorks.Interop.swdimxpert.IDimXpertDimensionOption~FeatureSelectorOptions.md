<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertDimensionOption~FeatureSelectorOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| FeatureSelectorOptions Property (IDimXpertDimensionOption) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertDimensionOption Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertDimensionOption.html) : FeatureSelectorOptions Property (IDimXpertDimensionOption) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets the type of feature to dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property FeatureSelectorOptions As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertDimensionOption Dim value As System.Object   instance.FeatureSelectorOptions = value   value = instance.FeatureSelectorOptions ``` | |

| C# |  |
| --- | --- |
| ``` System.object FeatureSelectorOptions {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ FeatureSelectorOptions {    System.Object^ get();    void set ( &   System.Object^ value); } ``` | |

#### Property Value

Array of long values as defined in [swDimXpertFeatureSelectorOption\_e](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.swDimXpertFeatureSelectorOption_e.html); however, only the first element in the array is used; all of the other elements, if any, in the array are ignored

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertDimensionOption::FeatureSelectorOptions.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Pattern Example (C#)](Get_and_Set_Pattern_Example_CSharp.htm)

[Get and Set Pattern Example (VB.NET)](Get_and_Set_Pattern_Example_VBNET.htm)

[Get and Set Pattern Example (VBA)](Get_and_Set_Pattern_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use this property to set the type of feature to dimension. For example, if you select a hole face and you want that face to be dimensioned as a cylinder, then make [swDimXpertFeatureSelectorOption\_e.swDimXpertFeatureSelectorOption\_Cylinder](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.swDimXpertFeatureSelectorOption_e.html) the first element in the FeatureSelectorOptions array.

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertDimensionOption Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertDimensionOption.html)

[IDimXpertDimensionOption Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertDimensionOption_members.html)

[IDimXpertPart::InsertDatum Method](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertDatum.html)

[IDimXpertPart::InsertSizeDimension Method](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertSizeDimension.html)

[IDimXpertPart::InsertPattern Method](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertPattern.html)

[IDimXpertPart::InsertBasicDimension Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertBasicDimension.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0
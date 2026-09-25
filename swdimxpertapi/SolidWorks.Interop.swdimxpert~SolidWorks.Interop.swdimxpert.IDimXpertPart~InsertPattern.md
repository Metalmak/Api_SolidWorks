<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertPattern.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| InsertPattern Method (IDimXpertPart) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertPart Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart.html) : InsertPattern Method (IDimXpertPart) |

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

*PatternType*
:   0 = linked

    1 = manual

    2 = collection

*FindAll*
:   True to select similar faces for PatternTypes 1 and 2, false to not. (see **Remarks**)

Inserts a linked, manual, or collection pattern using the selected faces.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertPattern( _    ByVal Option As DimXpertDimensionOption, _    ByVal PatternType As System.Integer, _    ByVal FindAll As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertPart Dim Option As DimXpertDimensionOption Dim PatternType As System.Integer Dim FindAll As System.Boolean Dim value As System.Boolean   value = instance.InsertPattern(Option, PatternType, FindAll) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertPattern(     DimXpertDimensionOption Option,    System.int PatternType,    System.bool FindAll ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertPattern(  &   DimXpertDimensionOption^ Option, &   System.int PatternType, &   System.bool FindAll ) ``` | |

#### Parameters

*Option*
:   [IDimXpertDimensionOption](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertDimensionOption.html)

*PatternType*
:   0 = linked

    1 = manual

    2 = collection

*FindAll*
:   True to select similar faces for PatternTypes 1 and 2, false to not. (see **Remarks**)

#### Return Value

False

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertPart::InsertPattern.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Pattern (C#)](Get_and_Set_Pattern_Example_CSharp.htm)

[Get and Set Pattern (VB.NET)](Get_and_Set_Pattern_Example_VBNET.htm)

[Get and Set Pattern (VBA)](Get_and_Set_Pattern_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method:

1. Call [IDimXpertPart::GetDimOption](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertPart~GetDimOption.html) to get an instance of IDimXpertDimensionOption.- Set [IDimXpertDimensionOption::FeatureSelectorOptions](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertDimensionOption~FeatureSelectorOptions.html) to swDimXpertFeatureSelectorOption\_Default to enable the FindAll property. If IDimXpertDimensionOption::FeatureSelectorOptions is set to anything other than the default, the FindAll setting is not in force.)- Populate Option with the instance of IDimXpertDimensionOption.- Select the features according to PatternType:
         1. If PatternType is linked, then select one feature to automatically select all features of the pattern.- If PatternType is manual or collection and FindAll is set to true, then select one feature to automatically select all similar features on the face.- Set the selection mark for each selected feature to a unique value that is greater than 50.

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertPart Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart.html)

[IDimXpertPart Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart_members.html)

[IDimXpertPart::AutoDimensionScheme Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~AutoDimensionScheme.html)

[IDimXpertPart::InsertBasicDimension Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertBasicDimension.html)

[IDimXpertPart::InsertDatum Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertDatum.html)

[IDimXpertPart::InsertLocationDimension Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertLocationDimension.html)

[IDimXpertPart::InsertSizeDimension Method ()](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertSizeDimension.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0
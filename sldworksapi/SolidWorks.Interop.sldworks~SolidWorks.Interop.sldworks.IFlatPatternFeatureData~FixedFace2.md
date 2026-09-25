<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlatPatternFeatureData~FixedFace2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FixedFace2 Property (IFlatPatternFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFlatPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlatPatternFeatureData.html) : FixedFace2 Property (IFlatPatternFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the fixed face of this Flat-Pattern feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property FixedFace2 As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFlatPatternFeatureData Dim value As System.Object   instance.FixedFace2 = value   value = instance.FixedFace2 ``` | |

| C# |  |
| --- | --- |
| ``` System.object FixedFace2 {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ FixedFace2 {    System.Object^ get();    void set ( &   System.Object^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Fixed [face](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) (or [edge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html) for cylindrical sheet metal parts)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FlatPatternFeatureData::FixedFace2.

# ![](dotnetimages/collapse.gif)Example

[Get Fixed Face of Flat-Pattern Feature (VBA)](Get_Fixed_Face_of_Flat-Pattern_Feature_Example_VB.htm)

[Get Fixed Face of Flat-Pattern Feature (VB.NET)](Get_Fixed_Face_of_Flat-Pattern_Feature_Example_VBNET.htm)

[Get Fixed Face of Flat-Pattern Feature (C#)](Get_Fixed_Face_of_Flat-Pattern_Feature_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The difference between this method and the now obsolete IFlatPatternFeatureData::FixedFace is that this method successfully returns the fixed face of a Flat-Pattern feature in a sheet metal part created in any version of SOLIDWORKS.

See Accessing Selections that Define Features for additional details on using this property.

# ![](dotnetimages/collapse.gif)See Also

####

[IFlatPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlatPatternFeatureData.html)

[IFlatPatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlatPatternFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweptFlangeFeatureData~Path.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Path Property (ISweptFlangeFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISweptFlangeFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweptFlangeFeatureData.html) : Path Property (ISweptFlangeFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the sweep path of this swept flange feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Path As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISweptFlangeFeatureData Dim value As System.Object   instance.Path = value   value = instance.Path ``` | |

| C# |  |
| --- | --- |
| ``` System.object Path {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ Path {    System.Object^ get();    void set ( &   System.Object^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Array of [edge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html)s or a [sketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html) of lines and arcs

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SweptFlangeFeatureData::Path.

# ![](dotnetimages/collapse.gif)Example

See the [ISweptFlangeFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweptFlangeFeatureData.html) and [ISheetMetalGaugeTableParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalGaugeTableParameters.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

If the sweep path is a closed loop, then [ISweptFlangeFeatureData::StartOffset](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweptFlangeFeatureData~StartOffset.html) and [ISweptFlangeFeatureData::EndOffset](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweptFlangeFeatureData~EndOffset.html) are not valid.

# ![](dotnetimages/collapse.gif)See Also

####

[ISweptFlangeFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweptFlangeFeatureData.html)

[ISweptFlangeFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweptFlangeFeatureData_members.html)

[ISweptFlangeFeatureData::GetPathType Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweptFlangeFeatureData~GetPathType.html)

[ISweptFlangeFeatureData::CylindricalOrConicalEdge Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweptFlangeFeatureData~CylindricalOrConicalEdge.html)

[ISweptFlangeFeatureData::FlattenAlongPath Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweptFlangeFeatureData~FlattenAlongPath.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 FCS, Revision Number 29
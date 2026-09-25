<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~FeatureScope.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureScope Property (ISketchPatternFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData.html) : FeatureScope Property (ISketchPatternFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets which bodies in this multibody part are affected by this sketch-driven pattern feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property FeatureScope As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchPatternFeatureData Dim value As System.Boolean   value = instance.FeatureScope ``` | |

| C# |  |
| --- | --- |
| ``` System.bool FeatureScope {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool FeatureScope {    System.bool get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to specify affected bodies, false to apply the pattern to all bodies every time the feature regenerates

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchPatternFeatureData::FeatureScope.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [ISketchPatternFeatureData::GeometryPattern](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~GeometryPattern.html) is true.

Call [ISketchPatternFeatureData::SetFeatureScope](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData~SetFeatureScope.html) to set this property.

For more information, see the **Sketch Driven Patterns PropertyManager** topic in the SOLIDWORKS user-interface help.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData.html)

[ISketchPatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0
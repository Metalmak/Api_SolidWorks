<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFindReplaceAnnotations~AnnotationFilter.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| AnnotationFilter Property (IFindReplaceAnnotations) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IFindReplaceAnnotations Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFindReplaceAnnotations.html) : AnnotationFilter Property (IFindReplaceAnnotations) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the type of annotations to find.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property AnnotationFilter As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFindReplaceAnnotations Dim value As System.Integer   instance.AnnotationFilter = value   value = instance.AnnotationFilter ``` | |

| C# |  |
| --- | --- |
| ``` System.int AnnotationFilter {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int AnnotationFilter {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Type of annotations to find as defined by [gtFraFilterType\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtFraFilterType_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IFindReplaceAnnotations::AnnotationFilter.

# ![](dotnetimages/collapse.gif)See Also

####

[IFindReplaceAnnotations Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFindReplaceAnnotations.html)

[IFindReplaceAnnotations Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFindReplaceAnnotations_members.html)

[IFindReplaceAnnotations::FindNext Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFindReplaceAnnotations~FindNext.html)

[IFindReplaceAnnotations::FindPrevious Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFindReplaceAnnotations~FindPrevious.html)

[IFindReplaceAnnotations::FindText Property](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFindReplaceAnnotations~FindText.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2008 FCS
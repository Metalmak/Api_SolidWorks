<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~CreateCircularSketchStepAndRepeat.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateCircularSketchStepAndRepeat Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : CreateCircularSketchStepAndRepeat Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ArcRadius*

*ArcAngle*

*PatternNum*

*PatternSpacing*

*PatternRotate*

*DeleteInstances*

Obsolete. Superseded by [IModelDoc2::CreateCircularSketchStepAndRepeat](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~CreateCircularSketchStepAndRepeat.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateCircularSketchStepAndRepeat( _    ByVal ArcRadius As System.Double, _    ByVal ArcAngle As System.Double, _    ByVal PatternNum As System.Integer, _    ByVal PatternSpacing As System.Double, _    ByVal PatternRotate As System.Boolean, _    ByVal DeleteInstances As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim ArcRadius As System.Double Dim ArcAngle As System.Double Dim PatternNum As System.Integer Dim PatternSpacing As System.Double Dim PatternRotate As System.Boolean Dim DeleteInstances As System.String Dim value As System.Boolean   value = instance.CreateCircularSketchStepAndRepeat(ArcRadius, ArcAngle, PatternNum, PatternSpacing, PatternRotate, DeleteInstances) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateCircularSketchStepAndRepeat(     System.double ArcRadius,    System.double ArcAngle,    System.int PatternNum,    System.double PatternSpacing,    System.bool PatternRotate,    System.string DeleteInstances ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateCircularSketchStepAndRepeat(  &   System.double ArcRadius, &   System.double ArcAngle, &   System.int PatternNum, &   System.double PatternSpacing, &   System.bool PatternRotate, &   System.String^ DeleteInstances ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ArcRadius*

*ArcAngle*

*PatternNum*

*PatternSpacing*

*PatternRotate*

*DeleteInstances*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::CreateCircularSketchStepAndRepeat.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)
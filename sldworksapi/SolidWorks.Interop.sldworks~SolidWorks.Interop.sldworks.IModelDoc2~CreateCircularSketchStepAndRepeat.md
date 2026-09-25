<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateCircularSketchStepAndRepeat.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateCircularSketchStepAndRepeat Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : CreateCircularSketchStepAndRepeat Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ArcRadius*
:   Radius to be used in the circular sketch pattern

*ArcAngle*
:   Angle relative to the sketch entities being patterned

*PatternNum*
:   Total number of instances, including the seed geometry

*PatternSpacing*
:   Spacing between pattern instances in radians

*PatternRotate*
:   True to rotate the pattern, false to not

*DeleteInstances*
:   Number of instances to delete passed as a string formatted as: "(a) (b) (c) "

Obsolete. Superseded by [ISketchManager::CreateCircularSketchStepAndRepeat](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~CreateCircularSketchStepAndRepeat.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateCircularSketchStepAndRepeat( _    ByVal ArcRadius As System.Double, _    ByVal ArcAngle As System.Double, _    ByVal PatternNum As System.Integer, _    ByVal PatternSpacing As System.Double, _    ByVal PatternRotate As System.Boolean, _    ByVal DeleteInstances As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim ArcRadius As System.Double Dim ArcAngle As System.Double Dim PatternNum As System.Integer Dim PatternSpacing As System.Double Dim PatternRotate As System.Boolean Dim DeleteInstances As System.String Dim value As System.Boolean   value = instance.CreateCircularSketchStepAndRepeat(ArcRadius, ArcAngle, PatternNum, PatternSpacing, PatternRotate, DeleteInstances) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateCircularSketchStepAndRepeat(     System.double ArcRadius,    System.double ArcAngle,    System.int PatternNum,    System.double PatternSpacing,    System.bool PatternRotate,    System.string DeleteInstances ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateCircularSketchStepAndRepeat(  &   System.double ArcRadius, &   System.double ArcAngle, &   System.int PatternNum, &   System.double PatternSpacing, &   System.bool PatternRotate, &   System.String^ DeleteInstances ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ArcRadius*
:   Radius to be used in the circular sketch pattern

*ArcAngle*
:   Angle relative to the sketch entities being patterned

*PatternNum*
:   Total number of instances, including the seed geometry

*PatternSpacing*
:   Spacing between pattern instances in radians

*PatternRotate*
:   True to rotate the pattern, false to not

*DeleteInstances*
:   Number of instances to delete passed as a string formatted as: "(a) (b) (c) "

#### Return Value

True if the sketch pattern was created successfully, false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::CreateCircularSketchStepAndRepeat.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::CreateLinearSketchStepAndRepeat Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateLinearSketchStepAndRepeat.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0
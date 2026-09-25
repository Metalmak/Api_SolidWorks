<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IInsertSheetMetalEdgeFlange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IInsertSheetMetalEdgeFlange Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : IInsertSheetMetalEdgeFlange Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FlangeEdge*

*SketchFeat*

*BooleanOptions*

*DAngle*

*DRadius*

*BendPosition*

*DOffsetDist*

*ReliefType*

*DReliefRatio*

*DReliefWidth*

*DReliefDepth*

Obsolete. Superseded by [IFeatureManager::InsertSheetMetalEdgeFlange2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertSheetMetalEdgeFlange2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IInsertSheetMetalEdgeFlange( _    ByVal FlangeEdge As Edge, _    ByVal SketchFeat As Feature, _    ByVal BooleanOptions As System.Integer, _    ByVal DAngle As System.Double, _    ByVal DRadius As System.Double, _    ByVal BendPosition As System.Integer, _    ByVal DOffsetDist As System.Double, _    ByVal ReliefType As System.Integer, _    ByVal DReliefRatio As System.Double, _    ByVal DReliefWidth As System.Double, _    ByVal DReliefDepth As System.Double _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim FlangeEdge As Edge Dim SketchFeat As Feature Dim BooleanOptions As System.Integer Dim DAngle As System.Double Dim DRadius As System.Double Dim BendPosition As System.Integer Dim DOffsetDist As System.Double Dim ReliefType As System.Integer Dim DReliefRatio As System.Double Dim DReliefWidth As System.Double Dim DReliefDepth As System.Double Dim value As Feature   value = instance.IInsertSheetMetalEdgeFlange(FlangeEdge, SketchFeat, BooleanOptions, DAngle, DRadius, BendPosition, DOffsetDist, ReliefType, DReliefRatio, DReliefWidth, DReliefDepth) ``` | |

| C# |  |
| --- | --- |
| ``` Feature IInsertSheetMetalEdgeFlange(     Edge FlangeEdge,    Feature SketchFeat,    System.int BooleanOptions,    System.double DAngle,    System.double DRadius,    System.int BendPosition,    System.double DOffsetDist,    System.int ReliefType,    System.double DReliefRatio,    System.double DReliefWidth,    System.double DReliefDepth ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ IInsertSheetMetalEdgeFlange(  &   Edge^ FlangeEdge, &   Feature^ SketchFeat, &   System.int BooleanOptions, &   System.double DAngle, &   System.double DRadius, &   System.int BendPosition, &   System.double DOffsetDist, &   System.int ReliefType, &   System.double DReliefRatio, &   System.double DReliefWidth, &   System.double DReliefDepth ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FlangeEdge*

*SketchFeat*

*BooleanOptions*

*DAngle*

*DRadius*

*BendPosition*

*DOffsetDist*

*ReliefType*

*DReliefRatio*

*DReliefWidth*

*DReliefDepth*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::IInsertSheetMetalEdgeFlange.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)
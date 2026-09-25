<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSheetMetalEdgeFlange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSheetMetalEdgeFlange Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertSheetMetalEdgeFlange Method (IFeatureManager) |

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

*FlangeSharpType*

*PCBA*

Obsolete. Superseded by [IFeatureManager::InsertSheetMetalEdgeFlange2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertSheetMetalEdgeFlange2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSheetMetalEdgeFlange( _    ByVal FlangeEdge As Edge, _    ByVal SketchFeat As Feature, _    ByVal BooleanOptions As System.Integer, _    ByVal DAngle As System.Double, _    ByVal DRadius As System.Double, _    ByVal BendPosition As System.Integer, _    ByVal DOffsetDist As System.Double, _    ByVal ReliefType As System.Integer, _    ByVal DReliefRatio As System.Double, _    ByVal DReliefWidth As System.Double, _    ByVal DReliefDepth As System.Double, _    ByVal FlangeSharpType As System.Integer, _    ByVal PCBA As CustomBendAllowance _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim FlangeEdge As Edge Dim SketchFeat As Feature Dim BooleanOptions As System.Integer Dim DAngle As System.Double Dim DRadius As System.Double Dim BendPosition As System.Integer Dim DOffsetDist As System.Double Dim ReliefType As System.Integer Dim DReliefRatio As System.Double Dim DReliefWidth As System.Double Dim DReliefDepth As System.Double Dim FlangeSharpType As System.Integer Dim PCBA As CustomBendAllowance Dim value As Feature   value = instance.InsertSheetMetalEdgeFlange(FlangeEdge, SketchFeat, BooleanOptions, DAngle, DRadius, BendPosition, DOffsetDist, ReliefType, DReliefRatio, DReliefWidth, DReliefDepth, FlangeSharpType, PCBA) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertSheetMetalEdgeFlange(     Edge FlangeEdge,    Feature SketchFeat,    System.int BooleanOptions,    System.double DAngle,    System.double DRadius,    System.int BendPosition,    System.double DOffsetDist,    System.int ReliefType,    System.double DReliefRatio,    System.double DReliefWidth,    System.double DReliefDepth,    System.int FlangeSharpType,    CustomBendAllowance PCBA ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertSheetMetalEdgeFlange(  &   Edge^ FlangeEdge, &   Feature^ SketchFeat, &   System.int BooleanOptions, &   System.double DAngle, &   System.double DRadius, &   System.int BendPosition, &   System.double DOffsetDist, &   System.int ReliefType, &   System.double DReliefRatio, &   System.double DReliefWidth, &   System.double DReliefDepth, &   System.int FlangeSharpType, &   CustomBendAllowance^ PCBA ) ``` | |

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

*FlangeSharpType*

*PCBA*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertSheetMetalEdgeFlange.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)
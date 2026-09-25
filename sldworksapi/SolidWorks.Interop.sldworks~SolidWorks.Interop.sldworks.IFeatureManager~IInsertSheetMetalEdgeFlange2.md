<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~IInsertSheetMetalEdgeFlange2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IInsertSheetMetalEdgeFlange2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : IInsertSheetMetalEdgeFlange2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EdgeCount*
:   Number of edges for the flange

*FlangeEdges*
:   Array of edge to which to apply a flange

*SketchFeatCount*
:   Number of sketches for the flange

*SketchFeat*
:   Array of sketch [features](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) to use for the flange

*BooleanOptions*
:   Flange options as defined by swInsertEdgeFlangeOptions\_e

*FlangeAngle*
:   Flange angle

*FlangeRadius*
:   Bend radius

*BendPosition*
:   Flange bend position as defined by swFlangePositionTypes\_e

*FlangeOffsetDist*
:   Length of flange

*ReliefType*
:   Relief type as defined by swSheetMetalReliefTypes\_e

*FlangeReliefRatio*
:   Relief ratio

*FlangeReliefWidth*
:   Relief width

*FlangeReliefDepth*
:   Relief depth

*FlangeSharpType*
:   Flange virtual sharp type as defined by swFlangeDimTypes\_e

*CustomBendAllowance*
:   |  |  |
    | --- | --- |
    | **If...** | **Then...** |
    | non-NULL | Pointer to [ICustomBendAllowance](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICustomBendAllowance.html) object for which required values have been set |
    | NULL | Parent bend's bend allowance is used |

Obsolete. Superseded by [IFeatureManager::CreateDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateDefinition.html) and [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IInsertSheetMetalEdgeFlange2( _    ByVal EdgeCount As System.Integer, _    ByRef FlangeEdges As Edge, _    ByVal SketchFeatCount As System.Integer, _    ByRef SketchFeat As Feature, _    ByVal BooleanOptions As System.Integer, _    ByVal FlangeAngle As System.Double, _    ByVal FlangeRadius As System.Double, _    ByVal BendPosition As System.Integer, _    ByVal FlangeOffsetDist As System.Double, _    ByVal ReliefType As System.Integer, _    ByVal FlangeReliefRatio As System.Double, _    ByVal FlangeReliefWidth As System.Double, _    ByVal FlangeReliefDepth As System.Double, _    ByVal FlangeSharpType As System.Integer, _    ByVal CustomBendAllowance As CustomBendAllowance _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim EdgeCount As System.Integer Dim FlangeEdges As Edge Dim SketchFeatCount As System.Integer Dim SketchFeat As Feature Dim BooleanOptions As System.Integer Dim FlangeAngle As System.Double Dim FlangeRadius As System.Double Dim BendPosition As System.Integer Dim FlangeOffsetDist As System.Double Dim ReliefType As System.Integer Dim FlangeReliefRatio As System.Double Dim FlangeReliefWidth As System.Double Dim FlangeReliefDepth As System.Double Dim FlangeSharpType As System.Integer Dim CustomBendAllowance As CustomBendAllowance Dim value As Feature   value = instance.IInsertSheetMetalEdgeFlange2(EdgeCount, FlangeEdges, SketchFeatCount, SketchFeat, BooleanOptions, FlangeAngle, FlangeRadius, BendPosition, FlangeOffsetDist, ReliefType, FlangeReliefRatio, FlangeReliefWidth, FlangeReliefDepth, FlangeSharpType, CustomBendAllowance) ``` | |

| C# |  |
| --- | --- |
| ``` Feature IInsertSheetMetalEdgeFlange2(     System.int EdgeCount,    ref Edge FlangeEdges,    System.int SketchFeatCount,    ref Feature SketchFeat,    System.int BooleanOptions,    System.double FlangeAngle,    System.double FlangeRadius,    System.int BendPosition,    System.double FlangeOffsetDist,    System.int ReliefType,    System.double FlangeReliefRatio,    System.double FlangeReliefWidth,    System.double FlangeReliefDepth,    System.int FlangeSharpType,    CustomBendAllowance CustomBendAllowance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ IInsertSheetMetalEdgeFlange2(  &   System.int EdgeCount, &   Edge^% FlangeEdges, &   System.int SketchFeatCount, &   Feature^% SketchFeat, &   System.int BooleanOptions, &   System.double FlangeAngle, &   System.double FlangeRadius, &   System.int BendPosition, &   System.double FlangeOffsetDist, &   System.int ReliefType, &   System.double FlangeReliefRatio, &   System.double FlangeReliefWidth, &   System.double FlangeReliefDepth, &   System.int FlangeSharpType, &   CustomBendAllowance^ CustomBendAllowance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*EdgeCount*
:   Number of edges for the flange

*FlangeEdges*
:   Array of edge to which to apply a flange

*SketchFeatCount*
:   Number of sketches for the flange

*SketchFeat*
:   Array of sketch [features](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) to use for the flange

*BooleanOptions*
:   Flange options as defined by swInsertEdgeFlangeOptions\_e

*FlangeAngle*
:   Flange angle

*FlangeRadius*
:   Bend radius

*BendPosition*
:   Flange bend position as defined by swFlangePositionTypes\_e

*FlangeOffsetDist*
:   Length of flange

*ReliefType*
:   Relief type as defined by swSheetMetalReliefTypes\_e

*FlangeReliefRatio*
:   Relief ratio

*FlangeReliefWidth*
:   Relief width

*FlangeReliefDepth*
:   Relief depth

*FlangeSharpType*
:   Flange virtual sharp type as defined by swFlangeDimTypes\_e

*CustomBendAllowance*
:   |  |  |
    | --- | --- |
    | **If...** | **Then...** |
    | non-NULL | Pointer to [ICustomBendAllowance](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICustomBendAllowance.html) object for which required values have been set |
    | NULL | Parent bend's bend allowance is used |

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::IInsertSheetMetalEdgeFlange2.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IModelDoc2::IInsertSketchForEdgeFlange](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~IInsertSketchForEdgeFlange.html) and create a profile for the flange. After creating the profile, call this method to create the flange.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::InsertSheetMetalEdgeFlange Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertSheetMetalEdgeFlange.html)

[IEdgeFlangeFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdgeFlangeFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateDefinition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateDefinition Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : CreateDefinition Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   Feature name ID as defined in swFeatureNameID\_e:

    * swFMBaseFlange (sheet metal base flange)* swFMBeltAndChain (belt/chain)* swFmBoundingBox (bounding box)* swFmCirPattern (circular pattern)* swFmCornerRelief (sheet metal corner relief)* swFmCurvePattern (curve-driven pattern)* swFmDerivedLPattern (derived-driven pattern)* swFmDimPattern (variable/dimension pattern)* swFmEdgeFlange (sheet metal edge flange)* swFmFillet (constant radius, face, full round fillet/chamfer)* swFmFillPattern (fill pattern)* swFmGroundPlane (ground plane)* swFmLibraryFeature (library)* swFmLocalChainPattern (chain component pattern)* swFmLocalCirPattern (circular component pattern)* swFmLocalCurvePattern (curve-driven component pattern)* swFmLocalLPattern (linear component pattern)* swFmLocalSketchPattern (sketch-driven component pattern)* swFmLPattern (linear pattern)* swFmMirrorComponent (mirror components)* swFmNormalCut (sheet metal normal cut)* swFmRefCurve (projection curve)* swFmRefSurface (surface sweep)* swFmSketchPattern (sketch-driven pattern)* swFmSMGusset (sheet metal gusset)* swFmSweep (boss sweep)* swFmSweepCut (cut sweep)* swFmSweepThread (sweep thread)* swFmSweptFlange (sheet metal swept flange)* swFmTabAndSlot (tab and slot)* swFmTablePattern (table pattern)

Creates a feature data object of the specified type.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateDefinition( _    ByVal Type As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Type As System.Integer Dim value As System.Object   value = instance.CreateDefinition(Type) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateDefinition(     System.int Type ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateDefinition(  &   System.int Type ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*
:   Feature name ID as defined in swFeatureNameID\_e:

    * swFMBaseFlange (sheet metal base flange)* swFMBeltAndChain (belt/chain)* swFmBoundingBox (bounding box)* swFmCirPattern (circular pattern)* swFmCornerRelief (sheet metal corner relief)* swFmCurvePattern (curve-driven pattern)* swFmDerivedLPattern (derived-driven pattern)* swFmDimPattern (variable/dimension pattern)* swFmEdgeFlange (sheet metal edge flange)* swFmFillet (constant radius, face, full round fillet/chamfer)* swFmFillPattern (fill pattern)* swFmGroundPlane (ground plane)* swFmLibraryFeature (library)* swFmLocalChainPattern (chain component pattern)* swFmLocalCirPattern (circular component pattern)* swFmLocalCurvePattern (curve-driven component pattern)* swFmLocalLPattern (linear component pattern)* swFmLocalSketchPattern (sketch-driven component pattern)* swFmLPattern (linear pattern)* swFmMirrorComponent (mirror components)* swFmNormalCut (sheet metal normal cut)* swFmRefCurve (projection curve)* swFmRefSurface (surface sweep)* swFmSketchPattern (sketch-driven pattern)* swFmSMGusset (sheet metal gusset)* swFmSweep (boss sweep)* swFmSweepCut (cut sweep)* swFmSweepThread (sweep thread)* swFmSweptFlange (sheet metal swept flange)* swFmTabAndSlot (tab and slot)* swFmTablePattern (table pattern)

#### Return Value

[thread](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThreadFeatureData.html), [sweep](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData.html), [library](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData.html), [tab and slot](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITabAndSlotFeatureData.html), [bounding box](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundingBoxFeatureData.html), [ground plane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGroundPlaneFeatureData.html), [mirror components](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorComponentFeatureData.html), [projection curve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProjectionCurveFeatureData.html), [sheet metal normal cut](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2.html), [sheet metal swept flange](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweptFlangeFeatureData.html), [sheet metal gusset](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMGussetFeatureData.html), [sheet metal edge flange](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdgeFlangeFeatureData.html), [simple fillet/chamfer](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2.html), [belt/chain](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData.html), [sheet metal base flange](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData.html), [sheet metal corner relief](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData.html), or pattern-specific feature data object (see **Remarks**); Nothing or null otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::CreateDefinition.

# ![](dotnetimages/collapse.gif)Example

See examples for:

[IBaseFlangeFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData.html)

[IBeltChainFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBeltChainFeatureData.html)

[ICornerReliefFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData.html)

[IEdgeFlangeFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdgeFlangeFeatureData.html)

[ITabAndSlotFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITabAndSlotFeatureData.html)

[IMirrorComponentFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorComponentFeatureData.html)

[IPartialEdgeFilletData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData.html)

[ISimpleFilletFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2.html)

[ISMGussetFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMGussetFeatureData.html)

[ISweptFlangeFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweptFlangeFeatureData.html)

# ![](dotnetimages/collapse.gif)Example

[Create a Thread Feature (VBA)](Create_a_Thread_Feature_Example_VB.htm)

[Create a Thread Feature (VB.NET)](Create_a_Thread_Feature_Example_VBNET.htm)

[Create a Thread Feature (C#)](Create_a_Thread_Feature_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method initializes the feature data objects with default data for pattern, sweep, bounding box, ground plane, mirror components, projection curve, sheet metal normal cut, sheet metal swept flange, sheet metal gusset, sheet metal edge flange, tab/slot, and belt/chain features. For sheet metal base flange, sheet metal corner relief, library, simple fillet, and thread features, you must initialize feature data objects using specific initialize methods. See the **See Also** section.

For additional information, see:

* Library Features and LibraryFeatureData Objects* Pattern Features and their Feature Data Objects* Sweep Features and SweepFeatureData Objects* Thread Features and ThreadFeatureData Objects

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeature::GetDefinition Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetDefinition.html)

[IFeature::IGetDefinition Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetDefinition.html)

[IFeatureManager::CreateFeature Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html)

[ILibraryFeatureData::Initialize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData~Initialize.html)

[IThreadFeatureData::InitializeThreadData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThreadFeatureData~InitializeThreadData.html)

[ISimpleFilletFeatureData2::Initialize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2~Initialize.html)

[IBaseFlangeFeatureData::Initialize Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData~Initialize.html)

[ICornerReliefFeatureData::Initialize](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICornerReliefFeatureData~Initialize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0
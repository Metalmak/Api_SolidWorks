<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetTypeName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetTypeName Method (IFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) : GetTypeName Method (IFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the type of feature.

**NOTE:** To get the underlying type of feature of an Instant3D feature (i.e., "ICE"), call this method; otherwise, call [IFeature::GetTypeName2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetTypeName2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetTypeName() As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeature Dim value As System.String   value = instance.GetTypeName() ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetTypeName() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetTypeName(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

String identifying the type of feature (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Feature::GetTypeName.

# ![](dotnetimages/collapse.gif)Example

[Get Faces Associated with Feature (VBA)](Get_Faces_Associated_with_Feature_Example_VB.htm)

[Select Origin of Assembly Component (VBA)](Select_Origin_of_Assembly_Component_Example_VB.htm)

[Set Custom Bend Deduction (VBA)](Set_Custom_Bend_Deduction_Example_VB.htm)

[Traverse All Cosmetic Threads (VBA)](Traverse_All_Cosmetic_Threads_Example_VB.htm)

[Traverse Assembly at Component and Feature Level (VBA)](Traverse_Assembly_at_Component_and_Feature_Level_Example_VB.htm)

[Get Info on Plane-Axis (C++)](Get_Info_on_Plane_Axis_Example_CPlusPlus_COM.htm)

[Get Parent Features (C++)](Get_Parent_Features_Example_CPlusPlus_COM.htm)

[Get Selected Feature (C++)](Get_Selected_Feature_Example_CPlusPlus_COM.htm)

[Get Type of Instant3D Feature (C#)](Get_Type_of_Instant3D_Feature_Example_CSharp.htm)

[Get Type of Instant3D Feature (VB.NET)](Get_Type_of_Instant3D_Feature_Example_VBNET.htm)

[Get Type of Instant3D Feature (VBA)](Get_Type_of_Instant3D_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use [IFeature::GetDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetDefinition.html) to get a feature data object (i.e., an object whose interface name ends in FeatureData or FeatureData2, such as ISymmetricMateFeatureData, IExtrudeFeatureData2, ILoftFeatureData, ISimpleFilletFeatureData2, IChamferFeatureData2, etc.); otherwise, use [IFeature::GetSpecificFeature2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetSpecificFeature2.html) to get an object for a feature.

| Type of feature | String returned by this method | Interface |
| --- | --- | --- |
| **Assembly** | AsmExploder | None (Assembly exploded view in ConfigurationManager) |
|  | CompExplodeStep | None (Explode step in assembly exploded view) |
|  | ExplodeLineProfileFeature | [ISketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html) |
|  | InContextFeatHolder | [IFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) |
|  | MagneticGroundPlane | [IFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) |
|  | MateCamTangent | [ICamFollowerMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICamFollowerMateFeatureData.html) |
|  | MateCoincident | [ICoincidentMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoincidentMateFeatureData.html) |
|  | MateConcentric | [IConcentricMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConcentricMateFeatureData.html) |
|  | MateDistanceDim | [IDistanceMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDistanceMateFeatureData.html) |
|  | MateGearDim | [IGearMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGearMateFeatureData.html) |
|  | MateHinge | [IHingeMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHingeMateFeatureData.html) |
|  | MateInPlace | [IMate2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2.html) |
|  | MateLinearCoupler | [ILinearCouplerMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILinearCouplerMateFeatureData.html) |
|  | MateLock | [ILockMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILockMateFeatureData.html) |
|  | MateParallel | [IParallelMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParallelMateFeatureData.html) |
|  | MatePerpendicular | [IPerpendicularMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPerpendicularMateFeatureData.html) |
|  | MatePlanarAngleDim | [IAngleMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAngleMateFeatureData.html) |
|  | MateProfileCenter | [IProfileCenterMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileCenterMateFeatureData.html) |
|  | MateRackPinionDim | [IRackPinionMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRackPinionMateFeatureData.html) |
|  | MateScrew | [IScrewMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IScrewMateFeatureData.html) |
|  | MateSlot | [ISlotMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlotMateFeatureData.html) |
|  | MateSymmetric | [ISymmetricMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISymmetricMateFeatureData.html) |
|  | MateTangent | [ITangentMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITangentMateFeatureData.html) |
|  | MateUniversalJoint | [IUniversalJointMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUniversalJointMateFeatureData.html) |
|  | MateWidth | [IWidthMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWidthMateFeatureData.html) |
|  | PosGroupFolder | [IMateReference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateReference.html) |
|  | SmartComponentFeature | [ISmartComponentFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISmartComponentFeatureData.html) |
| **Body** | AdvHoleWzd | [IAdvancedHoleFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedHoleFeatureData.html) |
|  | APattern | [IFillPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData.html) |
|  | BaseBody | [IExtrudeFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2.html) |
|  | Bending | None (**Flex** feature) |
|  | Blend | [ILoftFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoftFeatureData.html) |
|  | BlendCut | [ILoftFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoftFeatureData.html) |
|  | BodyExplodeStep | None (Explode step of multi-body part exploded view) |
|  | Boss | [IExtrudeFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2.html) |
|  | BossThin | [IExtrudeFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2.html) |
|  | Chamfer | [IChamferFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IChamferFeatureData2.html) |
|  | CirPattern | [ICircularPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICircularPatternFeatureData.html) |
|  | CombineBodies | [ICombineBodiesFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICombineBodiesFeatureData.html) |
|  | CosmeticThread | [ICosmeticThreadFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticThreadFeatureData.html) |
|  | CosmeticWeldBead | [ICosmeticWeldBeadFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFeatureData.html) |
|  | CreateAssemFeat | [ISaveBodyFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISaveBodyFeatureData.html) |
|  | CurvePattern | [ICurveDrivenPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurveDrivenPatternFeatureData.html) |
|  | Cut | [IExtrudeFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2.html) |
|  | CutThin | [IExtrudeFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2.html) |
|  | Deform | None (**Deform** feature) |
|  | DeleteBody | [IDeleteBodyFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDeleteBodyFeatureData.html) |
|  | DelFace | [IDeleteFaceFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDeleteFaceFeatureData.html) |
|  | DerivedCirPattern | [IDerivedPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData.html) |
|  | DerivedLPattern | [IDerivedPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPatternFeatureData.html) |
|  | DimPattern | [IDimPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimPatternFeatureData.html) |
|  | Dome | [IDomeFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDomeFeatureData2.html) |
|  | Draft | [IDraftFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDraftFeatureData2.html) |
|  | EdgeMerge | [IHealEdgesFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHealEdgesFeatureData.html) |
|  | Emboss | [IWrapSketchFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWrapSketchFeatureData.html) |
|  | Extrusion | [IExtrudeFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExtrudeFeatureData2.html) |
|  | Fillet | [ISimpleFilletFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2.html) |
|  | Helix | [IHelixFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHelixFeatureData.html) |
|  | HoleSeries | [IHoleSeriesFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleSeriesFeatureData2.html) |
|  | HoleWzd | [IWizardHoleFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWizardHoleFeatureData2.html) |
|  | Imported | None (**Imported** feature) |
|  | LocalChainPattern | [IChainPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IChainPatternFeatureData.html) |
|  | LocalCirPattern | [ILocalCircularPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalCircularPatternFeatureData.html) |
|  | LocalCurvePattern | [ILocalCurvePatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalCurvePatternFeatureData.html) |
|  | LocalLPattern | [ILocalLinearPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData.html) |
|  | LocalSketchPattern | [ILocalSketchPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalSketchPatternFeatureData.html) |
|  | LPattern | [ILinearPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILinearPatternFeatureData.html) |
|  | MacroFeature | [IMacroFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html) |
|  | MirrorCompFeat | [IMirrorComponentFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorComponentFeatureData.html) |
|  | MirrorPattern | [IMirrorPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorPatternFeatureData.html) |
|  | MirrorSolid | [IMirrorSolidFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorSolidFeatureData.html) |
|  | MirrorStock | [IMirrorPartFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorPartFeatureData.html) |
|  | MoveCopyBody | [IMoveCopyBodyFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveCopyBodyFeatureData.html) |
|  | NetBlend | [IBoundaryBossFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundaryBossFeatureData.html) |
|  | PrtExploder | None (Multi-body part exploded view) |
|  | Punch | [IIndentFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData.html) |
|  | ReplaceFace | [IReplaceFaceFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IReplaceFaceFeatureData.html) |
|  | RevCut | [IRevolveFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevolveFeatureData2.html) |
|  | Round fillet corner | [ISimpleFilletFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2.html) |
|  | Revolution | [IRevolveFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevolveFeatureData2.html) |
|  | RevolutionThin | [IRevolveFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevolveFeatureData2.html) |
|  | Rib | [IRibFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRibFeatureData2.html) |
|  | Rip | [IRipFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRipFeatureData.html) |
|  | Sculpt | [IIntersectFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIntersectFeatureData.html) |
|  | Shape | Obsolete |
|  | Shell | [IShellFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShellFeatureData.html) |
|  | SketchHole | [ISimpleHoleFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleHoleFeatureData2.html) |
|  | SketchPattern | [ISketchPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPatternFeatureData.html) |
|  | Split | [ISplitBodyFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData.html) for a feature that was created by splitting a part into multiple parts using either [IFeatureManager::PostSplitBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~PostSplitBody.html) or the **Split** feature in the user interface |
|  | SplitBody | None; returned for a body created by splitting a part and saving the body to a part; you cannot access the data of a split body saved to a part |
|  | Stock | [IDerivedPartFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPartFeatureData.html) |
|  | Sweep | [ISweepFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData.html) |
|  | SweepCut | [ISweepFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData.html) |
|  | SweepThread | [IThreadFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThreadFeatureData.html) |
|  | TablePattern | [ITablePatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData.html) |
|  | Thicken | [IThickenFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData.html) |
|  | ThickenCut | [IThickenFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData.html) |
|  | VarFillet | [IVariableFilletFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2.html) |
| **Drawing** | BendTableAchor | [ITableAnchor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnchor.html) |
|  | BomFeat | [IBomFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature.html) |
|  | BomTemplate | [ITableAnchor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnchor.html) |
|  | DetailCircle | [IDetailCircle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDetailCircle.html) |
|  | DrBreakoutSectionLine | [IDrSection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection.html) or [IBrokenOutSectionFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBrokenOutSectionFeatureData.html) |
|  | DrSectionLine | [IDrSection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection.html) |
|  | GeneralTableAnchor | [ITableAnchor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnchor.html) |
|  | HoleTableAnchor | [ITableAnchor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnchor.html) |
|  | LiveSection | [IRefPlane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html) |
|  | PunchTableAnchor | [ITableAnchor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnchor.html) |
|  | RevisionTableAnchor | [ITableAnchor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnchor.html) |
|  | WeldmentTableAnchor | [ITableAnchor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnchor.html) |
|  | WeldTableAnchor | [ITableAnchor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnchor.html) |
| **Folder** | BlockFolder | Obsolete |
|  | CommentsFolder | [ICommentFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommentFolder.html) |
|  | CosmeticWeldSubFolder | [ICosmeticWeldBeadFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticWeldBeadFolder.html) |
|  | CutListFolder | [IBodyFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBodyFolder.html) |
|  | FeatSolidBodyFolder | [IBodyFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBodyFolder.html) |
|  | FeatSurfaceBodyFolder | [IBodyFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBodyFolder.html) |
|  | FtrFolder | [IFeatureFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureFolder.html) |
|  | InsertedFeatureFolder | [IFeatureFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureFolder.html) |
|  | MateReferenceGroupFolder | [IFeatureFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureFolder.html) |
|  | ProfileFtrFolder | [IFeatureFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureFolder.html) |
|  | RefAxisFtrFolder | [IFeatureFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureFolder.html) |
|  | RefPlaneFtrFolder | [IFeatureFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureFolder.html) |
|  | SketchSliceFolder | [IFeatureFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureFolder.html) |
|  | SolidBodyFolder | [IBodyFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBodyFolder.html) |
|  | SubAtomFolder | [IBodyFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBodyFolder.html) if a body |
|  | SubWeldFolder | [IBodyFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBodyFolder.html) |
|  | SurfaceBodyFolder | [IBodyFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBodyFolder.html) |
|  | TemplateFlatPattern | [IFlatPatternFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlatPatternFolder.html) |
| **Imported File** | MBimport | [IImport3DInterconnectData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImport3DInterconnectData.html) |
| **Miscellaneous** | Attribute | [IAttribute](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAttribute.html) |
|  | BlockDef | Obsolete |
|  | CurveInFile | [IFreePointCurveFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFreePointCurveFeatureData.html) |
|  | GridFeature | None (**Grid** feature) |
|  | LibraryFeature | [ILibraryFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData.html) |
|  | Scale | [IScaleFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IScaleFeatureData.html) |
|  | Sensor | [ISensor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor.html) |
|  | ViewBodyFeature | Obsolete |
| **Mold** | Cavity | [ICavityFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICavityFeatureData.html) |
|  | MoldCoreCavitySolids | [IToolingSplitFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IToolingSplitFeatureData.html) |
|  | MoldPartingGeom | [IPartingSurfaceFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingSurfaceFeatureData.html) |
|  | MoldPartLine | [IPartingLineFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartingLineFeatureData.html) |
|  | MoldShutOffSrf | [IShutOffSurfaceFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShutOffSurfaceFeatureData.html) |
|  | SideCore | [ICoreFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData.html) |
|  | XformStock | [DerivedPartFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDerivedPartFeatureData.html) |
| **Motion and Simulation** | AEM3DContact | [ISimulation3DContactFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulation3DContactFeatureData.html) |
|  | AEMGravity | [ISimulationGravityFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationGravityFeatureData.html) |
|  | AEMLinearDamper | [ISimulationDamperFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationDamperFeatureData.html) |
|  | AEMLinearMotor | [ISimulationMotorFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData.html) |
|  | AEMLinearSpring | [ISimulationLinearSpringFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationLinearSpringFeatureData.html) |
|  | AEMRotationalMotor | [ISimulationMotorFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationMotorFeatureData.html) |
|  | AEMTorque | [ISimulationForceFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationForceFeatureData.html) |
|  | AEMTorsionalDamper | [ISimulationDamperFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimulationDamperFeatureData.html) |
|  | AEMTorsionalSpring | None (**TorsionalSpring** feature) |
|  | SimPlotFeature | [IMotionPlotFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMotionPlotFeatureData.html) |
|  | SimPlotXAxisFeature | [IMotionPlotAxisFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMotionPlotAxisFeatureData.html) |
|  | SimPlotYAxisFeature | [IMotionPlotAxisFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMotionPlotAxisFeatureData.html) |
|  | SimResultFolder | IMotionStudyResults |
| **Reference Geometry** | BoundingBox | [IBoundingBoxFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundingBoxFeatureData.html) |
|  | CoordSys | [ICoordinateSystemFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoordinateSystemFeatureData.html) |
|  | GroundPlane | [IGroundPlaneFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGroundPlaneFeatureData.html) |
|  | RefAxis | [IRefAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html) or [IRefAxisFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html) |
|  | RefPlane | [IRefPlane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html) or [IRefPlaneFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlaneFeatureData.html) |
| **Scenes, Lights, and Cameras** | AmbientLight | [ILight](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILight.html) |
|  | CameraFeature | [ICamera](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICamera.html) |
|  | DirectionLight | [ILight](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILight.html) |
|  | PointLight | [ILight](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILight.html) |
|  | SpotLight | [ILight](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILight.html) |
| **Sheet Metal** | SMBaseFlange | [IBaseFlangeFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBaseFlangeFeatureData.html) |
|  | BreakCorner | [IBreakCornerFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData.html) |
|  | CornerTrim | [IBreakCornerFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakCornerFeatureData.html) |
|  | CrossBreak | [ICrossBreakFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICrossBreakFeatureData.html) |
|  | EdgeFlange | [IEdgeFlangeFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdgeFlangeFeatureData.html) |
|  | FlatPattern | [IFlatPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlatPatternFeatureData.html) |
|  | FlattenBends | [IBendsFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendsFeatureData.html) |
|  | Fold | [IFoldsFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFoldsFeatureData.html) |
|  | FormToolInstance | None (**FormTool** feature) |
|  | Hem | [IHemFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHemFeatureData.html) |
|  | Jog | [IJogFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IJogFeatureData.html) |
|  | LoftedBend | [ILoftedBendsFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoftedBendsFeatureData.html) |
|  | Normal Cut | [ISMNormalCutFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2.html) |
|  | OneBend | [IOneBendFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IOneBendFeatureData.html) |
|  | ProcessBends | [IBendsFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendsFeatureData.html) |
|  | SheetMetal | [ISheetMetalFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFeatureData.html) |
|  | SketchBend | [IOneBendFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IOneBendFeatureData.html) |
|  | SM3dBend | [ISketchedBendFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchedBendFeatureData.html) |
|  | SMGusset | [ISMGussetFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMGussetFeatureData.html) |
|  | SMMiteredFlange | [IMiterFlangeFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMiterFlangeFeatureData.html) |
|  | TemplateSheetMetal | [ISheetMetalFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFolder.html) |
|  | ToroidalBend | [IOneBendFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IOneBendFeatureData.html) |
|  | UnFold | [IFoldsFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFoldsFeatureData.html) |
| **Sketch** | 3DProfileFeature | [ISketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html) |
|  | 3DSplineCurve | [IReferenceCurve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IReferenceCurve.html) or [IReferencePointCurveFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IReferencePointCurveFeatureData.html) |
|  | CompositeCurve | [IReferenceCurve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IReferenceCurve.html) or [ICompositeCurveFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICompositeCurveFeatureData.html) |
|  | ImportedCurve | [IReferenceCurve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IReferenceCurve.html) or [IImportedCurveFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportedCurveFeatureData.html) |
|  | PLine | [ISplitLineFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitLineFeatureData.html) |
|  | ProfileFeature | [ISketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html) |
|  | RefCurve | [IReferenceCurve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IReferenceCurve.html) or [IProjectionCurveFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProjectionCurveFeatureData.html) |
|  | RefPoint | [IRefPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPoint.html) or [IRefPointFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPointFeatureData.html) |
|  | SketchBlockDef | [ISketchBlockDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockDefinition.html) |
|  | SketchBlockInst | [ISketchBlockInstance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance.html) |
|  | SketchBitmap | [ISketchPicture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture.html) |
| **Surface** | BlendRefSurface | None (**Surface-Loft** feature) |
|  | ExtendRefSurface | [ISurfaceExtendFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceExtendFeatureData.html) |
|  | ExtruRefSurface | [ISurfExtrudeFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfExtrudeFeatureData.html) |
|  | FillRefSurface | [IFillSurfaceFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillSurfaceFeatureData.html) |
|  | FlattenSurface | [ISurfaceFlattenFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceFlattenFeatureData.html) |
|  | MidRefSurface | [IMidSurface3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMidSurface3.html) |
|  | OffsetRefSuface | [ISurfaceOffsetFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceOffsetFeatureData.html) |
|  | PlanarSurface | [ISurfacePlanarFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfacePlanarFeatureData.html) |
|  | RadiateRefSurface | [ISurfaceRadiateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceRadiateFeatureData.html) |
|  | RefSurface | None (**Surface-Imported** feature) |
|  | RevolvRefSurf | [ISurfRevolveFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfRevolveFeatureData.html) |
|  | RuledSrfFromEdge | [IRuledSurfaceFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRuledSurfaceFeatureData.html) |
|  | SewRefSurface | [ISurfaceKnitFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceKnitFeatureData.html) |
|  | SurfCut | [ISurfaceCutFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceCutFeatureData.html) |
|  | SweepRefSurface | [ISweepFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData.html) |
|  | TrimRefSurface | [ISurfaceTrimFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceTrimFeatureData.html) |
|  | UnTrimRefSurf | None (**Surface-Untrim** feature) |
| **Weldment and Structure System** | EndCap | [IEndCapFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEndCapFeatureData.html) |
|  | AdvStructMember | [IStructureSystemMemberFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructureSystemMemberFeatureData.html) |
|  | Gusset | [IGussetFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGussetFeatureData.html) |
|  | WeldBeadFeat | [IWeldmentBeadFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentBeadFeatureData.html) |
|  | WeldCornerFeat | [IWeldmentTrimExtendFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentTrimExtendFeatureData.html) |
|  | WeldMemberFeat | [IStructuralMemberFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberFeatureData.html) |
|  | WeldmentFeature | [IStructuralMemberFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberFeatureData.html) |
|  | WeldmentTableFeat | [IWeldmentCutListFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentCutListFeature.html) |

**NOTE:** This method returns strings for some features shown in the FeatureManager design (e.g., **MateGroup**, **Weldment**, etc.) that set up the design functionality environment and, thus, do not have interfaces.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

[IFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature_members.html)

[IFeature::Name Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~Name.html)

[IFeature::GetNameForSelection Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetNameForSelection.html)
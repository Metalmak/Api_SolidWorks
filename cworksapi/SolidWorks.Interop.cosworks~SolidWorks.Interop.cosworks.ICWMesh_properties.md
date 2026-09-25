<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_properties.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWMesh Interface Properties | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWMesh Interface |

For a list of all members of this type, see [ICWMesh members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [AutomaticLooping](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~AutomaticLooping.html) | Obsolete. Superseded by [ICWMesh::AutomaticLooping2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~AutomaticLooping2.html). |
| ![ Property](dotnetimages/Property.gif) | [AutomaticLooping2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~AutomaticLooping2.html) | Gets or sets whether to automatically retry to mesh the model using a different global element size for solids. |
| ![ Property](dotnetimages/Property.gif) | [AutomaticTransition](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~AutomaticTransition.html) | Obsolete. Superseded by [ICWMesh::AutomaticTransition2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~AutomaticTransition2.html). |
| ![ Property](dotnetimages/Property.gif) | [AutomaticTransition2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~AutomaticTransition2.html) | Gets or sets whether mesh controls are automatically applied to small features, holes, fillets, and other fine details in the model. |
| ![ Property](dotnetimages/Property.gif) | [ElementCount](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~ElementCount.html) | Gets the number of elements in the mesh. |
| ![ Property](dotnetimages/Property.gif) | [ElementSize](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~ElementSize.html) | Gets or sets the global element size. |
| ![ Property](dotnetimages/Property.gif) | [ElementSizeFactorForEachLoop](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~ElementSizeFactorForEachLoop.html) | Obsolete. Not superseded. |
| ![ Property](dotnetimages/Property.gif) | [GrowthRatio](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GrowthRatio.html) | Gets or sets the global element size growth ratio starting from regions of highest curvatures in all directions in a curvature-based mesh. |
| ![ Property](dotnetimages/Property.gif) | [IsMeshFailed](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~IsMeshFailed.html) | Obsolete. Superseded by [ICWMesh::IsMeshFailed2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~IsMeshFailed2.html). |
| ![ Property](dotnetimages/Property.gif) | [IsMeshFailed2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~IsMeshFailed2.html) | Checks the status of the mesh. |
| ![ Property](dotnetimages/Property.gif) | [JacobianPoints](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~JacobianPoints.html) | Gets or sets the number of points to be used in calculating a Jacobian ratio. |
| ![ Property](dotnetimages/Property.gif) | [MaxAspectRatio](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MaxAspectRatio.html) | Gets the maximum aspect ratio for all elements in the mesh. |
| ![ Property](dotnetimages/Property.gif) | [MaxElementSize](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MaxElementSize.html) | Gets the maximum element size used for boundaries with lowest curvature in a curvature-based mesh. |
| ![ Property](dotnetimages/Property.gif) | [MeshControlCount](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MeshControlCount.html) | Gets the number of mesh controls defined in the active study. |
| ![ Property](dotnetimages/Property.gif) | [MesherType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MesherType.html) | Gets or sets the type of mesh. |
| ![ Property](dotnetimages/Property.gif) | [MeshState](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MeshState.html) | Gets the mesh state. |
| ![ Property](dotnetimages/Property.gif) | [MeshType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MeshType.html) | Returns the mesh type. |
| ![ Property](dotnetimages/Property.gif) | [MinElementsInCircle](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MinElementsInCircle.html) | Gets or sets the minimum number of elements around a circle to determine the maximum angle in a curvature-based mesh. |
| ![ Property](dotnetimages/Property.gif) | [MinElementSize](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MinElementSize.html) | Gets the minimum element size used for boundaries with highest curvature in a curvature-based mesh. |
| ![ Property](dotnetimages/Property.gif) | [NegativeJacobianRatioCheck](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~NegativeJacobianRatioCheck.html) | Obsolete. Superseded by [ICWMesh::NegativeJacobianRatioCheck2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~NegativeJacobianRatioCheck2.html). |
| ![ Property](dotnetimages/Property.gif) | [NegativeJacobianRatioCheck2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~NegativeJacobianRatioCheck2.html) | Gets or sets whether to check for a negative Jacobian ratio while meshing. |
| ![ Property](dotnetimages/Property.gif) | [NodeCount](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~NodeCount.html) | Gets the number of nodes in the active study. |
| ![ Property](dotnetimages/Property.gif) | [NumberOfLoops](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~NumberOfLoops.html) | Gets or sets the number of loops for automatic mesh looping. |
| ![ Property](dotnetimages/Property.gif) | [Quality](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~Quality.html) | Gets or sets the mesh quality. |
| ![ Property](dotnetimages/Property.gif) | [SaveSettingsWithoutMeshing](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~SaveSettingsWithoutMeshing.html) | Obsolete. Superseded by [ICWMesh::SaveSettingsWithoutMeshing2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~SaveSettingsWithoutMeshing2.html). |
| ![ Property](dotnetimages/Property.gif) | [SaveSettingsWithoutMeshing2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~SaveSettingsWithoutMeshing2.html) | Gets or sets whether to save mesh settings without meshing. |
| ![ Property](dotnetimages/Property.gif) | [SmoothSurface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~SmoothSurface.html) | Obsolete. Not superseded. |
| ![ Property](dotnetimages/Property.gif) | [SmoothSurface2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~SmoothSurface2.html) | Obsolete. Not superseded. |
| ![ Property](dotnetimages/Property.gif) | [TimeToCompleteMesh](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~TimeToCompleteMesh.html) | Gets the estimated time to complete the mesh. |
| ![ Property](dotnetimages/Property.gif) | [Tolerance](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~Tolerance.html) | Gets the tolerance value for mesh loops. |
| ![ Property](dotnetimages/Property.gif) | [ToleranceFactorForEachLoop](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~ToleranceFactorForEachLoop.html) | Obsolete. Not superseded. |
| ![ Property](dotnetimages/Property.gif) | [Unit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~Unit.html) | Gets the units for the mesh. |
| ![ Property](dotnetimages/Property.gif) | [UseJacobianCheckForShells](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~UseJacobianCheckForShells.html) | Obsolete. Superseded by [ICWMesh::UseJacobianCheckForShells2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~UseJacobianCheckForShells2.html). |
| ![ Property](dotnetimages/Property.gif) | [UseJacobianCheckForShells2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~UseJacobianCheckForShells2.html) | Gets or sets whether to perform a Jacobian check for shells. |
| ![ Property](dotnetimages/Property.gif) | [UseJacobianCheckForSolids](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~UseJacobianCheckForSolids.html) | Gets or sets whether to perform a Jacobian check for solids. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)

[ICWMeshControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html)

[ICWStudy::CopyMeshFromStudy Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~CopyMeshFromStudy.html)

[ICWStudy::CreateMesh Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~CreateMesh.html)
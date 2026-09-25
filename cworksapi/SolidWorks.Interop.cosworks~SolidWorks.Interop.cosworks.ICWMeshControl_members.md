<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWMeshControl Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWMeshControl Interface |

The following tables list the members exposed by [ICWMeshControl](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [BeamSelected](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~BeamSelected.html) | Obsolete. Superseded by [ICWMeshControl::BeamSelected2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~BeamSelected2.html). |
| ![ Property](dotnetimages/Property.gif) | [BeamSelected2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~BeamSelected2.html) | Gets and sets whether to select beams for this mesh control. |
| ![ Property](dotnetimages/Property.gif) | [ElementSize](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~ElementSize.html) | Gets or sets the element size of the mesh. |
| ![ Property](dotnetimages/Property.gif) | [EntityCount](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~EntityCount.html) | Gets the number of entities in the mesh control. |
| ![ Property](dotnetimages/Property.gif) | [Layers](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~Layers.html) | Obsolete. Not superseded. |
| ![ Property](dotnetimages/Property.gif) | [MinimumElementSizeForBlendedCurveMesher](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~MinimumElementSizeForBlendedCurveMesher.html) | Gets and sets the minimum element size for a curvature-based mesh. |
| ![ Property](dotnetimages/Property.gif) | [MinNumOfElementsPerCircleForBlendedCurveMesher](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~MinNumOfElementsPerCircleForBlendedCurveMesher.html) | Gets and sets the minimum number of elements in a circle to determine the maximum angle in a curvature-based mesh. |
| ![ Property](dotnetimages/Property.gif) | [Name](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~Name.html) | Gets the name of the mesh control. |
| ![ Property](dotnetimages/Property.gif) | [NumofElementsforBeams](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~NumofElementsforBeams.html) | Gets or sets the total number of mesh elements for selected beams. |
| ![ Property](dotnetimages/Property.gif) | [Ratio](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~Ratio.html) | Gets or sets the ratio of the average element size for element layer (i) to that of layer (i-1) for this mesh control. |
| ![ Property](dotnetimages/Property.gif) | [State](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~State.html) | Gets whether the mesh control is suppressed. |
| ![ Property](dotnetimages/Property.gif) | [Units](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~Units.html) | Gets or sets the units for the mesh control. |
| ![ Property](dotnetimages/Property.gif) | [UseSameElementSize](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~UseSameElementSize.html) | Obsolete. Superseded by [ICWMeshControl::UseSameElementSize2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~UseSameElementSize2.html). |
| ![ Property](dotnetimages/Property.gif) | [UseSameElementSize2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~UseSameElementSize2.html) | Gets or sets whether to use the the same element for all selected components in this mesh control. |
| ![ Property](dotnetimages/Property.gif) | [WeightFactor](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~WeightFactor.html) | Gets or sets the component weight factor for the mesh control. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetEntityAt](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~GetEntityAt.html) | Obsolete. Superseded by [ICWMeshControl::GetEntityAt2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~GetEntityAt2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetEntityAt2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~GetEntityAt2.html) | Obsolete. Superseded by [ICWMeshControl::GetEntityAt3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~GetEntityAt3.html). |
| ![ Method](dotnetimages/Method.gif) | [GetEntityAt3](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~GetEntityAt3.html) | Gets the entity at the specified index for this mesh control. |
| ![ Method](dotnetimages/Method.gif) | [InsertEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~InsertEntity.html) | Adds an entity for mesh control. |
| ![ Method](dotnetimages/Method.gif) | [MeshControlBeginEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~MeshControlBeginEdit.html) | Starts editing the mesh control. |
| ![ Method](dotnetimages/Method.gif) | [MeshControlEndEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~MeshControlEndEdit.html) | Ends editing a mesh control. |
| ![ Method](dotnetimages/Method.gif) | [RemoveEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~RemoveEntity.html) | Removes the specified entity from the mesh control. |
| ![ Method](dotnetimages/Method.gif) | [SuppressUnSuppress](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl~SuppressUnSuppress.html) | Suppresses or unsuppresses the mesh control depending on its [state](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWMeshControl~State.html). |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMeshControl Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMeshControl.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IBody2 Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IBody2 Interface |

The following tables list the members exposed by [IBody2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Check3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Check3.html) | Gets whether the body is a valid and returns an [IFaultEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFaultEntity.html) object if any faults exist. |
| ![ Property](dotnetimages/Property.gif) | [DisableDisplay](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DisableDisplay.html) | Gets or sets whether to hide or show this body. |
| ![ Property](dotnetimages/Property.gif) | [DisableHighlight](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DisableHighlight.html) | Disables highlighting of the selected body in the graphics area. |
| ![ Property](dotnetimages/Property.gif) | [IMaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IMaterialPropertyValues.html) | Obsolete. Superseded by [IBody2::IMaterialPropertyValues2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IMaterialPropertyValues2.html). |
| ![ Property](dotnetimages/Property.gif) | [IMaterialPropertyValues2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IMaterialPropertyValues2.html) | Gets or sets the material properties for a body other than the base body in the active configuration. |
| ![ Property](dotnetimages/Property.gif) | [IsSafe](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IsSafe.html) | Not implemented. |
| ![ Property](dotnetimages/Property.gif) | [MaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~MaterialPropertyValues.html) | Obsolete. Superseded by [IBody2::MaterialPropertyValues2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~MaterialPropertyValues2.html). |
| ![ Property](dotnetimages/Property.gif) | [MaterialPropertyValues2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~MaterialPropertyValues2.html) | Gets or sets the material properties for a body other than the base body in the active configuration. |
| ![ Property](dotnetimages/Property.gif) | [Name](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Name.html) | Gets or sets the name of the selected body. |
| ![ Property](dotnetimages/Property.gif) | [Visible](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Visible.html) | Gets whether this body is visible or hidden. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddConstantFillets](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~AddConstantFillets.html) | Creates constant radius fillets on the specified edges on this body. |
| ![ Method](dotnetimages/Method.gif) | [AddProfileArc](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~AddProfileArc.html) | Creates an arc profile curve and returns a pointer to that curve. |
| ![ Method](dotnetimages/Method.gif) | [AddProfileBspline](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~AddProfileBspline.html) | Creates an B-spline profile curve and returns a pointer to that curve. |
| ![ Method](dotnetimages/Method.gif) | [AddProfileBsplineByPts](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~AddProfileBsplineByPts.html) | Adds a profile B-spline. |
| ![ Method](dotnetimages/Method.gif) | [AddProfileLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~AddProfileLine.html) | Creates a line profile curve and returns a pointer to that curve. |
| ![ Method](dotnetimages/Method.gif) | [AddPropertyExtension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~AddPropertyExtension.html) | Obsolete. Superseded by [IBody2::AddPropertyExtension2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~AddPropertyExtension2.html). |
| ![ Method](dotnetimages/Method.gif) | [AddPropertyExtension2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~AddPropertyExtension2.html) | Adds a property extension to this body. |
| ![ Method](dotnetimages/Method.gif) | [AddVertexPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~AddVertexPoint.html) | Adds a vertex. |
| ![ Method](dotnetimages/Method.gif) | [ApplyTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ApplyTransform.html) | Applies a transform to this body. |
| ![ Method](dotnetimages/Method.gif) | [Check](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Check.html) | Obsolete. Superseded by [IBody2::Check3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~Check3.html). |
| ![ Method](dotnetimages/Method.gif) | [Check2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Check2.html) | Obsolete. Superseded by [IBody2::Check3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~Check3.html). |
| ![ Method](dotnetimages/Method.gif) | [Copy](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Copy.html) | Obsolete. Superseded by [IBody2::Copy2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Copy2.html). |
| ![ Method](dotnetimages/Method.gif) | [Copy2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Copy2.html) | Gets a copy of this body. |
| ![ Method](dotnetimages/Method.gif) | [CreateBaseFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateBaseFeature.html) | Creates a base feature for the imported body. |
| ![ Method](dotnetimages/Method.gif) | [CreateBlendSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateBlendSurface.html) | Creates a constant radius rolling-ball blend surface (also known as a pipe surface) between two side surfaces. |
| ![ Method](dotnetimages/Method.gif) | [CreateBodyFromFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateBodyFromFaces.html) | Creates a temporary body from the faces. |
| ![ Method](dotnetimages/Method.gif) | [CreateBodyFromSurfaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateBodyFromSurfaces.html) | Creates a body from a list of trimmed surfaces. |
| ![ Method](dotnetimages/Method.gif) | [CreateBoundedSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateBoundedSurface.html) | Creates a bounded surface from an independent base surface. |
| ![ Method](dotnetimages/Method.gif) | [CreateBsplineSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateBsplineSurface.html) | Creates a new B-spline surface. |
| ![ Method](dotnetimages/Method.gif) | [CreateExtrusionSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateExtrusionSurface.html) | Creates a new surface of extrusion (infinitely long tabulated cylinder). |
| ![ Method](dotnetimages/Method.gif) | [CreateNewSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateNewSurface.html) | Creates a handle for a new surface to serve as geometry for a face to be added to the body. |
| ![ Method](dotnetimages/Method.gif) | [CreateOffsetSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateOffsetSurface.html) | Creates a new surface offset from an existing surface. |
| ![ Method](dotnetimages/Method.gif) | [CreatePlanarSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreatePlanarSurface.html) | Creates a new infinite planar surface. |
| ![ Method](dotnetimages/Method.gif) | [CreatePlanarTrimSurfaceDLL](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreatePlanarTrimSurfaceDLL.html) | Creates a planar trim surface for this body. |
| ![ Method](dotnetimages/Method.gif) | [CreateRevolutionSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateRevolutionSurface.html) | Creates a new surface of revolution. |
| ![ Method](dotnetimages/Method.gif) | [CreateRuledSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateRuledSurface.html) | Creates a ruled surface from the specified curves and apex point. |
| ![ Method](dotnetimages/Method.gif) | [CreateTempBodyFromSurfaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateTempBodyFromSurfaces.html) | Creates a temporary body from a list of existing trimmed surfaces. |
| ![ Method](dotnetimages/Method.gif) | [CreateTrimmedSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~CreateTrimmedSurface.html) | Creates a trimmed surface from a base surface and a list of existing trimming curves. |
| ![ Method](dotnetimages/Method.gif) | [DeleteBlends](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteBlends.html) | Obsolete. Superseded by [IBody2::DeleteBlends2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~DeleteBlends2.html). |
| ![ Method](dotnetimages/Method.gif) | [DeleteBlends2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteBlends2.html) | Obsolete. Superseded by [IBody2::DeleteBlends3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~DeleteBlends3.html). |
| ![ Method](dotnetimages/Method.gif) | [DeleteBlends3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteBlends3.html) | Removes a set of fillet faces from a temporary body and heals the body. |
| ![ Method](dotnetimages/Method.gif) | [DeleteFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteFaces.html) | Obsolete. Superseded by [IBody2::DeleteFaces3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~DeleteFaces3.html). |
| ![ Method](dotnetimages/Method.gif) | [DeleteFaces2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteFaces2.html) | Obsolete. Superseded by [IBody2::DeleteFaces3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~DeleteFaces3.html). |
| ![ Method](dotnetimages/Method.gif) | [DeleteFaces3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteFaces3.html) | Obsolete. Superseded by [IBody2::IDeleteFaces4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~DeleteFaces4.html). |
| ![ Method](dotnetimages/Method.gif) | [DeleteFaces4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteFaces4.html) | Obsolete. Superseded by [IBody2::DeleteFaces5](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~DeleteFaces5.html). |
| ![ Method](dotnetimages/Method.gif) | [DeleteFaces5](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteFaces5.html) | Deletes a set of faces from a temporary body. |
| ![ Method](dotnetimages/Method.gif) | [DeleteFacesMakeSheetBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeleteFacesMakeSheetBodies.html) | Creates sheet bodies from deleted faces. |
| ![ Method](dotnetimages/Method.gif) | [DeSelect](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DeSelect.html) | Deselects this body. |
| ![ Method](dotnetimages/Method.gif) | [Diagnose](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Diagnose.html) | Gets the [IDiagnoseResult](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDiagnoseResult.html) object for this body. |
| ![ Method](dotnetimages/Method.gif) | [Display](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Display.html) | Obsolete. Superseded by [IBody2::Display3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~Display3.html). |
| ![ Method](dotnetimages/Method.gif) | [Display2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Display2.html) | Obsolete. Superseded by [IBody2::Display3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~Display3.html). |
| ![ Method](dotnetimages/Method.gif) | [Display3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Display3.html) | Displays this temporary body in the context of the specified part or component. |
| ![ Method](dotnetimages/Method.gif) | [DisplayWireFrameXOR](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DisplayWireFrameXOR.html) | Displays a temporary body in the given part's context in XOR mode. |
| ![ Method](dotnetimages/Method.gif) | [DraftBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DraftBody.html) | Obsolete. Superseded by [IBody2::DraftBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~DraftBody2.html). |
| ![ Method](dotnetimages/Method.gif) | [DraftBody2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DraftBody2.html) | Adds drafts to the specified faces on a temporary body. This method modifies the body. |
| ![ Method](dotnetimages/Method.gif) | [EnumFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~EnumFaces.html) | Returns an enumerated list of the faces in a body. |
| ![ Method](dotnetimages/Method.gif) | [ExtendSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ExtendSurface.html) | Creates a new temporary body by extending the selected edges. |
| ![ Method](dotnetimages/Method.gif) | [FindAttribute](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~FindAttribute.html) | Finds an attribute on a body. |
| ![ Method](dotnetimages/Method.gif) | [GetBodyBox](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetBodyBox.html) | Gets the bounding box for this body. |
| ![ Method](dotnetimages/Method.gif) | [GetCoincidenceTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetCoincidenceTransform.html) | Obsolete. Superseded by [IBody2::GetCoincidenceTransform2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetCoincidenceTransform2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetCoincidenceTransform2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetCoincidenceTransform2.html) | Calculates the transformation matrix, which would make the input body coincident with this body if the transformation matrix is applied. |
| ![ Method](dotnetimages/Method.gif) | [GetEdgeCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetEdgeCount.html) | Gets the number of edges for this body. |
| ![ Method](dotnetimages/Method.gif) | [GetEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetEdges.html) | Gets the edges for this body. |
| ![ Method](dotnetimages/Method.gif) | [GetExcessBodyArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetExcessBodyArray.html) | Gets the excess bodies after sewing. |
| ![ Method](dotnetimages/Method.gif) | [GetExtremePoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetExtremePoint.html) | Calculates the extreme point of the model in the specified direction. |
| ![ Method](dotnetimages/Method.gif) | [GetFaceCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetFaceCount.html) | Gets the number of faces in this body. |
| ![ Method](dotnetimages/Method.gif) | [GetFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetFaces.html) | Gets all of the faces on the body. |
| ![ Method](dotnetimages/Method.gif) | [GetFeatureCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetFeatureCount.html) | Gets the number of features in this body in a multibody sheet metal part. |
| ![ Method](dotnetimages/Method.gif) | [GetFeatures](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetFeatures.html) | Gets the features in this body in a multibody sheet metal part. |
| ![ Method](dotnetimages/Method.gif) | [GetFirstFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetFirstFace.html) | Finds the first face in a body and returns the face. |
| ![ Method](dotnetimages/Method.gif) | [GetFirstSelectedFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetFirstSelectedFace.html) | Gets the first selected face on this body. For use with [IBody2::GetProcessedBodyWithSelFace](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetProcessedBodyWithSelFace.html) and intended for IGES routines. |
| ![ Method](dotnetimages/Method.gif) | [GetGraphicsBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetGraphicsBody.html) | Gets the graphics body associated with this body. |
| ![ Method](dotnetimages/Method.gif) | [GetIgesErrorCode](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetIgesErrorCode.html) | Gets the current IGES error code. |
| ![ Method](dotnetimages/Method.gif) | [GetIgesErrorCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetIgesErrorCount.html) | Gets the number of errors encountered while running an IGES routine. |
| ![ Method](dotnetimages/Method.gif) | [GetIntersectionEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetIntersectionEdges.html) | Obsolete. Superseded by [IBody2::GetIntersectionEdges2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetIntersectionEdges2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetIntersectionEdges2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetIntersectionEdges2.html) | Gets the edges resulting from the intersection of the specified tool body and this body. |
| ![ Method](dotnetimages/Method.gif) | [GetMassProperties](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMassProperties.html) | Gets the mass properties of this body. |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialIdName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMaterialIdName.html) | Obsolete. Superseded by [IBody2::GetMaterialIdName2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetMaterialIdName2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialIdName2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMaterialIdName2.html) | Gets the material name for this body. |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialPropertyName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMaterialPropertyName.html) | Gets the names of the material database and the material for the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialUserName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMaterialUserName.html) | Obsolete. Superseded by [IBody2::GetMaterialUserName2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetMaterialIdName2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialUserName2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMaterialUserName2.html) | Gets the material name for this body; the material name is visible to the user. |
| ![ Method](dotnetimages/Method.gif) | [GetMeshBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMeshBody.html) | Gets the mesh body associated with this body. |
| ![ Method](dotnetimages/Method.gif) | [GetMiddleSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetMiddleSurface.html) | Inserts a midsurface in a body. |
| ![ Method](dotnetimages/Method.gif) | [GetNextSelectedFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetNextSelectedFace.html) | Gets the next selected face. For use with [IBody2::GetProcessedBodyWithSelFace](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetProcessedBodyWithSelFace.html) and intended for IGES routines. |
| ![ Method](dotnetimages/Method.gif) | [GetOriginalPatternedBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetOriginalPatternedBody.html) | Gets the original body from this patterned body. Also gets the transformation of this body with respect to the original body. |
| ![ Method](dotnetimages/Method.gif) | [GetProcessedBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetProcessedBody.html) | Obsolete. Superseded by [IBody2::GetProcessedBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetProcessedBody2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetProcessedBody2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetProcessedBody2.html) | Pre-processes the geometry of the body using the specified parameters. |
| ![ Method](dotnetimages/Method.gif) | [GetProcessedBodyWithSelFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetProcessedBodyWithSelFace.html) | Gets a processed body. |
| ![ Method](dotnetimages/Method.gif) | [GetPropertyExtension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetPropertyExtension.html) | Obsolete. Superseded by [IBody2::GetPropertyExtension2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetPropertyExtension2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetPropertyExtension2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetPropertyExtension2.html) | Gets the specified property extension on this body. |
| ![ Method](dotnetimages/Method.gif) | [GetSafeBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetSafeBody.html) | Not implemented. |
| ![ Method](dotnetimages/Method.gif) | [GetSelectedFaceCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetSelectedFaceCount.html) | Gets the number of selected faces on this body. For use with [IBody2::GetProcessedBodyWithSelFace](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetProcessedBodyWithSelFace.html) and [IBody2::IGetPrcoessedBodyWithSelFace](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IGetProcessedBodyWithSelFace.html) and intended for IGES routines. |
| ![ Method](dotnetimages/Method.gif) | [GetSelectedFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetSelectedFaces.html) | Gets the selected faces. For use with [IBody2::GetProcessedBodyWithSelFace](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetProcessedBodyWithSelFace.html) and intended for IGES routines. |
| ![ Method](dotnetimages/Method.gif) | [GetSelectionId](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetSelectionId.html) | Gets the selection ID of the body, if one exists. |
| ![ Method](dotnetimages/Method.gif) | [GetSheetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetSheetBody.html) | Gets a sheet (surface) body in this body. |
| ![ Method](dotnetimages/Method.gif) | [GetTessellation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetTessellation.html) | Gets the [ITessellation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITessellation.html) object. |
| ![ Method](dotnetimages/Method.gif) | [GetTexture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetTexture.html) | Gets the texture applied to this body in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [GetTrackingIDs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetTrackingIDs.html) | Gets the [tracking IDs assigned to this body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~SetTrackingID.html). |
| ![ Method](dotnetimages/Method.gif) | [GetTrackingIDsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetTrackingIDsCount.html) | Gets the number of tracking IDs on this body. |
| ![ Method](dotnetimages/Method.gif) | [GetType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetType.html) | Gets the type of the body. |
| ![ Method](dotnetimages/Method.gif) | [GetUpdateStamp](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetUpdateStamp.html) | Gets the update stamp for the body as of the last rebuild. |
| ![ Method](dotnetimages/Method.gif) | [GetVertexCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetVertexCount.html) | Gets the number of vertices in this body. |
| ![ Method](dotnetimages/Method.gif) | [GetVertices](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetVertices.html) | Gets the vertices in this body. |
| ![ Method](dotnetimages/Method.gif) | [HasMaterialPropertyValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~HasMaterialPropertyValues.html) | Gets whether this body has an appearance. |
| ![ Method](dotnetimages/Method.gif) | [Hide](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Hide.html) | Hides this temporary body in the context of the specified part. |
| ![ Method](dotnetimages/Method.gif) | [HideBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~HideBody.html) | Hides or shows this body. |
| ![ Method](dotnetimages/Method.gif) | [IAddProfileArc](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddProfileArc.html) | Creates an arc profile curve and returns a pointer to that curve. |
| ![ Method](dotnetimages/Method.gif) | [IAddProfileArcDLL](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddProfileArcDLL.html) | Adds a profile arc. |
| ![ Method](dotnetimages/Method.gif) | [IAddProfileBspline](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddProfileBspline.html) | Creates an B-spline profile curve and returns a pointer to that curve. |
| ![ Method](dotnetimages/Method.gif) | [IAddProfileBsplineByPts](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddProfileBsplineByPts.html) | Adds a profile B-spline. |
| ![ Method](dotnetimages/Method.gif) | [IAddProfileBsplineDLL](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddProfileBsplineDLL.html) | Adds a profile B-spline. |
| ![ Method](dotnetimages/Method.gif) | [IAddProfileLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddProfileLine.html) | Creates a line profile curve and returns a pointer to that curve. |
| ![ Method](dotnetimages/Method.gif) | [IAddProfileLineDLL](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddProfileLineDLL.html) | Adds a profile line. |
| ![ Method](dotnetimages/Method.gif) | [IAddVertexPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IAddVertexPoint.html) | Adds a vertex. |
| ![ Method](dotnetimages/Method.gif) | [ICombineVolumes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICombineVolumes.html) | Combines the volumes of two bodies. |
| ![ Method](dotnetimages/Method.gif) | [ICopy](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICopy.html) | Gets a copy of this body. |
| ![ Method](dotnetimages/Method.gif) | [ICreateBaseFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateBaseFeature.html) | Creates a base feature for the imported body. |
| ![ Method](dotnetimages/Method.gif) | [ICreateBlendSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateBlendSurface.html) | Creates a constant radius rolling-ball blend surface (also known as a pipe surface) between two side surfaces. |
| ![ Method](dotnetimages/Method.gif) | [ICreateBodyFromFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateBodyFromFaces.html) | Creates a temporary body from the faces. |
| ![ Method](dotnetimages/Method.gif) | [ICreateBoundedSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateBoundedSurface.html) | Creates a bounded surface from an independent base surface. |
| ![ Method](dotnetimages/Method.gif) | [ICreateBsplineSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateBsplineSurface.html) | Creates a new B-spline surface. |
| ![ Method](dotnetimages/Method.gif) | [ICreateBsplineSurfaceDLL](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateBsplineSurfaceDLL.html) | Creates a B-spline surface in this body. |
| ![ Method](dotnetimages/Method.gif) | [ICreateExtrusionSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateExtrusionSurface.html) | Creates a new surface of extrusion (infinitely long tabulated cylinder). |
| ![ Method](dotnetimages/Method.gif) | [ICreateExtrusionSurfaceDLL](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateExtrusionSurfaceDLL.html) | Creates an extruded surface. |
| ![ Method](dotnetimages/Method.gif) | [ICreateNewSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateNewSurface.html) | Creates a handle for a new surface to serve as geometry for a face to be added to the body. |
| ![ Method](dotnetimages/Method.gif) | [ICreateOffsetSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateOffsetSurface.html) | Creates a new surface offset from an existing surface. |
| ![ Method](dotnetimages/Method.gif) | [ICreatePlanarSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreatePlanarSurface.html) | Creates a new infinite planar surface. |
| ![ Method](dotnetimages/Method.gif) | [ICreatePlanarSurfaceDLL](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreatePlanarSurfaceDLL.html) | Creates a planar surface. |
| ![ Method](dotnetimages/Method.gif) | [ICreatePlanarTrimSurfaceDLL](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreatePlanarTrimSurfaceDLL.html) | Creates a planar trim surface for this body. |
| ![ Method](dotnetimages/Method.gif) | [ICreatePsplineSurfaceDLL](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreatePsplineSurfaceDLL.html) | Creates a B-surface from a piecewise surface. |
| ![ Method](dotnetimages/Method.gif) | [ICreateRevolutionSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateRevolutionSurface.html) | Creates a new surface of revolution. |
| ![ Method](dotnetimages/Method.gif) | [ICreateRevolutionSurfaceDLL](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateRevolutionSurfaceDLL.html) | Creates a surface of revolution for this body. |
| ![ Method](dotnetimages/Method.gif) | [ICreateRuledSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateRuledSurface.html) | Creates a ruled surface from the specified curves and apex point. |
| ![ Method](dotnetimages/Method.gif) | [ICreateTempBodyFromSurfaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ICreateTempBodyFromSurfaces.html) | Creates a temporary body from a list of existing trimmed surfaces. |
| ![ Method](dotnetimages/Method.gif) | [IDeleteBlends](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDeleteBlends.html) | Obsolete. Superseded by [IBody2::IDeleteBlends2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IDeleteBlends2.html). |
| ![ Method](dotnetimages/Method.gif) | [IDeleteBlends2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDeleteBlends2.html) | Obsolete. Superseded by [IBody2::DeleteBlends3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IDeleteBlends3.html). |
| ![ Method](dotnetimages/Method.gif) | [IDeleteBlends3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDeleteBlends3.html) | Removes a set of fillet faces from a temporary body and heals the body. |
| ![ Method](dotnetimages/Method.gif) | [IDeleteFaces2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDeleteFaces2.html) | Obsolete. Superseded by [IBody2::IDeleteFaces3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IDeleteFaces3.html). |
| ![ Method](dotnetimages/Method.gif) | [IDeleteFaces3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDeleteFaces3.html) | Obsolete. Superseded by [IBody2::IDeleteFaces4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~DeleteFaces4.html). |
| ![ Method](dotnetimages/Method.gif) | [IDeleteFacesMakeSheetBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDeleteFacesMakeSheetBodies.html) | Creates sheet bodies from deleted faces. |
| ![ Method](dotnetimages/Method.gif) | [IDeleteFacesMakeSheetBodiesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDeleteFacesMakeSheetBodiesCount.html) | Gets the number of sheet bodies to create from the deleted faces. |
| ![ Method](dotnetimages/Method.gif) | [IDisplay](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDisplay.html) | Obsolete. Superseded by [IBody2::Display3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~Display3.html). |
| ![ Method](dotnetimages/Method.gif) | [IDisplayWireFrameXOR](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDisplayWireFrameXOR.html) | Displays a temporary body in the given part's context in XOR mode. |
| ![ Method](dotnetimages/Method.gif) | [IDraftBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDraftBody.html) | Obsolete. Superseded by [IBody2::IDraftBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IDraftBody2.html). |
| ![ Method](dotnetimages/Method.gif) | [IDraftBody2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IDraftBody2.html) | Adds drafts to the specified faces on a temporary body. This method modifies the body. |
| ![ Method](dotnetimages/Method.gif) | [IExtendSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IExtendSurface.html) | Creates a new temporary body by extending the selected edges. |
| ![ Method](dotnetimages/Method.gif) | [IGetBodyBox](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetBodyBox.html) | Gets the bounding box for this body. |
| ![ Method](dotnetimages/Method.gif) | [IGetEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetEdges.html) | Gets the edges for this body. |
| ![ Method](dotnetimages/Method.gif) | [IGetExcessBodyArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetExcessBodyArray.html) | Gets the excess bodies after sewing. |
| ![ Method](dotnetimages/Method.gif) | [IGetExcessBodyCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetExcessBodyCount.html) | Gets the number of excess bodies. |
| ![ Method](dotnetimages/Method.gif) | [IGetFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetFaces.html) | Gets all of the faces on the body. |
| ![ Method](dotnetimages/Method.gif) | [IGetFeatures](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetFeatures.html) | Gets the features in this body in a multibody sheet metal part. |
| ![ Method](dotnetimages/Method.gif) | [IGetFirstFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetFirstFace.html) | Finds the first face in a body and returns the face. |
| ![ Method](dotnetimages/Method.gif) | [IGetFirstSelectedFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetFirstSelectedFace.html) | Gets the first selected face on this body. For use with [IBody2::IGetProcessedBodyWithSelFace](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IGetProcessedBodyWithSelFace.html) and intended for IGES routines. |
| ![ Method](dotnetimages/Method.gif) | [IGetIntersectionEdgeCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetIntersectionEdgeCount.html) | Gets the number of intersecting edges between this body and the specified tool body. |
| ![ Method](dotnetimages/Method.gif) | [IGetIntersectionEdges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetIntersectionEdges.html) | Obsolete. Superseded by [IBody2::GetIntersectionEdges2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetIntersectionEdges2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetMassProperties](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetMassProperties.html) | Gets the mass properties of this body. |
| ![ Method](dotnetimages/Method.gif) | [IGetMaterialPropertyValuesForFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetMaterialPropertyValuesForFace.html) | Gets the color of the specified face. |
| ![ Method](dotnetimages/Method.gif) | [IGetMiddleSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetMiddleSurface.html) | Inserts a midsurface in a body. |
| ![ Method](dotnetimages/Method.gif) | [IGetNextSelectedFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetNextSelectedFace.html) | Gets the next selected face. For use with [IBody2::GetProcessedBodyWithSelFace](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetProcessedBodyWithSelFace.html) and intended for IGES routines. |
| ![ Method](dotnetimages/Method.gif) | [IGetProcessedBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetProcessedBody.html) | Obsolete. Superseded by [IBody2::GetProcessedBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetProcessedBody2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetProcessedBodyWithSelFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetProcessedBodyWithSelFace.html) | Gets a processed body. |
| ![ Method](dotnetimages/Method.gif) | [IGetSelectedFaces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetSelectedFaces.html) | Gets the selected faces. For use with [IBody2::GetProcessedBodyWithSelFace](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~GetProcessedBodyWithSelFace.html) and intended for IGES routines. |
| ![ Method](dotnetimages/Method.gif) | [IGetSheetBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetSheetBody.html) | Gets a sheet (surface) body in this body. |
| ![ Method](dotnetimages/Method.gif) | [IGetTessellation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetTessellation.html) | Gets the [ITessellation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITessellation.html) object. |
| ![ Method](dotnetimages/Method.gif) | [IGetTrackingIDs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetTrackingIDs.html) | Gets the [tracking IDs assigned to this body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~SetTrackingID.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetVertices](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IGetVertices.html) | Gets the vertices in this body. |
| ![ Method](dotnetimages/Method.gif) | [IHide](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IHide.html) | Hides a temporary body using the specified part's context. |
| ![ Method](dotnetimages/Method.gif) | [IMatchedBoolean](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IMatchedBoolean.html) | Obsolete. Superseded by [IBody2::IMatchedBoolean3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IMatchedBoolean3.html). |
| ![ Method](dotnetimages/Method.gif) | [IMatchedBoolean2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IMatchedBoolean2.html) | Obsolete. Superseded by [IBody2::IMatchedBoolean3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IMatchedBoolean3.html). |
| ![ Method](dotnetimages/Method.gif) | [IMatchedBoolean3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IMatchedBoolean3.html) | Obsolete. Superseded by [IBody2::IMatchedBoolean4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IMatchedBoolean4.html). |
| ![ Method](dotnetimages/Method.gif) | [IMatchedBoolean4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IMatchedBoolean4.html) | Performs a matched boolean on the specified bodies and supports an optional list of faces that match exactly. |
| ![ Method](dotnetimages/Method.gif) | [IOperations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IOperations.html) | Obsolete. Superseded by [IBody2::Operations2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IOperations2.html). |
| ![ Method](dotnetimages/Method.gif) | [IOperations2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IOperations2.html) | Performs add, cut, and intersect (unite, subtract, and interfere) operations between two temporary bodies. |
| ![ Method](dotnetimages/Method.gif) | [IRemoveFacesFromSheet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IRemoveFacesFromSheet.html) | Removes the specified faces from a sheet (surface) body. |
| ![ Method](dotnetimages/Method.gif) | [IRemoveMaterialProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IRemoveMaterialProperty.html) | Removes the material property values (e.g., color) from the body in the specified configurations in parts and assemblies. |
| ![ Method](dotnetimages/Method.gif) | [ISave](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ISave.html) | Saves this body. |
| ![ Method](dotnetimages/Method.gif) | [ISectionBySheet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ISectionBySheet.html) | Sections a body using a sheet (surface) body. |
| ![ Method](dotnetimages/Method.gif) | [ISetCurrentSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ISetCurrentSurface.html) | Places an existing surface into a temporary body that is under construction. |
| ![ Method](dotnetimages/Method.gif) | [ISetXform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ISetXform.html) | Obsolete. Superseded by [IBody2::ApplyTransform](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ApplyTransform.html). |
| ![ Method](dotnetimages/Method.gif) | [IsGraphicsBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IsGraphicsBody.html) | Gets whether this body is a graphics body. |
| ![ Method](dotnetimages/Method.gif) | [IsMeshBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IsMeshBody.html) | Gets whether this body is a mesh body. |
| ![ Method](dotnetimages/Method.gif) | [IsPatternSeed](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IsPatternSeed.html) | Gets whether this body is the seed of a patterned body. |
| ![ Method](dotnetimages/Method.gif) | [IsSheetMetal](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IsSheetMetal.html) | Gets whether this body was created by a sheet metal feature. |
| ![ Method](dotnetimages/Method.gif) | [IsTemporaryBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IsTemporaryBody.html) | Gets whether the body is a temporary body. |
| ![ Method](dotnetimages/Method.gif) | [MakeOffset](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~MakeOffset.html) | Creates a new temporary body by offsetting the selected surface body by the specified distance and in the specified direction. |
| ![ Method](dotnetimages/Method.gif) | [MatchedBoolean](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~MatchedBoolean.html) | Obsolete. Superseded by [IBody2::MatchedBoolean3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~MatchedBoolean3.html). |
| ![ Method](dotnetimages/Method.gif) | [MatchedBoolean2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~MatchedBoolean2.html) | Obsolete. Superseded by [IBody2::MatchedBoolean3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~MatchedBoolean3.html). |
| ![ Method](dotnetimages/Method.gif) | [MatchedBoolean3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~MatchedBoolean3.html) | Obsolete. Superseded by [IBody2::MatchedBoolean4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~MatchedBoolean4.html). |
| ![ Method](dotnetimages/Method.gif) | [MatchedBoolean4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~MatchedBoolean4.html) | Performs a matched boolean on the specified bodies and supports an optional list of faces that match exactly. |
| ![ Method](dotnetimages/Method.gif) | [MinimumRadius](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~MinimumRadius.html) | Gets the minimum radius of this body. |
| ![ Method](dotnetimages/Method.gif) | [Negate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Negate.html) | Reverses the direction (i.e., orientation) of the body. |
| ![ Method](dotnetimages/Method.gif) | [OffsetPlanarWireBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~OffsetPlanarWireBody.html) | Offsets a planar wire body in the normal plane by the specified distance. |
| ![ Method](dotnetimages/Method.gif) | [Operations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Operations.html) | Obsolete. Superseded by [IBody2::Operations2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~Operations2.html). |
| ![ Method](dotnetimages/Method.gif) | [Operations2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Operations2.html) | Performs add, cut, and intersect (unite, subtract, and interfere) operations between two temporary bodies. |
| ![ Method](dotnetimages/Method.gif) | [RemoveFacesFromSheet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~RemoveFacesFromSheet.html) | Removes the specified faces from a sheet (surface) body. |
| ![ Method](dotnetimages/Method.gif) | [RemoveMaterialProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~RemoveMaterialProperty.html) | Removes the material property values (e.g., color) from the body in the specified configurations in parts and assemblies. |
| ![ Method](dotnetimages/Method.gif) | [RemoveRedundantTopology](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~RemoveRedundantTopology.html) | Removes redundant topology from the body. |
| ![ Method](dotnetimages/Method.gif) | [RemoveTexture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~RemoveTexture.html) | Removes the texture applied to this body in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [RemoveTextureByDisplayState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~RemoveTextureByDisplayState.html) | Removes the texture applied to this body in the specified display state. |
| ![ Method](dotnetimages/Method.gif) | [RemoveTrackingID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~RemoveTrackingID.html) | Removes a [tracking ID assigned to this body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~SetTrackingID.html). |
| ![ Method](dotnetimages/Method.gif) | [ResetEdgeTolerances](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ResetEdgeTolerances.html) | Resets the tolerance on all edges of this body. |
| ![ Method](dotnetimages/Method.gif) | [ResetPropertyExtension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ResetPropertyExtension.html) | Obsolete. Superseded by [IBody2::ResetPropertyExtension2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ResetPropertyExtension2.html). |
| ![ Method](dotnetimages/Method.gif) | [ResetPropertyExtension2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~ResetPropertyExtension2.html) | Clears all values stored in the property extension. |
| ![ Method](dotnetimages/Method.gif) | [Save](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Save.html) | Saves this body. |
| ![ Method](dotnetimages/Method.gif) | [Select](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Select.html) | Obsolete. Superseded by [IBody2::Select2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~Select2.html). |
| ![ Method](dotnetimages/Method.gif) | [Select2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Select2.html) | Selects this body and marks it. |
| ![ Method](dotnetimages/Method.gif) | [SetCurrentSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetCurrentSurface.html) | Places an existing surface into a temporary body that is under construction. |
| ![ Method](dotnetimages/Method.gif) | [SetIgesInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetIgesInfo.html) | Sends IGES-specific data to the geometric modeler. |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialIdName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetMaterialIdName.html) | Obsolete. Superseded by [IBody2::SetMaterialIdName2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~SetMaterialIdName2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialIdName2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetMaterialIdName2.html) | Sets the material name for this body. |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetMaterialProperty.html) | Sets the material for this body. |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialUserName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetMaterialUserName.html) | Obsolete. Superseded by [IBody2::SetMaterialUserName2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~SetMaterialUserName2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetMaterialUserName2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetMaterialUserName2.html) | Sets the material name for this body. This material name is visible to the user. |
| ![ Method](dotnetimages/Method.gif) | [SetTexture](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetTexture.html) | Applies texture to this body in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [SetTextureByDisplayState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetTextureByDisplayState.html) | Sets the texture applied to this body in the specified display state. |
| ![ Method](dotnetimages/Method.gif) | [SetTrackingID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetTrackingID.html) | Assigns a tracking ID to this body. |
| ![ Method](dotnetimages/Method.gif) | [SetXform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~SetXform.html) | Obsolete. Superseded by [IBody2::ApplyTransform](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ApplyTransform.html). |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IEnumBodies2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumBodies2.html)
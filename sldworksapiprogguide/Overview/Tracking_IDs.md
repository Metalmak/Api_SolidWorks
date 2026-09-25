<!-- source: sldworksapiprogguide/Overview/Tracking_IDs.htm -->

# SOLIDWORKS API Help

# Tracking IDs

## Overview

Tracking IDs allow you to assign IDs to the following topological entities
in order to track them across modeling operations such as split, merge,
copy, delete, etc.:

* bodies (IBody2::GetTrackingIDs,
  IBody2::IGetTrackingIDs,
  IBody2::GetTrackingIDsCount,
  IBody2::RemoveTrackingID,
  IBody2::SetTrackingID)
* edges (IEdge::GetTrackingIDs,
  IEdge::IGetTrackingIDs,
  IEdge::GetTrackingIDsCount,
  IEdge::RemoveTrackingID,
  IEdge::SetTrackingID)
* faces (IFace2::GetTrackingIDs,
  IFace2::IGetTrackingIDs,
  IFace2::GetTrackingIDsCount,
  IFace2::RemoveTrackingID,
  IFace2::SetTrackingID)
* loops ILoop2::GetTrackingIDs,
  ILoop2::IGetTrackingIDs,
  ILoop2::GetTrackingIDsCount,
  ILoop2::RemoveTrackingID,
  ILoop2::SetTrackingID)
* vertices (IVertex::GetTrackingIDs,
  IVertex::IGetTrackingIDs,
  IVertex::GetTrackingIDsCount,
  IVertex::RemoveTrackingID,
  and IVertex::SetTrackingID)

Your application can define tracking IDs that are specific to that application
to avoid interference with other applications using ISldWorks::RegisterTrackingDefinition.
Because tracking IDs are intended for use by application developers, there
are no visual clues that entities have been assigned tracking IDs. You
can find the entities assigned tracking IDs in a document using IModelDocExtension::FindTrackedObjects.

## Usage

Tracking IDs are supported within a single model document only and are
limited to part and assembly documents. Tracking IDs propagate across
modeling operations (e.g., splitting a face in two —
both faces inherit the tracking ID of the original face) while attributes, persistent IDs, and safe entities
do not.

The lifetime of a tracking ID is from the time of its creation until a
rebuild of the model. Attributes, persistent IDs, and safe entities have longer
lifetimes. Persistent IDs exist across
SOLIDWORKS sessions, and safe entities continue to exist after a rebuild.
Attributes behave like features.

By default, tracking IDs are not persistent across SOLIDWORKS sessions.
However, you can create a macro feature to assign tracking IDs, which
would then allow you to retrieve tracking IDs across SOLIDWORKS sessions.

You can assign a tracking
ID to the result body of a macro feature. You assign the tracking ID as
the last step, just before the result body is returned by the rebuild
function of the macro feature to avoid modifying the body and losing the
tracking ID. You assign the tracking ID to the entire body using IBody2::SetTrackingID
or to individual entities using, for example, IFace2::SetTrackingID. The
latter allows you to reuse the logic required for IMacroFeatureData::SetFaceUserId
(for SOLIDWORKS purposes) for assigning a tracking ID (for your purposes).

## Guidelines

You assign a tracking ID before modifying an entity.

You can:

* obtain bodies to which to assign tracking IDs
  using IPartDoc::GetBodies2.
* obtain bodies, belonging to components in assembly
  documents, to which to assign tracking IDs using IComponent2::GetBodies.
* propagate tracking IDs from a part document to
  component instances of that part in an assembly context. Your application
  can obtain the corresponding face using IModelDocExtension::GetCorrespondingEntity.
  The same tracking ID used in the part document can be assigned to the
  corresponding face in the component context.
* assign:

+ same tracking ID to multiple objects of different
  types.
+ same tracking ID to edges, faces, loops, and
  vertices that belong to different bodies.
+ same tracking ID to bodies, edges, faces,
   loops,
  and vertices that belong to different components.
+ multiple tracking IDs to the same object.
+ tracking IDs to temporary bodies, model bodies,
  surface and solid bodies, and the output bodies of macro features.

You cannot assign tracking IDs:

+ to a general, i.e., non-manifold, body
+ to entities used in sketch or drawing context
+ transient entities (e.g., silhouette edges
  returned by IFace2::IGetSilhoutteEdges
  or edges returned by ISketchText::GetEdges)

## Implementation

| Object | Modeling Operation | | | | | |

| Split | Merge | Delete | Replace | Copy | Pattern |
| IBody2 | S | M | D | R | C | P |
| IEdge | S | M | D | R | C | N/A |
| IFace2 | S | M | D | R | C | P |
| ILoop2 | S | M | D | R | C | N/A |
| IVertex | S | M | D | R | C | N/A |

S = Assign ID to the new object resulting from the split operation.
The number of objects to which the ID is assigned is incremented by 1.

M = Remove ID from the object being merged into another object. The
number of objects to which the ID is assigned is decremented by 1.

D = Remove ID from object being deleted. The number of objects to which
the ID is assigned is decremented with 1.

R = Remove ID from object and assign it to the object that replaces
it. The number of objects to which the ID is assigned remains the same.

C = Assign ID to the new objects resulting from the copy operation.
The number of objects to which the ID is assigned is incremented by the
number of new copies.

P = Assign ID to new objects corresponding to the source object being
patterned. The number of objects to which the ID is assigned is incremented
by the number of new pattern instances. Similar implementation for mirror
operations.

N/A = Not applicable.
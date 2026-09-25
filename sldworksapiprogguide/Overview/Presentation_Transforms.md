<!-- source: sldworksapiprogguide/Overview/Presentation_Transforms.htm -->

# SOLIDWORKS API Help

# Presentation Transforms

The IComponent2::PresentationTransform
property changes the displayed portion of assembly components without
affecting the position of the underlying model geometry. This API:

* Gets or sets the component transform for graphical
  display.
* Ignores all mate and in-context relationships.
  Only the display of the component on the screen is affected.
* Does not apply the transform to component geometry.
* Does not display any changes. To display changes,
  call IModelDoc2::GraphicsRedraw2.

This property's functionality is for graphical purposes only and does
not affect solid models. For example, if you want to animate the explode
steps for an assembly, then maintaining assembly mate and in-context relationships
is not needed or desirable.

Before setting a presentation transform, you must set IAssemblyDoc::EnablePresentation
to true. IAssemblyDoc::EnablePresentation must then be set to false after
a user is finished with presentation transforms and has called IComponent2::RemovePresentationTransform,
which removes any transform applied by IComponent2::PresentationTransform.
After calling this method, the component is next drawn in a position consistent
with its underlying geometry (IComponent2::Transform2).

The preferred way to change the position of an assembly component is
to use the IDragOperator
object. This object allows access to the settings for the Move
Component command in the SOLIDWORKS user interface. Components
moved with this API honor all assembly mate and in-context relationships.
When done
moving a component (IDragOperator::EndDrag),
you might have to call IModelDoc2::EditRebuild3
to update any model geometry.
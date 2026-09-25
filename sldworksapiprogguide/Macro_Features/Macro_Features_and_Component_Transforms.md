<!-- source: sldworksapiprogguide/Macro_Features/Macro_Features_and_Component_Transforms.htm -->

# SOLIDWORKS API Help

# Macro Features and Component Transforms

If a macro feature allows users to select entities, then you may need
to know the component transform of the component where the entity resides
and the transform of the component where the macro feature resides when
editing or regenerating a macro feature.

For example, if an edge on a component other than the component where
the macro feature resides is selected, and you want to use that edge for
direction, then the vector that you calculate will be the component's.
To get the actual direction (the way that it looks on the screen), you
must transform this vector from the edge's component to the component
where the macro feature resides.

To make this transform, you must do two transforms in this order:

1. You must transform the vector from the component
   to the assembly using the transform from IMacroFeatureData::GetSelections3
   or IMacroFeatureData::IGetSelections3.
2. You must transform the vector from the assembly
   to the component where the macro feature resides using IMacroFeatureData::GetEditTargetTransfrom.
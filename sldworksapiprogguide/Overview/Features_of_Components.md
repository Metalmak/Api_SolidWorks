<!-- source: sldworksapiprogguide/Overview/Features_of_Components.htm -->

# SOLIDWORKS API Help

# Features of Components

In SOLIDWORKS 2006 and later, if you want to access a feature of an
assembly component:

1. Get the model document of the
   assembly component by calling:
> * IComponent2::ReferencedConfiguration
> * IComponent2::GetModelDoc
> * IModelDoc2::ShowConfiguration

2. Traverse the FeatureManager design tree to access the feature by
   calling:
> * IModelDoc2::FirstFeature
> * IFeature::GetNextFeature
> * IFeature::GetNextSubFeature

3. Call
   IFeature::GetTypeName
   to check the type of the feature.
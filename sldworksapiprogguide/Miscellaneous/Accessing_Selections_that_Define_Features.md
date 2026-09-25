<!-- source: sldworksapiprogguide/Miscellaneous/Accessing_Selections_that_Define_Features.htm -->

# SOLIDWORKS API Help

# Accessing Selections that Define Features

### To access selections that define features:

1. First, call the AccessSelections
   method for that feature data object (e.g., ICosmeticThreadFeatureData,
   IExtrudeFeatureData2,
   IRevolveFeatureData2,
   ISweepFeatureData,
   etc.).
2. Then, call the desired method for that feature
   data object.
3. Finally,
   release the feature data object:

| If you... | Then... |
| modified the feature data object using IFeature::ModifyDefinition or IFeature::IModifyDefinition2 | the feature data object is automatically released. |
| did not modify the feature data object | call that feature data object's ReleaseSelectionAccess method. |
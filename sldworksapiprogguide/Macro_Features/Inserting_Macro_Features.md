<!-- source: sldworksapiprogguide/Macro_Features/Inserting_Macro_Features.htm -->

# SOLIDWORKS API Help

# Inserting Macro Features

A macro feature can:

* Create one or more new bodies that become part of the model.
* Modify one or more existing bodies.

You insert macro features into a model using IFeatureManager::InsertMacroFeature3
or IFeatureManager::IInsertMacroFeature3.
Pass the feature base name that appears in the FeatureManager design tree
as an argument to the method. Also, pass the parameters needed by the
[rebuild function](Rebuild_Function.htm) as arguments. These
parameters are stored with the feature and are accessible from the rebuild
function and [edit definition function](Edit_Definition_Function.htm)
through the IMacroFeatureData
interface.

Selections that are in effect when the feature is inserted are also
stored with the feature and can be used to define the feature. The feature
becomes dependent on these selections, so it is important to manage the
selection list that is in effect at the time a feature is inserted. If
an existing body is to be modified, it must be passed to the IFeatureManager::InsertMacroFeature3
or IFeatureManager::IInsertMacroFeature3method, and several options can
be specified as well.

For macro features using VBA callback functions, the names of the rebuild
and edit definition functions are passed in as well as the module and
file names in which they can be found. For macro features using COM callback
functions, the ProgId of the COM server is passed in and identifies the
rebuild and edit definition functions to associate with this feature.

If you are working with multiple input and output bodies, set
IMacroFeatureData::EnableMultiBodyConsume to true.
<!-- source: sldworksapiprogguide/Overview/Thread_Features_and_ThreadFeatureData_Objects.htm -->

# SOLIDWORKS API Help

# Thread  Features and ThreadFeatureData Objects

### To create a Thread  feature:

1. See the
   IThreadFeatureData
   examples.
2. Ensure that **Tools > Options > System Options > File Location > Thread
   Options > Folder** contains thread profiles (**\*.sldlfp**).
3. Open a part document with a Hole Wizard hole, Advanced Hole, or Extruded
   Cut.
4. Call IFeatureManager::CreateDefinition(swFeatureNameID\_e.swFmSweepThread)
   to create a new
   ThreadFeatureData object.
5. Initialize the thread feature data object with default property settings using
   IThreadFeatureData::InitializeThreadData.
6. Select thread feature reference entities using
   IModelDocExtension::SelectByRay:
   * Edge of cylinder where the thread begins with Mark = 1.
   * Up To Selection end condition reference with Mark = 1.
   * (Optional) Starting location of the thread helix with Mark = 2, (only
     if step 1 does not select a planar circular edge):
     + vertex
     + reference point
     + edge
     + reference axis
     + reference plane
     + planar surface
7. Set
   IThreadFeatureData::Edge with the selection from step 6.1.
8. Call
   IThreadFeatureData::SetEndConditionReference with Value set to the
   selection from step 6.2.
9. Set
   IThreadFeatureData::StartEntity with the selection from step 6.3.
10. Modify other property settings in the ThreadFeatureData object.
11. Create the thread feature by calling
    IFeatureManager::CreateFeature.

**To edit a Thread feature:**

1. Call
   IFeature::GetDefinition.
2. Call
   IThreadFeatureData::AccessSelections.
3. Modify property settings in the ThreadFeatureData object.
4. Call
   IFeature::ModifyDefinition if you modified the
   feature or
   IThreadFeatureData::ReleaseSelectionAccess if you did not modify
   the feature.
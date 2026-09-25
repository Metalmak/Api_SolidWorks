<!-- source: sldworksapiprogguide/Overview/Hole_Wizard_Features_and_WizardHoleFeatureData2_Objects.htm -->

# SOLIDWORKS API Help

# Hole Wizard Features and WizardHoleFeatureData2 Objects

You can create a Hole Wizard feature by:

* Using an existing
  WizardHoleFeatureData2
  object.
* Creating a new IWizardHoleFeatureData2
  object.

### To create a Hole Wizard feature by using an existing hole wizard feature:

1. Select an existing hole wizard feature to get
   its IWizardHoleFeatureData2 object.
2. Use IFeature::GetDefinition
   to get the IWizardHoleFeatureData2 object.
3. Select the reference entities to use to create
   the hole wizard feature.
4. Use IFeatureManager::CreateFeature
   to create the new hole wizard feature.

### To create a new Hole Wizard feature :

1. Use IFeatureManager::CreateDefinition
   to create a new WizardHoleFeatureData2 object.
2. Initialize the feature data object using IWizardHoleFeatureData2::InitializeHole.
3. Change any default settings using the corresponding
   WizardHoleFeatureData2 properties.
4. Select the reference entities to use to create
   the hole wizard feature.
5. Use IFeatureManager::CreateFeature
   to create the new hole wizard feature.
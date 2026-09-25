<!-- source: sldworksapiprogguide/Overview/Library_Features_and_LibraryFeatureData_Objects.htm -->

# SOLIDWORKS API Help

# Library Features and LibraryFeatureData Objects

### To create a Library feature:

1. Use IFeatureManager::CreateDefinition
   to create a new
   LibraryFeatureData
   object.
2. Initialize the library feature data object using
   ILibraryFeatureData::Initialize
   and a library feature.

   NOTE: This method initializes and opens the last active configuration.
3. If you do not want to apply the library feature
   to the last active configuration:

1. Get all of the configurations using ILibraryFeatureData::GetAllConfigurationNames.
2. Set the configuration name using ILibraryFeatureData::ConfigurationName
   to which to apply the library feature.

   NOTE: This step re-initializes the library feature data
   object.

4. Set whether to link this library feature with
   the original library feature using ILibraryFeatureData::LinkToLibraryPart.
5. Get the type of references required using
   ILibraryFeatureData::GetReferences3.
6. Get the locating dimension names and values using
   ILibraryFeatureData::GetDimensions.
7. Select where to place the library feature using
   IModelDocExtension::SelectByID2.
8. Create the library feature using IFeatureManager::CreateFeature.
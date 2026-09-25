<!-- source: sldworksapiprogguide/Macro_Features/MacroFeatureData_Interface.htm -->

# SOLIDWORKS API Help

# IMacroFeatureData Interface

The IMacroFeatureData
allows access to the data that defines a macro feature. The IMacroFeature
interface supports:

* Typical feature data methods such as IMacroFeatureData::AccessSelections
  or IMacroFeatureData::IAccessSelections
  and IMacroFeatureData::ReleaseSelectionAccess
* An input body, which you can get or set using
  IMacroFeatureData::EditBodies
  or IMacroFeatureData::IGetEditBodies
* Methods for feature parameters. For example:

+ IMacroFeatureData::GetStringByName
  and IMacroFeatureData::SetStringByName
+ IMacroFeatureData::GetDoubleByName
  and IMacroFeatureData::SetDoubleByName
+ IMacroFeatureData::GetIntegerByName
  and IMacroFeatureData::SetIntegerByName
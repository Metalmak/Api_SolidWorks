<!-- source: sldworksapiprogguide/Macro_Features/Exposed_COM_DLL_or_Executable.htm -->

# SOLIDWORKS API Help

# Exposed COM DLL or Executable and Macro Features

For macro features that define their behavior using COM, a COM server
needs to implement the ISwComFeature
interface. This interface has three methods that must be implemented in
the appropriate [macro feature
function](Overview_of_Macro_Features.htm):

* ISwComFeature::Edit
  in the edit definition function
* ISwComFeature::Regenerate
  in the rebuild function
* ISwComFeature::Security
  in the security function

To associate the COM server with the macro feature, supply the program
ID of the COM server as an argument to IFeatureManager::InsertMacroFeature3
or IFeatureManager::IInsertMacroFeature3.
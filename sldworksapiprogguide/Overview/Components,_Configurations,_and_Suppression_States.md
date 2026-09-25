<!-- source: sldworksapiprogguide/Overview/Components,_Configurations,_and_Suppression_States.htm -->

# SOLIDWORKS API Help

# Components, Configurations, and Suppression States

To query the suppression states of a component across multiple configurations,
use:

* IModelDoc2::ConfigurationManager
* IConfigurationManager::GetConfigurationParams

IConfigurationManager::GetConfigurationParams outputs an array of the
configured elements in the document, which is the same information shown
in a design table. If a component is suppressed in a specific configuration,
that component is included in the array. If a component's suppression
state is not output, then the component's suppression state applies to
all configurations.

To query the suppression states of subassembly components across multiple
configurations, you must query each of the subassembly documents and perform
the same operation.
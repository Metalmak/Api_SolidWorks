<!-- source: sldworksapiprogguide/Macro_Features/Macro_Features,_Configurations,_and_Dimensions.htm -->

# SOLIDWORKS API Help

# Macro Features and Configurations

When working with configurable dimensions and a macro feature, only
your [edit definition function](Edit_Definition_Function.htm)
should take into consideration configurations. In your edit definition
function, you can use IDimension::SetSystemValue3
or IDimension::ISetSystemValue3
to modify dimensions values as per the user’s changes. This is similar
to how it works in the SOLIDWORKS user-interface when modifying feature
dimensions across configurations.

Your [rebuild function](Rebuild_Function.htm) should not
attempt to modify dimensions across configurations.
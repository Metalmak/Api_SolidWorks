<!-- source: sldworksapiprogguide/Macro_Features/VBA_Macro_Files.htm -->

# SOLIDWORKS API Help

# VBA Macro Files and Macro Features

Macro features that use VBA macros to define the [macro
feature functions](Overview_of_Macro_Features.htm) must reside in SOLIDWORKS VBA macro files (\*.swp).

Each function:

* Must accept these three arguments, which must
  be declared as type VARIANT:

+ ISldWorks
  interface of the calling process
+ Model interface (IPartDoc,
  IAssemblyDoc,
  or IDrawingDoc)
  to which the feature belongs
+ IFeature
  interface of the macro feature itself

For example:

Function swmRegen(app As Variant, part As
Variant, feature As Variant) As Variant

* Can exist in the same or different file or module.
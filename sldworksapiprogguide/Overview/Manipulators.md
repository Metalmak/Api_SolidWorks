<!-- source: sldworksapiprogguide/Overview/Manipulators.htm -->

# SOLIDWORKS API Help

# Manipulators

You can create a manipulator to use in your part and assembly documents.

Typically to create a manipulator:

1. Create the handler interface, ISwManipulatorHandler2,
   which your add-in application must implement. Your add-in application:

+ Governs the behavior of the manipulator using
  the ISwManipulatorHandler2 methods.
+ Provides any temporary graphics associated
  with the manipulator.
+ Applies transforms.

2. Create the IManipulatorobject using IModelViewManager::CreateManipulator.
3. Use the IManipulator methods and properties to:

+ Remove, show, and control the visibility of
  the manipulator in part or assembly documents.
+ Create a specific manipulator using IManipulator::GetSpecificManipulator.

4. Customize the size and appearance of the specific
   manipulator using the specific manipulator's methods and properties.
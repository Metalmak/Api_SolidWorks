<!-- source: sldworksapi/Get_and_Set_Constraint_for_Dome_Feature_Example_VB.htm -->

# SOLIDWORKS API Help

# Get and Set Constraint for Dome Feature Example (VBA)

This example shows how to get and set a constraining point for a dome
feature. A part containing a dome feature constrained by a sketch point
on the origin is open.

'---------------------------------------------

Option Explicit

Dim swApp As SldWorks.SldWorks

Dim Part As SldWorks.PartDoc

Dim component As SldWorks.Component2

Dim newPointFeat As SldWorks.SketchPoint

Dim dome As SldWorks.feature

Dim domeConstraintPoint As SldWorks.SketchPoint

Dim dome\_featData As SldWorks.DomeFeatureData2

Dim boolstatus As Variant

Sub main()

'{

    Set
swApp = Application.SldWorks

    Set
Part = swApp.ActiveDoc

    boolstatus
= Part.Extension.SelectByID2("Point1@Sketch1",
"EXTSKETCHPOINT", 0, 0, 0, False, 0, Nothing, swSelectOptionDefault)

    Set
newPointFeat = Part.SelectionManager.GetSelectedObject5(1)

    Set
dome = Part.FeatureByName("Dome1")

    Set
dome\_featData = dome.GetDefinition

    boolstatus
= dome\_featData.AccessSelections(Part,
component)

    Set
domeConstraintPoint = dome\_featData.ConstraintPointOrSketch

    If
Not domeConstraintPoint Is Nothing Then

        dome\_featData.ConstraintPointOrSketch = newPointFeat

        boolstatus
= dome.ModifyDefinition(dome\_featData,
Part, Nothing)

    End
If

dome\_featData.ReleaseSelectionAccess

'}

End Sub
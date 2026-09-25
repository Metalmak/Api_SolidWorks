<!-- source: sldworksapi/Get_and_Set_Direction_for_Dome_Feature_Example_VB.htm -->

# SOLIDWORKS API Help

# Get and Set Direction for Dome Feature Example (VBA)

This example shows how to get and set the direction of a dome feature.
You must have a part  containing
a dome feature created with an edge indicating the direction of the feature
and preselect that edge.

'---------------------------------------------

Option Explicit

Dim swApp As SldWorks.SldWorks

Dim part As SldWorks.PartDoc

Dim component As SldWorks.Component2

Dim newEdge As SldWorks.Edge

Dim dome As SldWorks.feature

Dim dome\_featData As SldWorks.DomeFeatureData2

Dim domeDirection As SldWorks.Edge

Dim boolstatus As Variant

Sub main()

'{

    Set
swApp = Application.SldWorks

    Set
part = swApp.ActiveDoc

    Set
newEdge = part.SelectionManager.GetSelectedObject5(1)

    Set
dome = part.FeatureByName("Dome1")

    Set
dome\_featData = dome.GetDefinition

    boolstatus
= dome\_featData.AccessSelections(part,
component)

    Set
domeDirection = dome\_featData.Direction

    If
Not domeDirection Is Nothing Then

        dome\_featData.Direction = newEdge

        boolstatus
= dome.ModifyDefinition(dome\_featData,
part, Nothing)

    End
If

    dome\_featData.ReleaseSelectionAccess

'}

End Sub
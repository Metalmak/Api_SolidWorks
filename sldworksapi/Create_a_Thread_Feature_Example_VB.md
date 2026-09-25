<!-- source: sldworksapi/Create_a_Thread_Feature_Example_VB.htm -->

# SOLIDWORKS API Help

# Create a Thread Feature Example (VBA)

This example shows how to create and edit a thread feature.

'----------------------------------------------------------------------------

' Preconditions:
' 1. Open:
'    *public\_documents***\samples\tutorial\api\holecube.sldprt**
' 2. Open an Immediate window.
'
' Postconditions:
' 1. Creates **Thread1**.
' 2. Modifies the start angle and overrides the pitch of **Thread1**.
' 3. Inspect the Immediate window.
'
' NOTE: Because the model is used elsewhere, do not save changes.
'----------------------------------------------------------------------------

Option Explicit

Sub main()

    Dim swApp As SldWorks.SldWorks
    Dim swModel As SldWorks.ModelDoc2
    Dim swFeat As SldWorks.Feature
    Dim FeatMgr As SldWorks.FeatureManager
    Dim swThreadFeatData As SldWorks.ThreadFeatureData
    Dim pEdge As SldWorks.Edge
    Dim boolstatus As Boolean

     Set swApp = Application.SldWorks
    Set swModel = swApp.**ActiveDoc**

     Set FeatMgr = swModel.**FeatureManager**

'Create and initialize a thread
feature data object
    Set swThreadFeatData = FeatMgr.**CreateDefinition**(swFmSweepThread)
    swThreadFeatData.**InitializeThreadData**
'Specify the thread method type as extrude
    swThreadFeatData.**ThreadMethod** = swThreadMethod\_Extrude

    'Specify the up-to-selection end condition
    swThreadFeatData.**EndCondition** =
swThreadEndCondition\_UpToSelection

     'Select the thread's starting edge
    boolstatus = swModel.**Extension**.**SelectByRay**(0.011047195612548,
-1.90800402080527E-02, -3.65739009737354E-04, 0.164466301431523,
-0.479983539625146, -0.861723063044243, 1.60036844432164E-03, 1, False, 1, 0)
    Set pEdge = swModel.SelectionManager.**GetSelectedObject6**(1,
-1)
    swThreadFeatData.**Edge** = pEdge
    swModel.**ClearSelection2** True

    'Select the thread's up-to reference
    boolstatus = swModel.**Extension**.**SelectByRay**(8.50469161018452E-03,
-2.12858011305457E-02, -2.54798703094821E-02, 0.164466301431523,
-0.479983539625146, -0.861723063044243, 1.60036844432164E-03, 1, True, 1, 0)
    Set pEdge = swModel.**SelectionManager**.**GetSelectedObject6**(1,
-1)
    swThreadFeatData.**SetEndConditionReference** pEdge
    swModel.**ClearSelection2** True

     'Create the thread feature
    Set swFeat = FeatMgr.**CreateFeature**(swThreadFeatData)

     Debug.Print "File = " & swModel.**GetPathName**

     'Access the thread feature data and
print its properties
    Set swThreadFeatData = swFeat.**GetDefinition**()

     swThreadFeatData.**AccessSelections**
swModel, Nothing
    Debug.Print "Offset the starting location of the helix? " &
swThreadFeatData.**Offset**
    Debug.Print "Reverse direction of offset? " &
swThreadFeatData.**ReverseOffset**
    Debug.Print "Offset distance: " & swThreadFeatData.**OffsetDistance**
    Debug.Print "Thread starting angle: " & swThreadFeatData.**ThreadStartAngle**
    Debug.Print "End condition as defined in
swThreadEndCondition\_e: " & swThreadFeatData.**EndCondition**
    Debug.Print "End condition offset: " & swThreadFeatData.**EndConditionOffset**
    Debug.Print "Reverse end condition offset? " &
swThreadFeatData.**EndConditionOffsetReverse**
    Debug.Print "End condition offset distance: " &
swThreadFeatData.**EndConditionOffsetDistance**
    Debug.Print "Keep thread length constant? " &
swThreadFeatData.**MaintainThreadLength**
    Debug.Print "Thread profile type: " & swThreadFeatData.**Type**
    Debug.Print "Size: " & swThreadFeatData.**Size**
    Debug.Print "Diameter overridden? " & swThreadFeatData.**DiameterOverride**
    Debug.Print "Diameter: " & swThreadFeatData.**Diameter**
    Debug.Print "Pitch overridden? " & swThreadFeatData.**PitchOverride**
    Debug.Print "Pitch: " & swThreadFeatData.**Pitch**
    Debug.Print "Thread method as defined in swThreadMethod\_e: "
& swThreadFeatData.**ThreadMethod**
    Debug.Print "Flip the profile of the helix about an axis? " &
swThreadFeatData.**MirrorProfile**
    Debug.Print "How to flip the profile of the helix as defined
in swThreadMirrorType\_e: " & swThreadFeatData.**MirrorType**
    Debug.Print "Helix rotation angle: " & swThreadFeatData.**RotationAngle**
    Debug.Print "Thread wind direction (True = clockwise, False =
counterclockwise): " & swThreadFeatData.**RightHanded**
    Debug.Print "Multiple thread starts? " & swThreadFeatData.**MultipleStart**
    If swThreadFeatData.**MultipleStart** = True Then
        Debug.Print "  Number of starts?
" & swThreadFeatData.**NumberOfStarts**
    End If
    Debug.Print "Trim with the end face? " & swThreadFeatData.**TrimEndFace**
    Debug.Print "Trim with the start face? " & swThreadFeatData.**TrimStartFace**

     'Change the start angle and pitch of
the thread
    swThreadFeatData.**ThreadStartAngle** =
0.04
    swThreadFeatData.**PitchOverride** =
True
    swThreadFeatData.**Pitch** = 0.01

    'Modify the feature definition
    swFeat.**ModifyDefinition** swThreadFeatData, swModel,
Nothing

End Sub
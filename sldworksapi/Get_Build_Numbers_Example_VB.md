<!-- source: sldworksapi/Get_Build_Numbers_Example_VB.htm -->

# SOLIDWORKS API Help

# Get Build Numbers Example (VBA)

This example shows how to get the build, major revision, and hot fix numbers
of the SOLIDWORKS application.

'------------------------------------------------------------
' Preconditions: Open SOLIDWORKS.
'
' Postconditions: Inspect the Immediate window for build,
' major revision, and hot fix numbers.
'-----------------------------------------------------------

```
Dim swApp As SldWorks.SldWorks
Dim BaseVersion As String
Dim CurrentVersion As String
Dim HotFixes As String
```

```
Option Explicit
```

```
Sub main()
```

```
    Set swApp = Application.SldWorks
    swApp.GetBuildNumbers2 BaseVersion, CurrentVersion, HotFixes
    Debug.Print "SOLIDWORKS major revision number: " & BaseVersion
    Debug.Print "SOLIDWORKS build number: " & CurrentVersion
    Debug.Print "SOLIDWORKS hot fix numbers: " & HotFixes
```

```
End Sub
```
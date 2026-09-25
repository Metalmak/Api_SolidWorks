<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RestoreSettings.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RestoreSettings Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : RestoreSettings Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Full path and filename of the settings to restore (**\*.sldreg**) (see **Remarks**)

*SystemOptions*
:   True to restore system options, false to not

*ToolbarLayout*
:   True to restore the toolbar layout, false to not

*KeyboardShortcuts*
:   True to restore keyboard shortcuts, false to not (see **Remarks**)

*MouseGestures*
:   True to restore mouse gestures, false to not

*MenuCustomization*
:   True to restore menu customizations, false to not

*SavedViews*
:   True to restore saved views, false to not (see **Remarks**)

*CreateBackup*
:   True to create a backup of the current settings, false to not (see **Remarks**)

Restores the specified SOLIDWORKS settings from the specified **\*.sldreg** file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RestoreSettings( _    ByVal FileName As System.String, _    ByVal SystemOptions As System.Boolean, _    ByVal ToolbarLayout As System.Boolean, _    ByVal KeyboardShortcuts As System.Boolean, _    ByVal MouseGestures As System.Boolean, _    ByVal MenuCustomization As System.Boolean, _    ByVal SavedViews As System.Boolean, _    ByVal CreateBackup As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FileName As System.String Dim SystemOptions As System.Boolean Dim ToolbarLayout As System.Boolean Dim KeyboardShortcuts As System.Boolean Dim MouseGestures As System.Boolean Dim MenuCustomization As System.Boolean Dim SavedViews As System.Boolean Dim CreateBackup As System.Boolean Dim value As System.Integer   value = instance.RestoreSettings(FileName, SystemOptions, ToolbarLayout, KeyboardShortcuts, MouseGestures, MenuCustomization, SavedViews, CreateBackup) ``` | |

| C# |  |
| --- | --- |
| ``` System.int RestoreSettings(     System.string FileName,    System.bool SystemOptions,    System.bool ToolbarLayout,    System.bool KeyboardShortcuts,    System.bool MouseGestures,    System.bool MenuCustomization,    System.bool SavedViews,    System.bool CreateBackup ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int RestoreSettings(  &   System.String^ FileName, &   System.bool SystemOptions, &   System.bool ToolbarLayout, &   System.bool KeyboardShortcuts, &   System.bool MouseGestures, &   System.bool MenuCustomization, &   System.bool SavedViews, &   System.bool CreateBackup ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Full path and filename of the settings to restore (**\*.sldreg**) (see **Remarks**)

*SystemOptions*
:   True to restore system options, false to not

*ToolbarLayout*
:   True to restore the toolbar layout, false to not

*KeyboardShortcuts*
:   True to restore keyboard shortcuts, false to not (see **Remarks**)

*MouseGestures*
:   True to restore mouse gestures, false to not

*MenuCustomization*
:   True to restore menu customizations, false to not

*SavedViews*
:   True to restore saved views, false to not (see **Remarks**)

*CreateBackup*
:   True to create a backup of the current settings, false to not (see **Remarks**)

#### Return Value

Error code as defined in swSaveRestoreSettingsResults\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::RestoreSettings.

# ![](dotnetimages/collapse.gif)Example

' VBA precondition:

' c:\temp exists

```
Dim swApp As SldWorks.SldWorks
Option Explicit
Sub main()
```

```
    Set swApp = Application.SldWorks

    Dim boolStatus As Long
    Dim path As String

    path = "C:\temp\swSettings2.sldreg"
    boolStatus = swApp.SaveSettings(path, True, swToolbarLayoutOption_e.swToolbarLayoutOption_AllToolbars, True, True, True, True)

    path = "C:\temp\swSettings2.sldreg"
    boolStatus = swApp.RestoreSettings(path, True, True, True, True, True, True, True)
```

```
End Sub
```

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ISldWorks::SaveSettings](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SaveSettings.html) was called previously.

KeyboardShortcuts and SavedViews are valid only if these settings were previously saved using ISldWorks::SaveSettings.

If CreateBackup is true, this method backs up the current settings to **backup\_***userid*\_*yyyymmdd***\_***hhmms*s**.sldreg** in the same location as specified in FileName.

For C++ only, specify all System.bool parameters using VARIANT\_TRUE (-1) and VARIANT\_FALSE (0).

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::LoadAdminSettingsFile Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~LoadAdminSettingsFile.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0
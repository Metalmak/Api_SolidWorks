<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~UploadToMySolidWorksSettings.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| UploadToMySolidWorksSettings Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : UploadToMySolidWorksSettings Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SystemOptions*
:   True to upload, false to not

*FileLocations*
:   True to upload, false to not

*Customizations*
:   True to upload, false to not

Uploads the specified SOLIDWORKS Desktop settings to SOLIDWORKS Connected.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function UploadToMySolidWorksSettings( _    ByVal SystemOptions As System.Boolean, _    ByVal FileLocations As System.Boolean, _    ByVal Customizations As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim SystemOptions As System.Boolean Dim FileLocations As System.Boolean Dim Customizations As System.Boolean Dim value As System.Integer   value = instance.UploadToMySolidWorksSettings(SystemOptions, FileLocations, Customizations) ``` | |

| C# |  |
| --- | --- |
| ``` System.int UploadToMySolidWorksSettings(     System.bool SystemOptions,    System.bool FileLocations,    System.bool Customizations ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int UploadToMySolidWorksSettings(  &   System.bool SystemOptions, &   System.bool FileLocations, &   System.bool Customizations ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SystemOptions*
:   True to upload, false to not

*FileLocations*
:   True to upload, false to not

*Customizations*
:   True to upload, false to not

#### Return Value

Return code as defined by swConnectedSyncSettingsErrors\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::UploadToMySolidWorksSettings.

# ![](dotnetimages/collapse.gif)Remarks

In order to use this method, you must be logged into SOLIDWORKS Connected.

To turn on auto synchronization of settings, call:

* [ISldWorks::SetUserPreferenceToggle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetUserPreferenceToggle.html)(swUserPreferenceToggle\_e.swAutomaticSyncSettings, True)

and then call one, two, or all three of:

* ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSyncSettingsToInclude\_SystemOptions, True)* ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSyncSettingsToInclude\_FileLocations, True)* ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutoSyncSettingsToInclude\_Customizations, True)

To get the timestamp of the last synchronization, call [ISldWorks::GetUserPreferenceStringValue](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetUserPreferenceStringValue.html)(swUserPreferenceStringValue\_e.swLastSynchronizationTimeStamp).

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::DownloadFromMySolidWorksSettings Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~DownloadFromMySolidWorksSettings.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 FCS, Revision Number 29
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings~SaveRoutingSettingsToFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SaveRoutingSettingsToFile Method (IRoutingSettings) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRoutingSettings Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html) : SaveRoutingSettingsToFile Method (IRoutingSettings) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RoutingSettingsFilename*
:   Full path name of file to which to save routing settings; file name must have an extension of **.sqy**

Saves routing settings to the specified file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SaveRoutingSettingsToFile( _    ByVal RoutingSettingsFilename As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRoutingSettings Dim RoutingSettingsFilename As System.String Dim value As System.Boolean   value = instance.SaveRoutingSettingsToFile(RoutingSettingsFilename) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SaveRoutingSettingsToFile(     System.string RoutingSettingsFilename ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SaveRoutingSettingsToFile(  &   System.String^ RoutingSettingsFilename ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RoutingSettingsFilename*
:   Full path name of file to which to save routing settings; file name must have an extension of **.sqy**

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RoutingSettings::SaveRoutingSettingsToFile.

# ![](dotnetimages/collapse.gif)Example

See the [IRoutingSettings](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IRoutingSettings Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings.html)

[IRoutingSettings Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings_members.html)

[IRoutingSettings::LoadRoutingSettingsFromFile Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRoutingSettings~LoadRoutingSettingsFromFile.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0
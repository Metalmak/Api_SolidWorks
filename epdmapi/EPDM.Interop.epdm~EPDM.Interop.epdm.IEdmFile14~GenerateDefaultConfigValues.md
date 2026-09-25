<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile14~GenerateDefaultConfigValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GenerateDefaultConfigValues Method (IEdmFile14) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile14 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile14.html) : GenerateDefaultConfigValues Method (IEdmFile14) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lOldFileID*
:   ID of drawing or file that lacks properties at the configuration level

*bsOldConfigName*
:   Name of configuration whose values to copy (see **Remarks**)

*bsNewConfigName*
:   Name of the configuration to which to copy values (see **Remarks**)

*bsActiveConfig*
:   Name of the active configuration (see **Remarks**)

*bOnlyForUpdateAllFlag*
:   True to copy values only for controls for which [IEdmCardControl6::UpdatesAllConfigurations](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl6~UpdatesAllConfigurations.html) is set to true, false to copy values for all variables associated with this file

Generates default configuration data for the specified drawing or file that lacks properties at the configuration level.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GenerateDefaultConfigValues( _    ByVal lOldFileID As System.Integer, _    ByVal bsOldConfigName As System.String, _    ByVal bsNewConfigName As System.String, _    ByVal bsActiveConfig As System.String, _    ByVal bOnlyForUpdateAllFlag As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GenerateDefaultConfigValues(     System.int lOldFileID,    System.string bsOldConfigName,    System.string bsNewConfigName,    System.string bsActiveConfig,    System.bool bOnlyForUpdateAllFlag ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GenerateDefaultConfigValues(  &   System.int lOldFileID, &   System.String^ bsOldConfigName, &   System.String^ bsNewConfigName, &   System.String^ bsActiveConfig, &   System.bool bOnlyForUpdateAllFlag ) ``` | |

#### Parameters

*lOldFileID*
:   ID of drawing or file that lacks properties at the configuration level

*bsOldConfigName*
:   Name of configuration whose values to copy (see **Remarks**)

*bsNewConfigName*
:   Name of the configuration to which to copy values (see **Remarks**)

*bsActiveConfig*
:   Name of the active configuration (see **Remarks**)

*bOnlyForUpdateAllFlag*
:   True to copy values only for controls for which [IEdmCardControl6::UpdatesAllConfigurations](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl6~UpdatesAllConfigurations.html) is set to true, false to copy values for all variables associated with this file

# ![](dotnetimages/collapse.gif)Example

[Generate Configuration Values (C#)](Generate_Config_Values_Example_CSharp.htm)

[Generate Configuration Values (VB.NET)](Generate_Config_Values_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method:

* is valid only for files with data card variables.* copies values from bsOldConfigName to bsNewConfigName. If it encounters a null control variable in bsOldConfigName, it takes the value from bsActiveConfig instead.

Use [IEdmFile5::GetConfigurations](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetConfigurations.html) to populate the configuration parameters.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile14 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile14.html)

[IEdmFile14 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile14_members.html)

[IEdmFile8::GenerateDefaultValuesForNewConfiguration Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile8~GenerateDefaultValuesForNewConfiguration.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018 SP03
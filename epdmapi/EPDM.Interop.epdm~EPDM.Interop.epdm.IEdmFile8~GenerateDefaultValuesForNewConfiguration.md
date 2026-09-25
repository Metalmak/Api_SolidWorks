<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile8~GenerateDefaultValuesForNewConfiguration.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GenerateDefaultValuesForNewConfiguration Method (IEdmFile8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile8.html) : GenerateDefaultValuesForNewConfiguration Method (IEdmFile8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsConfiguration*
:   Name of the new configuration

*llCfgPersistID*
:   SOLIDWORKS configuration ID; 0 if ID is not available (see **Remarks**)

*poAux*
:   Null; for internal use only

*ppoRetVariables*
:   Array of [IEdmVariableValue5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue5.html)s for the file data card

Populates the file data card with default data when a new configuration is added in SOLIDWORKS.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GenerateDefaultValuesForNewConfiguration( _    ByVal bsConfiguration As System.String, _    ByVal llCfgPersistID As System.Long, _    ByVal poAux As System.Object, _    ByRef ppoRetVariables() As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GenerateDefaultValuesForNewConfiguration(     System.string bsConfiguration,    System.long llCfgPersistID,    System.object poAux,    out System.object[] ppoRetVariables ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GenerateDefaultValuesForNewConfiguration(  &   System.String^ bsConfiguration, &   System.int64 llCfgPersistID, &   System.Object^ poAux, &   [Out] System.array<Object^>^ ppoRetVariables ) ``` | |

#### Parameters

*bsConfiguration*
:   Name of the new configuration

*llCfgPersistID*
:   SOLIDWORKS configuration ID; 0 if ID is not available (see **Remarks**)

*poAux*
:   Null; for internal use only

*ppoRetVariables*
:   Array of [IEdmVariableValue5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue5.html)s for the file data card

# ![](dotnetimages/collapse.gif)Remarks

This method is called by the SOLIDWORKS add-in when a new configuration is added to a file. Its purpose is to populate the file data card with default data for the new configuration.

llCfgPersistID is a unique SOLIDWORKS API configuration ID.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile8.html)

[IEdmFile8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile8_members.html)

[IEdmFile14::GenerateDefaultConfigValues Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile14~GenerateDefaultConfigValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010
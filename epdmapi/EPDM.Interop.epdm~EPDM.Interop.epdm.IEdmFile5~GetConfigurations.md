<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetConfigurations.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetConfigurations Method (IEdmFile5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) : GetConfigurations Method (IEdmFile5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poVersionNoOrRevisionName*
:   Version number or revision name; 0 or empty string to get configurations for the latest version of this file

Gets a list of names of the configurations for the specified version of this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetConfigurations( _    Optional ByRef poVersionNoOrRevisionName As System.Object _ ) As EdmStrLst5 ``` | |

| C# |  |
| --- | --- |
| ``` EdmStrLst5 GetConfigurations(     ref System.object poVersionNoOrRevisionName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmStrLst5^ GetConfigurations(  &   System.Object^% poVersionNoOrRevisionName ) ``` | |

#### Parameters

*poVersionNoOrRevisionName*
:   Version number or revision name; 0 or empty string to get configurations for the latest version of this file

#### Return Value

[IEdmStrList5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html)

# ![](dotnetimages/collapse.gif)Example

[Get File Information (VB.NET)](Get_File_Info_Example_VBNET.htm)

[Get File Information (C#)](Get_File_Info_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Some file types, such as files from AutoCAD and SOLIDWORKS, can contain several configurations or layouts. These configurations are visible as pages in the SOLIDWORKS PDM Professional file data cards.

C++ users not using smart pointer wrapper functions must release the returned interface, IEdmStrLst5.

See [Return Codes](ReturnCodes.htm) for the complete list of potential success and error codes. The following are just a few examples:

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The logged-in user does not have read-access to the specified version or revision.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[IEdmFile5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html)

[IEdmFile14::GenerateDefaultConfigValues Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile14~GenerateDefaultConfigValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2
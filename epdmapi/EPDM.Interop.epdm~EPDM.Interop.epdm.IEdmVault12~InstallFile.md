<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault12~InstallFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| InstallFile Method (IEdmVault12) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault12 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault12.html) : InstallFile Method (IEdmVault12) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsPath*
:   Path to the file to install

*lEdmInstallFileFlags*
:   Combination of [EdmInstallFileFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmInstallFileFlags.html) bits

*oInstallArg*
:   ID of folder where to install the file; valid only if bsPath contains the path to a card file

Installs administrative export files (\*.CEX) and card files (\*.CRD).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub InstallFile( _    ByVal bsPath As System.String, _    ByVal lEdmInstallFileFlags As System.Integer, _    ByVal oInstallArg As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void InstallFile(     System.string bsPath,    System.int lEdmInstallFileFlags,    System.object oInstallArg ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InstallFile(  &   System.String^ bsPath, &   System.int lEdmInstallFileFlags, &   System.Object^ oInstallArg ) ``` | |

#### Parameters

*bsPath*
:   Path to the file to install

*lEdmInstallFileFlags*
:   Combination of [EdmInstallFileFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmInstallFileFlags.html) bits

*oInstallArg*
:   ID of folder where to install the file; valid only if bsPath contains the path to a card file

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault12 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault12.html)

[IEdmVault12 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault12_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011
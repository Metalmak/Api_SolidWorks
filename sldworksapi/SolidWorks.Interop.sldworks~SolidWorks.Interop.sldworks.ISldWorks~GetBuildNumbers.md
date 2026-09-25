<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetBuildNumbers.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBuildNumbers Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetBuildNumbers Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BaseVersion*
:   SOLIDWORKS major revision number

*CurrentVersion*
:   SOLIDWORKS build number

Obsolete. Superseded by [ISldWorks::GetBuildNumbers2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetBuildNumbers2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetBuildNumbers( _    ByRef BaseVersion As System.String, _    ByRef CurrentVersion As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim BaseVersion As System.String Dim CurrentVersion As System.String   instance.GetBuildNumbers(BaseVersion, CurrentVersion) ``` | |

| C# |  |
| --- | --- |
| ``` void GetBuildNumbers(     out System.string BaseVersion,    out System.string CurrentVersion ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetBuildNumbers(  &   [Out] System.String^ BaseVersion, &   [Out] System.String^ CurrentVersion ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BaseVersion*
:   SOLIDWORKS major revision number

*CurrentVersion*
:   SOLIDWORKS build number

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetBuildNumbers.

# ![](dotnetimages/collapse.gif)Example

**Visual Basic for Applications (VBA)**

'-------------------------

Option Explicit

Dim swApp as SldWorks.SldWorks

Dim BaseVersion as String

Dim CurrentVersion as String

Sub main()

Set swApp = Application.SldWorks

swApp.**GetBuildNumbers** BaseVersion, CurrentVersion

Debug.Print "SOLIDWORKS major revision number: " & BaseVersion

Debug.Print "SOLIDWORKS build number: " & CurrentVersion

End Sub

'------------------------------------------

**Output**

SOLIDWORKS major revision number: SW2009\_a1

SOLIDWORKS build number: d080407.062

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::VersionHistory Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~VersionHistory.html)

[ISldWorks::IGetVersionHistoryCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IGetVersionHistoryCount.html)

[ISldWorks::IVersionHistory Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IVersionHistory.html)

[ISldWorks::RevisionNumber Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RevisionNumber.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0
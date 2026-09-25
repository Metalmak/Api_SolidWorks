<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetBuildNumbers2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBuildNumbers2 Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetBuildNumbers2 Method (ISldWorks) |

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

*HotFixes*
:   SOLIDWORKS hot fix numbers

Gets the build, major revision, and hot fix numbers of the SOLIDWORKS application.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetBuildNumbers2( _    ByRef BaseVersion As System.String, _    ByRef CurrentVersion As System.String, _    ByRef HotFixes As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim BaseVersion As System.String Dim CurrentVersion As System.String Dim HotFixes As System.String   instance.GetBuildNumbers2(BaseVersion, CurrentVersion, HotFixes) ``` | |

| C# |  |
| --- | --- |
| ``` void GetBuildNumbers2(     out System.string BaseVersion,    out System.string CurrentVersion,    out System.string HotFixes ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetBuildNumbers2(  &   [Out] System.String^ BaseVersion, &   [Out] System.String^ CurrentVersion, &   [Out] System.String^ HotFixes ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BaseVersion*
:   SOLIDWORKS major revision number

*CurrentVersion*
:   SOLIDWORKS build number

*HotFixes*
:   SOLIDWORKS hot fix numbers

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetBuildNumbers2.

# ![](dotnetimages/collapse.gif)Example

[Get Build Numbers (VBA)](Get_Build_Numbers_Example_VB.htm)

[Get Build Numbers (VB.NET)](Get_Build_Numbers_Example_VBNET.htm)

[Get Build Numbers (C#)](Get_Build_Numbers_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::VersionHistory Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~VersionHistory.html)

[ISldWorks::IVersionHistory Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IVersionHistory.html)

[ISldWorks::IGetVersionHistoryCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IGetVersionHistoryCount.html)

[ISldWorks::RevisionNumber Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RevisionNumber.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 SP05, Revision Number 19.5
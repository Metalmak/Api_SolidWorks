<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SetProgId.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetProgId Method (IMacroFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html) : SetProgId Method (IMacroFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ProgId*
:   Name of the program ID for the component that implements the COM feature handler

Sets the version-independent program ID that is valid for this COM feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetProgId( _    ByVal ProgId As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMacroFeatureData Dim ProgId As System.String   instance.SetProgId(ProgId) ``` | |

| C# |  |
| --- | --- |
| ``` void SetProgId(     System.string ProgId ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetProgId(  &   System.String^ ProgId ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ProgId*
:   Name of the program ID for the component that implements the COM feature handler

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MacroFeatureData::SetProgId.

# ![](dotnetimages/collapse.gif)Remarks

See Exposed COM DLL or Executable and Macro Features for details about macro features that define their behavior using COM.

# ![](dotnetimages/collapse.gif)See Also

####

[IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html)

[IMacroFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData_members.html)

[IMacroFeatureData::GetProgId Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetProgId.html)

[IMacroFeatureData::IsCOMFeature Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IsCOMFeature.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 SP4, Revision Number 14.4
<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions~SetPreservedRegionSetting.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetPreservedRegionSetting Method (ICWTopologyStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions.html) : SetPreservedRegionSetting Method (ICWTopologyStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NPreservedRegionSetting*
:   Preserved region setting as defined in [swsTopologyPreservedRegionOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyPreservedRegionOption_e.html)

Sets the preserved region setting.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetPreservedRegionSetting( _    ByVal NPreservedRegionSetting As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyStudyOptions Dim NPreservedRegionSetting As System.Integer   instance.SetPreservedRegionSetting(NPreservedRegionSetting) ``` | |

| C# |  |
| --- | --- |
| ``` void SetPreservedRegionSetting(     System.int NPreservedRegionSetting ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetPreservedRegionSetting(  &   System.int NPreservedRegionSetting ) ``` | |

#### Parameters

*NPreservedRegionSetting*
:   Preserved region setting as defined in [swsTopologyPreservedRegionOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyPreservedRegionOption_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyStudyOptions::SetPreservedRegionSetting.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions.html)

[ICWTopologyStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0
<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod~SetFlipOffsetDirAtEnd2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetFlipOffsetDirAtEnd2 Method (ICWLinkageRod) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLinkageRod Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html) : SetFlipOffsetDirAtEnd2 Method (ICWLinkageRod) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NFlipDir*
:   Offset flip direction as defined by [swsFlipOffsetDir\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFlipOffsetDir_e.html)

Sets the flip direction of the offset at End 2 of this linkage rod connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetFlipOffsetDirAtEnd2( _    ByVal NFlipDir As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLinkageRod Dim NFlipDir As System.Integer   instance.SetFlipOffsetDirAtEnd2(NFlipDir) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFlipOffsetDirAtEnd2(     System.int NFlipDir ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFlipOffsetDirAtEnd2(  &   System.int NFlipDir ) ``` | |

#### Parameters

*NFlipDir*
:   Offset flip direction as defined by [swsFlipOffsetDir\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFlipOffsetDir_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLinkageRod::SetFlipOffsetDirAtEnd2.

# ![](dotnetimages/collapse.gif)Remarks

This method is not valid if End 2 is a vertex.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLinkageRod Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod.html)

[ICWLinkageRod Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkageRod_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2022 SP0
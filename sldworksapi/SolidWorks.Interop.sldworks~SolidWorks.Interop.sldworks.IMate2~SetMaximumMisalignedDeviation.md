<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~SetMaximumMisalignedDeviation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetMaximumMisalignedDeviation Method (IMate2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMate2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2.html) : SetMaximumMisalignedDeviation Method (IMate2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MaximumDeviation*
:   Maximum allowed misalignment deviation

Sets the maximum allowed misalignment deviation for this misaligned concentric mate.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetMaximumMisalignedDeviation( _    ByVal MaximumDeviation As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMate2 Dim MaximumDeviation As System.Double   instance.SetMaximumMisalignedDeviation(MaximumDeviation) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMaximumMisalignedDeviation(     System.double MaximumDeviation ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMaximumMisalignedDeviation(  &   System.double MaximumDeviation ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MaximumDeviation*
:   Maximum allowed misalignment deviation

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Mate2::SetMaximumMisalignedDeviation.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [IMate2::GetUseMisalignedDeviationDocumentProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetUseMisalignedDeviationDocumentProperty.html) returns false. Call [IMate2::SetUseMisalignedDeviationDocumentProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~SetUseMisalignedDeviationDocumentProperty.html) to set UseDocumentProperty to false if you want to use this method to set the maximum misaligned deviation for this mate.

If [IMate2::GetCurrentMisalignedDeviation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetCurrentMisalignedDeviation.html) is greater than the value set by this method, then the mate fails to solve.

The current deviation and the maximum deviation are cumulative across both concentric mates in the Hole Set. For example, if [IMate2::GetConcentricAlignmentType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetConcentricAlignmentType.html) is set to swConcentricAlignmentType\_e.swConcentricAlignSymmetric, the deviation from both holes is summed before comparison with the maximum deviation.

# ![](dotnetimages/collapse.gif)See Also

####

[IMate2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2.html)

[IMate2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2_members.html)

[IMate2::GetMaximumMisalignedDeviation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~GetMaximumMisalignedDeviation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0
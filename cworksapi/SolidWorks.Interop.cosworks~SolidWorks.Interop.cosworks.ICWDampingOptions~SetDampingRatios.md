<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~SetDampingRatios.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetDampingRatios Method (ICWDampingOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDampingOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions.html) : SetDampingRatios Method (ICWDampingOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NRows*
:   Number of rows in Values

*Values*
:   Array of modes and damping ratios (see **Remarks**)

Sets the damping ratios.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetDampingRatios( _    ByVal NRows As System.Integer, _    ByVal Values As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDampingOptions Dim NRows As System.Integer Dim Values As System.Object Dim value As System.Integer   value = instance.SetDampingRatios(NRows, Values) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetDampingRatios(     System.int NRows,    System.object Values ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetDampingRatios(  &   System.int NRows, &   System.Object^ Values ) ``` | |

#### Parameters

*NRows*
:   Number of rows in Values

*Values*
:   Array of modes and damping ratios (see **Remarks**)

#### Return Value

Error code as defined in [swsSetDampingRatiosError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSetDampingRatiosError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDampingOptions::SetDampingRatios.

# ![](dotnetimages/collapse.gif)Example

See the [ICWDampingOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method works only if [ICWDampingOptions::DampingType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDampingOptions~DampingType.html) is set to [swsDampingType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDampingType_e.html).swsDampingType\_Modal and [ICWDampingOptions::ComputeFromMaterialDamping](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDampingOptions~ComputeFromMaterialDamping.html) is set to 0 (off).

The Values parameter takes a one-dimensional array of one or more data sets, each containing:

* Index of first mode* Index of last mode* Damping ratio

For more information about modal damping, see the SOLIDWORKS Simulation Help.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDampingOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions.html)

[ICWDampingOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions_members.html)

[ICWDampingOptions::GetDampingRatios Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~GetDampingRatios.html)

[ICWDampingOptions::ClearAllDampingRatios Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDampingOptions~ClearAllDampingRatios.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0
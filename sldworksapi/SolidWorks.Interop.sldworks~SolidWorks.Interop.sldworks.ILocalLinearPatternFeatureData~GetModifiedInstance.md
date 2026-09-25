<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~GetModifiedInstance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetModifiedInstance Method (ILocalLinearPatternFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILocalLinearPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData.html) : GetModifiedInstance Method (ILocalLinearPatternFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Instance*
:   Pattern instance number (see **Remarks**)

*D1Distance*
:   Distance from the pattern seed in Direction 1

*D1NominalVal*
:   Offset from the nominal position of Instance in Direction 1

*D2Distance*
:   Distance from the pattern seed in Direction 2

*D2NominalVal*
:   Offset from the nominal position of Instance in Direction 2

Gets the modified values for the specified pattern instance in this linear component pattern feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetModifiedInstance( _    ByVal Instance As System.Integer, _    ByRef D1Distance As System.Double, _    ByRef D1NominalVal As System.Double, _    ByRef D2Distance As System.Double, _    ByRef D2NominalVal As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILocalLinearPatternFeatureData Dim Instance As System.Integer Dim D1Distance As System.Double Dim D1NominalVal As System.Double Dim D2Distance As System.Double Dim D2NominalVal As System.Double   instance.GetModifiedInstance(Instance, D1Distance, D1NominalVal, D2Distance, D2NominalVal) ``` | |

| C# |  |
| --- | --- |
| ``` void GetModifiedInstance(     System.int Instance,    out System.double D1Distance,    out System.double D1NominalVal,    out System.double D2Distance,    out System.double D2NominalVal ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetModifiedInstance(  &   System.int Instance, &   [Out] System.double D1Distance, &   [Out] System.double D1NominalVal, &   [Out] System.double D2Distance, &   [Out] System.double D2NominalVal ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Instance*
:   Pattern instance number (see **Remarks**)

*D1Distance*
:   Distance from the pattern seed in Direction 1

*D1NominalVal*
:   Offset from the nominal position of Instance in Direction 1

*D2Distance*
:   Distance from the pattern seed in Direction 2

*D2NominalVal*
:   Offset from the nominal position of Instance in Direction 2

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See LocalLinearPatternFeatureData::GetModifiedInstance.

# ![](dotnetimages/collapse.gif)Remarks

To specify Instance, you can use [ILocalLinearPatternFeatureData::GetModifiedInstances](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~GetModifiedInstances.html) to learn which pattern instances are modified.

To calculate Instance:

1. Ensure that [ILocalLinearPatternFeatureData::D2PatternSeedOnly](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~D2PatternSeedOnly.html) is set to false.- Calculate:

      For a bi-directional pattern:

*I* = *n2* \* (*i* - 1) + (*j* - 1)

      For a uni-directional pattern:

*I* = *i* - 1

      where:

* *I* = pattern instance number* *n2* = number of instances in Direction 2* *i* = index for Direction 1* *j* = index for Direction 2

> In the pattern's PropertyManager, find *n2* in the **Direction 2** **> Spacing and Instances > Number of instances** field and find [*i,j*] in the **Modified Instances** section.

# ![](dotnetimages/collapse.gif)See Also

####

[ILocalLinearPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData.html)

[ILocalLinearPatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 FCS, Revision Number 29
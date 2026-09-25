<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalCircularPatternFeatureData~GetModifiedInstance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetModifiedInstance Method (ILocalCircularPatternFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILocalCircularPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalCircularPatternFeatureData.html) : GetModifiedInstance Method (ILocalCircularPatternFeatureData) |

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

*AngleFromSeed*
:   Angle from the pattern seed

*OffsetFromNominal*
:   Degree offset from the nominal position of Instance

Gets the modified values for the specified pattern instance in this circular component pattern feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetModifiedInstance( _    ByVal Instance As System.Integer, _    ByRef AngleFromSeed As System.Double, _    ByRef OffsetFromNominal As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILocalCircularPatternFeatureData Dim Instance As System.Integer Dim AngleFromSeed As System.Double Dim OffsetFromNominal As System.Double   instance.GetModifiedInstance(Instance, AngleFromSeed, OffsetFromNominal) ``` | |

| C# |  |
| --- | --- |
| ``` void GetModifiedInstance(     System.int Instance,    out System.double AngleFromSeed,    out System.double OffsetFromNominal ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetModifiedInstance(  &   System.int Instance, &   [Out] System.double AngleFromSeed, &   [Out] System.double OffsetFromNominal ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Instance*
:   Pattern instance number (see **Remarks**)

*AngleFromSeed*
:   Angle from the pattern seed

*OffsetFromNominal*
:   Degree offset from the nominal position of Instance

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See LocalCircularPatternFeatureData::GetModifiedInstance.

# ![](dotnetimages/collapse.gif)Remarks

To specify Instance, you can use [ILocalCircularPatternFeatureData::GetModifiedInstances](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalCircularPatternFeatureData~GetModifiedInstances.html) to learn which pattern instances are modified.

To calculate Instance:

Calculate:

      For a bi-directional pattern:

*I* = *n2* \* (*i* - 1) + (*j* - 1)

      For a uni-directional pattern:

*I* = *i* - 1

      where:

* *I* = pattern instance number* *n2* = number of instances in Direction 2* *i* = index for Direction 1* *j* = index for Direction 2

> In the pattern's PropertyManager, find *n2* in the **Direction 2** **> Spacing and Instances > Number of instances** field and find [*i,j*] in the **Modified Instances** section.

# ![](dotnetimages/collapse.gif)See Also

####

[ILocalCircularPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalCircularPatternFeatureData.html)

[ILocalCircularPatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalCircularPatternFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 FCS, Revision Number 29
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileCenterMateFeatureData~MateAlignment.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MateAlignment Property (IProfileCenterMateFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IProfileCenterMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileCenterMateFeatureData.html) : MateAlignment Property (IProfileCenterMateFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the alignment of this profile center mate.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property MateAlignment As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IProfileCenterMateFeatureData Dim value As System.Integer   instance.MateAlignment = value   value = instance.MateAlignment ``` | |

| C# |  |
| --- | --- |
| ``` System.int MateAlignment {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int MateAlignment {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Mate alignment as defined in swMateAlign\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ProfileCenterMateFeatureData::MateAlignment.

# ![](dotnetimages/collapse.gif)Example

See the [IProfileCenterMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileCenterMateFeatureData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

If this property is set to swMateAlign\_e:

* swMateAlignALIGNED, then vectors normal to the selected entities point in the same direction.* swMateAlignANTI\_ALIGNED, then vectors normal to the selected entities point in opposite directions.

# ![](dotnetimages/collapse.gif)See Also

####

[IProfileCenterMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileCenterMateFeatureData.html)

[IProfileCenterMateFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IProfileCenterMateFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0
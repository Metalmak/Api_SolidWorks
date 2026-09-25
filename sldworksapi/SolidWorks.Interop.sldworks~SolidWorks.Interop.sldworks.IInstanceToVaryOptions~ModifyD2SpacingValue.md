<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions~ModifyD2SpacingValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ModifyD2SpacingValue Method (IInstanceToVaryOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IInstanceToVaryOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions.html) : ModifyD2SpacingValue Method (IInstanceToVaryOptions) |

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

*Value*
:   Spacing value in Direction 2

Modifies the spacing in Direction 2 of the specified pattern instance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ModifyD2SpacingValue( _    ByVal Instance As System.Integer, _    ByVal Value As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IInstanceToVaryOptions Dim Instance As System.Integer Dim Value As System.Double Dim value As System.Boolean   value = instance.ModifyD2SpacingValue(Instance, Value) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ModifyD2SpacingValue(     System.int Instance,    System.double Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ModifyD2SpacingValue(  &   System.int Instance, &   System.double Value ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Instance*
:   Pattern instance number (see **Remarks**)

*Value*
:   Spacing value in Direction 2

#### Return Value

True if the spacing is modified successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See InstanceToVaryOptions::ModifyD2SpacingValue.

# ![](dotnetimages/collapse.gif)Example

See the [IInstanceToVaryOptions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

To calculate Instance:

1. Ensure that the D2PatternSeedOnly property in the pattern feature data object is set to false.- Calculate:

      For a bi-directional pattern:

*I* = *n2* \* (*i* - 1) + (*j* - 1)

      For a uni-directional pattern:

*I* = *i* - 1

      where:

* *I* = pattern instance number* *n2* = number of instances in Direction 2* *i* = index for Direction 1* *j* = index for Direction 2

> In the pattern's PropertyManager, find *n2* in the **Direction 2** **> Spacing and Instances > Number of instances** field and find [*i,j*] in the **Modified Instances** section.

# ![](dotnetimages/collapse.gif)See Also

####

[IInstanceToVaryOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions.html)

[IInstanceToVaryOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 FCS, Revision Number 29
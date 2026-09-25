<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions~SetD2IncrementDimensions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetD2IncrementDimensions Method (IInstanceToVaryOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IInstanceToVaryOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions.html) : SetD2IncrementDimensions Method (IInstanceToVaryOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IncrementDimensions*
:   Array of dimensions to increment

*IncrementDimValues*
:   Array of dimension increments in Direction 2

Sets the dimensions to increment in Direction 2.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetD2IncrementDimensions( _    ByVal IncrementDimensions As System.Object, _    ByVal IncrementDimValues As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IInstanceToVaryOptions Dim IncrementDimensions As System.Object Dim IncrementDimValues As System.Object Dim value As System.Boolean   value = instance.SetD2IncrementDimensions(IncrementDimensions, IncrementDimValues) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetD2IncrementDimensions(     System.object IncrementDimensions,    System.object IncrementDimValues ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetD2IncrementDimensions(  &   System.Object^ IncrementDimensions, &   System.Object^ IncrementDimValues ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IncrementDimensions*
:   Array of dimensions to increment

*IncrementDimValues*
:   Array of dimension increments in Direction 2

#### Return Value

True if the dimensions are incremented successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See InstanceToVaryOptions::SetD2IncrementDimensions.

# ![](dotnetimages/collapse.gif)See Also

####

[IInstanceToVaryOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions.html)

[IInstanceToVaryOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 FCS, Revision Number 29
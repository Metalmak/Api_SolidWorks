<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions~GetModifiedInstances.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetModifiedInstances Method (IInstanceToVaryOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IInstanceToVaryOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions.html) : GetModifiedInstances Method (IInstanceToVaryOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModificationType*
:   Modification type as defined by swInstanceToVaryModificationType\_e

Gets instance numbers of modified pattern instances of the specified type.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetModifiedInstances( _    ByVal ModificationType As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IInstanceToVaryOptions Dim ModificationType As System.Integer Dim value As System.Object   value = instance.GetModifiedInstances(ModificationType) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetModifiedInstances(     System.int ModificationType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetModifiedInstances(  &   System.int ModificationType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModificationType*
:   Modification type as defined by swInstanceToVaryModificationType\_e

#### Return Value

Array of pattern instance numbers

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See InstanceToVaryOptions::GetModifiedInstances.

# ![](dotnetimages/collapse.gif)See Also

####

[IInstanceToVaryOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions.html)

[IInstanceToVaryOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions_members.html)

[IInstanceToVaryOptions::GetModifiedDimensions Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions~GetModifiedDimensions.html)

[IInstanceToVaryOptions::GetD1ModifiedSpacingValue Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions~GetD1ModifiedSpacingValue.html)

[IInstanceToVaryOptions::GetD2ModifiedSpacingValue Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInstanceToVaryOptions~GetD2ModifiedSpacingValue.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 FCS, Revision Number 29
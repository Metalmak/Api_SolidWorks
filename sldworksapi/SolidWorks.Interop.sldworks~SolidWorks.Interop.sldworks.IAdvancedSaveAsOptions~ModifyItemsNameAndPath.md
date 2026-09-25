<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions~ModifyItemsNameAndPath.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ModifyItemsNameAndPath Method (IAdvancedSaveAsOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAdvancedSaveAsOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions.html) : ModifyItemsNameAndPath Method (IAdvancedSaveAsOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IdsList*
:   Array of reference component IDs (see **Remarks**)

*NamesList*
:   Array of new reference component names

*PathsList*
:   Array of new reference component paths

Modifies the specified reference components with the specified names and paths.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ModifyItemsNameAndPath( _    ByVal IdsList As System.Object, _    ByVal NamesList As System.Object, _    ByVal PathsList As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedSaveAsOptions Dim IdsList As System.Object Dim NamesList As System.Object Dim PathsList As System.Object Dim value As System.Integer   value = instance.ModifyItemsNameAndPath(IdsList, NamesList, PathsList) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ModifyItemsNameAndPath(     System.object IdsList,    System.object NamesList,    System.object PathsList ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ModifyItemsNameAndPath(  &   System.Object^ IdsList, &   System.Object^ NamesList, &   System.Object^ PathsList ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IdsList*
:   Array of reference component IDs (see **Remarks**)

*NamesList*
:   Array of new reference component names

*PathsList*
:   Array of new reference component paths

#### Return Value

Return code as defined in swSaveItemsPathError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedSaveAsOptions::ModifyItemsNameAndPath.

# ![](dotnetimages/collapse.gif)Example

See the [IAdvancedSaveAsOptions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions.html) example.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method call:

1. [IAdvancedSaveAsOptions::SetPrefixSuffixToAll](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions~SetPrefixSuffixToAll.html)- [IAdvancedSaveAsOptions::GetItemsNameAndPath](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions~GetItemsNameAndPath.html) to populate IDsList.

IdsList, NamesList, and PathsList are the same array size and map one to one. Use Nothing or null to specify no change to an individual reference in each array.

If you use this method to change the name or path of the top-level document, then it overrides the name or path passed in the Name parameter of [IModelDocExtension::SaveAs3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SaveAs3.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedSaveAsOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions.html)

[IAdvancedSaveAsOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 SP02, Revision Number 28.2
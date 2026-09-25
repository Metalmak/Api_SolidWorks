<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions~GetItemsNameAndPath.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetItemsNameAndPath Method (IAdvancedSaveAsOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAdvancedSaveAsOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions.html) : GetItemsNameAndPath Method (IAdvancedSaveAsOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IdsList*
:   Array of component reference IDs

*NamesList*
:   Array of component reference names

*PathsList*
:   Array of component reference paths

Gets all reference components' names and paths.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetItemsNameAndPath( _    ByRef IdsList As System.Object, _    ByRef NamesList As System.Object, _    ByRef PathsList As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedSaveAsOptions Dim IdsList As System.Object Dim NamesList As System.Object Dim PathsList As System.Object   instance.GetItemsNameAndPath(IdsList, NamesList, PathsList) ``` | |

| C# |  |
| --- | --- |
| ``` void GetItemsNameAndPath(     out System.object IdsList,    out System.object NamesList,    out System.object PathsList ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetItemsNameAndPath(  &   [Out] System.Object^ IdsList, &   [Out] System.Object^ NamesList, &   [Out] System.Object^ PathsList ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IdsList*
:   Array of component reference IDs

*NamesList*
:   Array of component reference names

*PathsList*
:   Array of component reference paths

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedSaveAsOptions::GetItemsNameAndPath.

# ![](dotnetimages/collapse.gif)Example

See the [IAdvancedSaveAsOptions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions.html) example.

# ![](dotnetimages/collapse.gif)Remarks

IdsList, NamesList, and PathsList are the same array size and map one to one. Call this method to obtain the current list of component references before calling [IAdvancedSaveAsOptions::ModifyItemsNameAndPath](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions~ModifyItemsNameAndPath.html) to modify them.

This method lists component references according to the Options parameter that was specified in the call to [IModelDocExtension::GetAdvancedSaveAsOptions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetAdvancedSaveAsOptions.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedSaveAsOptions Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions.html)

[IAdvancedSaveAsOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 SP02, Revision Number 28.2
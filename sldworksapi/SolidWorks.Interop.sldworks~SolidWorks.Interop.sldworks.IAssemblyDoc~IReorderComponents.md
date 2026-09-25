<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~IReorderComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IReorderComponents Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : IReorderComponents Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Number of items in the Source array

*Source*
:   Array of the [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) to move

*Target*
:   Target component or folder feature to which to move the components

*Where*
:   Where to move the components as defined in swReorderComponentsWhere\_e

Moves components to a different location in the FeatureManager tree.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IReorderComponents( _    ByVal Count As System.Integer, _    ByRef Source As Component2, _    ByVal Target As System.Object, _    ByVal Where As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim Count As System.Integer Dim Source As Component2 Dim Target As System.Object Dim Where As System.Integer Dim value As System.Boolean   value = instance.IReorderComponents(Count, Source, Target, Where) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IReorderComponents(     System.int Count,    ref Component2 Source,    System.object Target,    System.int Where ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IReorderComponents(  &   System.int Count, &   Component2^% Source, &   System.Object^ Target, &   System.int Where ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Count*
:   Number of items in the Source array

*Source*
:   Array of the [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) to move

*Target*
:   Target component or folder feature to which to move the components

*Where*
:   Where to move the components as defined in swReorderComponentsWhere\_e

#### Return Value

True if the components were moved, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::IReorderComponents.

# ![](dotnetimages/collapse.gif)Remarks

The Source argument contains the components to reorder in the FeatureManager tree.

The order of the items in the array will be the order that the components appear after the reorder occurs. The components can only be moved within the same component of the model; you cannot move a component from a subassembly into the top level assembly.

The Where argument indicates where the Source should be moved relative to the Target as defined by swReorderComponentsWhere\_e. If the target is a feature, but not a folder feature, this method takes no action and returns false. Only folders that occur within the components section of the Assembly FeatureManager tree can be used; a folder that is among the body features will not be accepted. If the Where argument is specified as one of the two folder-related values, but the Target is a component, the method uses swReorderComponents\_After.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::ReorderComponents Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ReorderComponents.html)

[IPartDoc::ReorderFeature Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ReorderFeature.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP2, Revision Number 15.2
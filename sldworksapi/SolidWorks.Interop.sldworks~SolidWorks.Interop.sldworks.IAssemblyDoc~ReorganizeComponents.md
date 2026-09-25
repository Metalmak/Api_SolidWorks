<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ReorganizeComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReorganizeComponents Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : ReorganizeComponents Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Source*
:   Array of selected [components](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) to more; all of the components must be at the same level in one parent assembly

*Target*
:   Where to move the components, which can be a top-level assembly or sub-assembly anywhere at any level of the hierarchy

Reorganizes an assembly's structure by moving the selected components to the selected assembly or sub-assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReorganizeComponents( _    ByVal Source As System.Object, _    ByVal Target As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim Source As System.Object Dim Target As System.Object Dim value As System.Boolean   value = instance.ReorganizeComponents(Source, Target) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ReorganizeComponents(     System.object Source,    System.object Target ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ReorganizeComponents(  &   System.Object^ Source, &   System.Object^ Target ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Source*
:   Array of selected [components](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) to more; all of the components must be at the same level in one parent assembly

*Target*
:   Where to move the components, which can be a top-level assembly or sub-assembly anywhere at any level of the hierarchy

#### Return Value

True if the selected components were moved to the selected assembly or sub-assembly, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::ReorganizeComponents.

# ![](dotnetimages/collapse.gif)Example

[Reorganize Components (VBA)](Reorganize_Components_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

See SOLIDWORKS Help for more information about reorganizing components and restructuring assemblies.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::IReorganizeComponents Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~IReorganizeComponents.html)

[IAssemblyDoc::ReorderComponents Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ReorderComponents.html)

[DAssemblyDocEvents\_ComponentReorganizeNotifyEventHandler Delegate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_ComponentReorganizeNotifyEventHandler.html)

[IFeatureManager::GroupComponentInstances Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~GroupComponentInstances.html)

[IAssemblyDoc::UngroupComponents Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~UngroupComponents.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0
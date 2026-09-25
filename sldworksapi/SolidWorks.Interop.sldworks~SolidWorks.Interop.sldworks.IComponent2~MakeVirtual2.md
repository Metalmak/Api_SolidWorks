<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~MakeVirtual2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MakeVirtual2 Method (IComponent2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) : MakeVirtual2 Method (IComponent2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AlsoChildVirtual*
:   True to make child components of this component virtual, false to keep the child components linked to external files

Makes this component and optionally its child components virtual by saving them in the current assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function MakeVirtual2( _    ByVal AlsoChildVirtual As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent2 Dim AlsoChildVirtual As System.Boolean Dim value As System.Boolean   value = instance.MakeVirtual2(AlsoChildVirtual) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool MakeVirtual2(     System.bool AlsoChildVirtual ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool MakeVirtual2(  &   System.bool AlsoChildVirtual ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AlsoChildVirtual*
:   True to make child components of this component virtual, false to keep the child components linked to external files

#### Return Value

True if this component and optionally its child components are saved in an assembly, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Component2::MakeVirtual2.

# ![](dotnetimages/collapse.gif)Example

[Add Component and Mate (C#)](Add_Component_and_Mate_Example_CSharp.htm)

[Add Component and Mate (VB.NET)](Add_Component_and_Mate_Example_VBNET.htm)

[Add Component and Mate (VBA)](Add_Component_and_Mate_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method breaks the link to the external component file and optionally the links to any of its child component files. Existing references are ignored, and the component and optionally any of its child components are renamed.

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[IComponent2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html)

[IComponent2::IsVirtual Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsVirtual.html)

[IComponent2::SaveVirtualComponent Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SaveVirtualComponent.html)

[IAssemblyDoc::InsertNewVirtualAssembly Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~InsertNewVirtualAssembly.html)

[IAssemblyDoc::InsertNewVirtualPart Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~InsertNewVirtualPart.html)

[IModelDocExtension::IsVirtualComponent3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IsVirtualComponent3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IsVirtualComponent3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IsVirtualComponent3 Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : IsVirtualComponent3 Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PathChain*
:   Array of fully qualified paths to parent assembly components, up to and including the first non-virtual parent assembly component, if the model is a virtual component

*TitleChain*
:   Array of document titles; each document title corresponds to a fully qualified path in PathChain

Gets the paths to parent assembly components, up to and including the first non-virtual parent, if the model is a virtual component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IsVirtualComponent3( _    ByRef PathChain As System.Object, _    ByRef TitleChain As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim PathChain As System.Object Dim TitleChain As System.Object Dim value As System.Boolean   value = instance.IsVirtualComponent3(PathChain, TitleChain) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsVirtualComponent3(     out System.object PathChain,    out System.object TitleChain ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IsVirtualComponent3(  &   [Out] System.Object^ PathChain, &   [Out] System.Object^ TitleChain ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PathChain*
:   Array of fully qualified paths to parent assembly components, up to and including the first non-virtual parent assembly component, if the model is a virtual component

*TitleChain*
:   Array of document titles; each document title corresponds to a fully qualified path in PathChain

#### Return Value

True if the component is virtual, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::IsVirtualComponent3.

# ![](dotnetimages/collapse.gif)Example

[Get Paths and Titles of Parent of Virtual Component (C#)](Get_Paths_and_Titles_of_Parents_of_Virtual_Component_Example_CSharp.htm)

[Get Paths and Titles of Parent of Virutal Component (VB.NET)](Get_Paths_and_Titles_of_Parents_of_Virtual_Component_Example_VBNET.htm)

[Get Paths and Titles of Parent of Virtual Component (VBA)](Get_Paths_and_Titles_of_Parents_of_Virtual_Component_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IComponent2::IsVirtual Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsVirtual.html)

[IAssemblyDoc::InsertNewVirtualAssembly Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~InsertNewVirtualAssembly.html)

[IComponent2::MakeVirtual Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~MakeVirtual.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 SP4, Revision Number 16.4
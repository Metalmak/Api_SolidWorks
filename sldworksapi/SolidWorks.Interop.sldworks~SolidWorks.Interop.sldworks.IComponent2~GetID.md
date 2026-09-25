<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetID Method (IComponent2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) : GetID Method (IComponent2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the component ID for this component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetID() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent2 Dim value As System.Integer   value = instance.GetID() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetID() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetID(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

ID for this component

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Component2::GetID.

# ![](dotnetimages/collapse.gif)Example

[Get Component State (C#)](Get_Component_State_Example_CSharp.htm)

[Get Component State (VB.NET)](Get_Component_State_Example_VBNET.htm)

[Get Component State (VBA)](Get_Component_State_Example_VB.htm)

[Get Component IDs (C#)](Get_Component_IDs_Example_CSharp.htm)

[Get Component IDs (VB.NET)](Get_Component_IDs_Example_VBNET.htm)

[Get Component IDs (VBA)](Get_Component_IDs_Example_VB.htm)

[Get Top-level Components Using Component IDs (C#)](Get_Top-level_Component_Using_Component_IDs_Example_CSharp.htm)

[Get Top-level Components Using Component IDs (VB.NET)](Get_Top-level_Component_Using_Component_IDs_Example_VBNET.htm)

[Get Top-level Components Using Component IDs (VBA)](Get_Top-level_Component_Using_Component_IDs_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

A component ID:

* is unique within the context of the assembly to which it belongs.
  **NOTE:** A component ID might not be unique across subassemblies within the assembly. For example, a component in subassembly A might have a component ID of 1, and a component in subassembly B might also have a component ID of 1.* is persistent across SOLIDWORKS sessions and never changes, even if you [change the name of the component](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Name2.html).* can be used to identify a specific component in an assembly. Use the component ID returned by this method with [IAssemblyDoc::GetComponentByID](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~GetComponentByID.html) to get a top-level assembly component.* cannot be assigned by applications or users.* is not the same as a persistent reference ID. You can get any component using its persistent reference ID.

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[IComponent2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAssemblyDoc Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IAssemblyDoc Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to functions that perform assembly operations; for example, adding new components, adding mate conditions, hiding, and exploding components.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IAssemblyDoc ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc ``` | |

| C# |  |
| --- | --- |
| ``` public interface IAssemblyDoc ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IAssemblyDoc ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc.

# ![](dotnetimages/collapse.gif)Example

[Run Interference Detection (C#)](Run_Interference_Detection_Example_CSharp.htm)

[Run Interference Detection (VB.NET)](Run_Interference_Detection_Example_VBNET.htm)

[Run Interference Detection (VBA)](Run_Interference_Detection_Example_VB.htm)

[Insert and Save Virtual Assembly (C#)](Insert_and_Save_Virtual_Assembly_Example_CSharp.htm)

[Insert and Save Virtual Assembly (VB.NET)](Insert_and_Save_Virtual_Assembly_Example_VBNET.htm)

[Insert and Save Virtual Assembly (VBA)](Insert_and_Save_Virtual_Assembly_Example_VB.htm)

[Add Components (C#)](Add_Components_Example_CSharp.htm)

[Add Components (VB.NET)](Add_Components_Example_VBNET.htm)

[Add Components (VBA)](Add_Components_Example_VB.htm)

[Add Component and Mate (C++)](Add_Component_and_Mate_Example_CPlusPlus_COM.htm)

[Add Component and Mate (VBA)](Add_Component_and_Mate_Example_VB.htm)

[Insert MidSurface in Assembly (C#)](Insert_MidSurface_in_Component_Example_CSharp.htm)

[Insert MidSurface in Component (VB.NET)](Insert_MidSurface_in_Component_Example_VBNET.htm)

[Insert MidSurface in Component (VBA)](Insert_MidSurface_in_Component_Example_VB.htm)

[Create Auto Route (VBA)](Create_Auto_Route_Example_VB.htm)

[Create Auto Route (VB.NET)](Create_Auto_Route_Example_VBNET.htm)

[Create Auto Route (C#)](Create_Auto_Route_Example_CSharp.htm)

[Add Component and Mate (VB.NET)](Add_Component_and_Mate_Example_VBNET.htm)

[Add Component and Mate Example (C#)](Add_Component_and_Mate_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The SOLIDWORKS API includes functions that are common to all document types; for example, determining the file name associated with a document is a common operation. To expose common document-level functions, the SOLIDWORKS API uses the [IModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) object.

Events are implemented with delegates in the Microsoft .NET Framework. See the [Overview](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks_namespace.html) topic for a list of delegates for this interface.

# ![](dotnetimages/collapse.gif)Accessors

[ICollisionDetectionManager::GetAssembly](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager~GetAssembly.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[AssemblyDoc](SWObjectModel.pdf#AssemblyDoc)

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)
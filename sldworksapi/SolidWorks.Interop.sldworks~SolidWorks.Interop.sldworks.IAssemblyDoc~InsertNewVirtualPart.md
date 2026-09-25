<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~InsertNewVirtualPart.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertNewVirtualPart Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : InsertNewVirtualPart Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FaceOrPlaneToSelect*
:   Plane or planar face

*InsertedComponent*
:   New part inserted as virtual component

Creates a new part in the context of an assembly and saves the part internally in the assembly file as a virtual component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertNewVirtualPart( _    ByVal FaceOrPlaneToSelect As System.Object, _    ByRef InsertedComponent As Component2 _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim FaceOrPlaneToSelect As System.Object Dim InsertedComponent As Component2 Dim value As System.Integer   value = instance.InsertNewVirtualPart(FaceOrPlaneToSelect, InsertedComponent) ``` | |

| C# |  |
| --- | --- |
| ``` System.int InsertNewVirtualPart(     System.object FaceOrPlaneToSelect,    out Component2 InsertedComponent ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int InsertNewVirtualPart(  &   System.Object^ FaceOrPlaneToSelect, &   [Out] Component2^ InsertedComponent ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FaceOrPlaneToSelect*
:   Plane or planar face

*InsertedComponent*
:   New part inserted as virtual component

#### Return Value

Error as defined by swInsertNewPartErrorCode\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::InsertNewVirtualPart.

# ![](dotnetimages/collapse.gif)Example

[Insert New Virtual Component (VB.NET)](Insert_New_Virtual_Component_Example_VBNET.htm)

[Insert New Virtual Component (VBA)](Insert_New_Virtual_Component_Example_VB.htm)

[Insert New Virtual Component (C#)](Insert_New_Virtual_Component_Example_CSharp.htm)

[Insert New Instance of Virtual Component (VBA)](Insert_New_Instance_of_Virtual_Component_Example_VB.htm)

[Insert New Instance of Virtual Component (VB.NET)](Insert_New_Instance_of_Virtual_Component_Example_VBNET.htm)

[Insert New Instance of Virtual Component (C#)](Insert_New_Instance_of_Virtual_Component_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IComponent2::IsVirtual Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IsVirtual.html)

[IModelDocExtension::IsVirtualComponent3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IsVirtualComponent3.html)

[IAssemblyDoc::InsertNewVirtualAssembly Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~InsertNewVirtualAssembly.html)

[IAssemblyDoc::InsertNewAssembly Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~InsertNewAssembly.html)

[IComponent2::MakeVirtual Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~MakeVirtual.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0
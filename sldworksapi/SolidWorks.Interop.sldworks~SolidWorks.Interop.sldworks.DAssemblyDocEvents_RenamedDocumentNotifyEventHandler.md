<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_RenamedDocumentNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_RenamedDocumentNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_RenamedDocumentNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RenamedDocumentInterface*
:   [RenamedDocumentReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenamedDocumentReferences.html) object

Fired when saving an assembly document in which a renamed component file is referenced by other assembly documents.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_RenamedDocumentNotifyEventHandler( _    ByRef RenamedDocumentInterface As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_RenamedDocumentNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_RenamedDocumentNotifyEventHandler(     ref System.object RenamedDocumentInterface ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_RenamedDocumentNotifyEventHandler(  &   System.Object^% RenamedDocumentInterface ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RenamedDocumentInterface*
:   [RenamedDocumentReferences](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenamedDocumentReferences.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RenamedDocumentNotify Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Example

[Rename Component and Update References (C#)](Rename_Component_and_Update_References_Example_CSharp.htm)

[Rename Component and Update References (VB.NET)](Rename_Component_and_Update_References_Example_VBNET.htm)

[Rename Component and Update References (VBA)](Rename_Component_and_Update_References_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swAssemblyRenamedDocumentNotify to register for this notification.

| To... | Use... |
| --- | --- |
| Rename a component file | [IModelDocExtension::RenameDocument](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~RenameDocument.html) |
| Get whether an assembly document has renamed components | [IModelDocExtension::HasRenamedDocuments](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~HasRenamedDocuments.html) |

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0
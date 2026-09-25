<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~CreateNewBody.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateNewBody Method (IPartDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : CreateNewBody Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Creates a new body to use for import sewing operations and returns it to the caller.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateNewBody() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim value As System.Object   value = instance.CreateNewBody() ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateNewBody() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateNewBody(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

New [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::CreateNewBody.

# ![](dotnetimages/collapse.gif)Example

[Create Body Using Trimmed Surfaces (VBA)](Create_Body_using_Trimmed_Surfaces_Example_VB.htm)

[Create Reference Curve (C#)](Create_Reference_Curve_Example_CSharp.htm)

[Create Reference Curve (VB.NET)](Create_Reference_Curve_Example_VBNET.htm)

[Create Reference Curve (VBA)](Create_Reference_Curve_Example_VB.htm)

[Create Imported Solid Body (C#)](Create_Imported_Solid_Body_Example_CSharp.htm)

[Create Imported Solid Body (VB.NET)](Create_Imported_Solid_Body_Example_VBNET.htm)

[Create Imported Solid Body (VBA)](Create_Imported_Solid_Body_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The intention is that with a handle on such a (initially empty) body, appropriate construction methods (for example, [IBody2::CreateTrimmedSurface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~CreateTrimmedSurface.html)) can be called that eventually amount to a non-trivial object.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[IPartDoc::ICreateNewBody2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ICreateNewBody2.html)
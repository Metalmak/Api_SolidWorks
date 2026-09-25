<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| IPropertyManagerPage2Handler9 Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) : IPropertyManagerPage2Handler9 Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Must be implemented by the add-in application to handle callbacks from IPropertyManagerPage2.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IPropertyManagerPage2Handler9 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler9 ``` | |

| C# |  |
| --- | --- |
| ``` public interface IPropertyManagerPage2Handler9 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IPropertyManagerPage2Handler9 ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler9.

# ![](dotnetimages/collapse.gif)Example

To create a SOLIDWORKS .NET add-in that implements this interface, open in Visual Studio one of these projects:

* Visual Basic - SwVBAddin* Visual C# - SwCSharpAddin

# ![](dotnetimages/collapse.gif)Example

[Create PropertyManager Page (VBA)](Create_PropertyManager_Page_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To use this interface:

* In a SOLIDWORKS VBA macro, you must reference the SOLIDWORKS exposed type libraries for add-in use type library specific to the version of SOLIDWORKS that you are running.* In a SOLIDWORKS VB.NET or C# add-in, you must reference the **SOLIDWORKS.interop.swpublished** assembly and set ComVisibleAttribute to true (see ComVisibleAttribute in VB.NET or C# Macros and Add-ins).

For all unimplemented methods of this object, the add-in application can return E\_NOTIMPL.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler9 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9_members.html)

[SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html)
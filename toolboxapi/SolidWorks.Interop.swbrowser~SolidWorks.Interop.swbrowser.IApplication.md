<!-- source: toolboxapi/SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IApplication.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Toolbox Browser API | Send Feedback |
| IApplication Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IApplication_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swbrowser Namespace](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser_namespace.html) : IApplication Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Provides access to the SOLIDWORKS Toolbox Browser add-in.
**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IApplication ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IApplication ``` | |

| C# |  |
| --- | --- |
| ``` public interface IApplication ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IApplication ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Application.

# ![](dotnetimages/collapse.gif)Example

See [Getting Started](GettingStarted-toolboxapi.html) for more information.

# ![](dotnetimages/collapse.gif)Remarks

This interface is available only if SOLIDWORKS Toolbox Browser add-in is an active SOLIDWORKS add-in.

Events are implemented with delegates in the Microsoft .NET Framework. See the [Overview](SOLIDWORKS.Interop.swbrowser~SOLIDWORKS.Interop.swbrowser_namespace.html) topic for a list of delegates for this interface.

# ![](dotnetimages/collapse.gif)Accessors

Call ISldWorks::GetAddInObject, passing in the GUID of the SOLIDWORKS Toolbox Browser add-in type library (**Registry Editor >** **Computer\HKEY\_CLASSES\_ROOT\TypeLib\{ED783340-D5DB-11d4-BD5A-00C04F019809}**), to get a Dispatch pointer to the IApplication object and connect to the SOLIDWORKS Toolbox Browser.

For example, in COM:

> LPDISPATCH pDisp = NULL;
> HRESULT hres = pSldWorks->GetAddInObject("{ED783340-D5DB-11d4-BD5A-00C04F019809}" , &pDisp);

# ![](dotnetimages/collapse.gif)See Also

####

[IApplication Members](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.IApplication_members.html)

[SolidWorks.Interop.swbrowser Namespace](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser_namespace.html)
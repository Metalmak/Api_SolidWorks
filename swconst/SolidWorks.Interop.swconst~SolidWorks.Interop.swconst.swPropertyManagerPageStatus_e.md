<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swPropertyManagerPageStatus_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swPropertyManagerPageStatus\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swPropertyManagerPageStatus\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

PropertyManager page statuses.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swPropertyManagerPageStatus_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swPropertyManagerPageStatus_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swPropertyManagerPageStatus_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swPropertyManagerPageStatus_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swPropertyManagerPage\_CreationFailure** | -1 |
| **swPropertyManagerPage\_NoDocument** | -2 = A PropertyManager page can only be shown in a SOLIDWORKS document window; you can create and set up the page without a document being active, but there must be a document active when you try to show the page; if there is no active document window, then swPropertyManagerPage\_NoDocument is returned |
| **swPropertyManagerPage\_Okay** | 0 |
| **swPropertyManagerPage\_UnsupportedHandler** | 1 = The PropertyManager page is created and shown; however, a problem exists; for example, you must specify the handler when you create the PropertyManager page; your add-in must implement IPropertyManagerPage2Handler4 so that SOLIDWORKS can call back certain methods when operations, such as clicking a button, occur on the PropertyManager page;if the interface that is passed in does not support PropertyManagerPage2Handler4, then swPropertyManagerPage\_UnsupportedHandler is returned |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)
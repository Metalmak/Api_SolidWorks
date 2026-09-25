<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAddComponentConfigOptions_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swAddComponentConfigOptions\_e Enumeration | |
| [See Also](#seealsobookmark)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swAddComponentConfigOptions\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Options for adding components to an assembly.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swAddComponentConfigOptions_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swAddComponentConfigOptions_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swAddComponentConfigOptions_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swAddComponentConfigOptions_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAddComponentConfigOptions\_CurrentSelectedConfig** | 0 = Add a part or assembly in its last saved configuration.  (See IAssemblyDoc::AddComponent5) |
| **swAddComponentConfigOptions\_NewConfigWithAllReferenceModels** | 1 = Add an assembly with all of its components resolved.  (See IAssemblyDoc::AddComponent5) |
| **swAddComponentConfigOptions\_NewConfigWithAsmStructure** | 2 = Add an assembly with all of its components suppressed.  (See IAssemblyDoc::AddComponent5) |

# ![](dotnetimages/collapse.gif)Example

Add Component and Mate (VBA)

Add Component and Mate (VB.NET)

Add Component and Mate (C#)

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)
<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAnnotationVisibilityState_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swAnnotationVisibilityState\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swAnnotationVisibilityState\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Annotation visibility states.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swAnnotationVisibilityState_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swAnnotationVisibilityState_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swAnnotationVisibilityState_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swAnnotationVisibilityState_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAnnotationHalfHidden** | 2 = Annotation is half-hidden (grayed out) or hidden depending on the interactive user's actions. For example, if the annotation's visibility is set to swAnnotationHalfHidden by IAnnotation::Visible, then that annotation is in a half-hidden state, which is not a permanent state. During a Hide/Show Annotations operation in a drawing, a half-hidden annotation is displayed in gray if the interactive user selects to show all annotations. Any annotation set to swAnnotationHalfHidden is hidden when the interactive user finishes using Hide/Show Annotations. |
| **swAnnotationHidden** | 3 = Annotation is hidden |
| **swAnnotationVisibilityUnknown** | 0 = Annotation visibility is not known |
| **swAnnotationVisible** | 1 = Annotation is visible |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)
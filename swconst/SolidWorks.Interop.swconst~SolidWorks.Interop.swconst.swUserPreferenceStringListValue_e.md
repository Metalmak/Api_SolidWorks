<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swUserPreferenceStringListValue_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swUserPreferenceStringListValue\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swUserPreferenceStringListValue\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

User-preference enumerators for system options and document properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swUserPreferenceStringListValue_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swUserPreferenceStringListValue_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swUserPreferenceStringListValue_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swUserPreferenceStringListValue_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swDxfMappingFiles** | 0 = This setting is persistent across SOLIDWORKS sessions; you can also interactively get or set the custom map file setting by clicking File, Save As, .dxf or .dwg as Save as type, and Options; separate each string in the list by a line feed  (e.g., the vbLf constant in Visual Basic). |
| **swEmodelAttachmentList** | 2 = Sets which configurations for which to generate and attach STEP files |
| **swEmodelSelectionList** | 1 = Sets which configurations or sheets to save when publishing an eDrawings |

# ![](dotnetimages/collapse.gif)Remarks

Use this enumeration with ISldWorks::GetUserPreferenceStringListValue and ISldWorks::SetUserPreferenceStringListValue.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)

[swUserPreferenceDoubleValue\_e Enumeration](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swUserPreferenceDoubleValue_e.html)

[swUserPreferenceIntegerValue\_e Enumeration](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swUserPreferenceIntegerValue_e.html)

[swUserPreferenceStringValue\_e Enumeration](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swUserPreferenceStringValue_e.html)

[swUserPreferenceTextFormat\_e Enumeration](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swUserPreferenceTextFormat_e.html)

[swUserPreferenceToggle\_e Enumeration](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swUserPreferenceToggle_e.html)
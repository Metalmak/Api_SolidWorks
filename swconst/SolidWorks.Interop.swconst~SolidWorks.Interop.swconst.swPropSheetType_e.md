<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swPropSheetType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swPropSheetType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swPropSheetType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Property sheet types.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swPropSheetType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swPropSheetType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swPropSheetType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swPropSheetType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swPropSheetAmbientLight** | 3 = Property sheet ambient light |
| **swPropSheetDirectionalLight** | 4 = Property sheet directional light |
| **swPropSheetLighting** | 1 = Property sheet lighting |
| **swPropSheetNotValid** | 0 = Invalid property sheet |
| **swPropSheetPositionLight** | 5 = Property sheet position light |
| **swPropSheetSpotLight** | 6 = Property sheet spot light |
| **swPropSheetToolsOptions** | 2 = Property sheet tools options |

# ![](dotnetimages/collapse.gif)Remarks

This enumerator specifies possible values for the types of ISWPropertySheets exported by the SOLIDWORKS software when a SldWorks notification of type [swAppPropertySheetCreateNotify](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAppNotify_e.html) is sent.

An example of a property sheet is the dialog that is displayed when you click Tools, Options. This dialog consists of a base property sheet and property pages stacked on top of it. To display a specific property page, click its tab.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)
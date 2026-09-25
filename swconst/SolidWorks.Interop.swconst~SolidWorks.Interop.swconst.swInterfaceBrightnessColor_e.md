<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swInterfaceBrightnessColor_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swInterfaceBrightnessColor\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swInterfaceBrightnessColor\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Background colors.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swInterfaceBrightnessColor_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swInterfaceBrightnessColor_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swInterfaceBrightnessColor_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swInterfaceBrightnessColor_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swIBColor\_ActiveTabColor** | 3 = Color of a tab's fill area when the tab is active |
| **swIBColor\_ButtonFillCheckedAndHotColor** | 8 = Color of the CommandManager flat-style button's fill area |
| **swIBColor\_ButtonFillCheckedColor** | 6 = Color of the CommandManager flat-style button's fill area |
| **swIBColor\_ButtonFillHotColor** | 5 = Color of the CommandManager flat-style button's fill area |
| **swIBColor\_ButtonFillPressedColor** | 7 = Color of the CommandManager flat-style button's fill area when pressing and holding down the left button of the mouse |
| **swIBColor\_DisabledTextColor** | 2 = Color of text when text is disabled |
| **swIBColor\_EnabledTextColor** | 1 = Color of text when text is enabled |
| **swIBColor\_FeatureMgrBkgnd** | 0 = Background color is the same as the FeatureManager design tree's background color |
| **swIBColor\_InactiveTabColor** | 4 = Color of a tab's fill area when the tab is inactive |

# ![](dotnetimages/collapse.gif)Remarks

If you want your add-in to use the same colors for your buttons as used by the SOLIDWORKS CommandManager buttons, then you can query and use these values.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)
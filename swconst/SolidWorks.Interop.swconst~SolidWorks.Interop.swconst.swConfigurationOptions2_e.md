<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swConfigurationOptions2_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swConfigurationOptions2\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swConfigurationOptions2\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Option bits used when setting configuration options. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swConfigurationOptions2_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swConfigurationOptions2_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swConfigurationOptions2_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swConfigurationOptions2_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swConfigOption\_DoDisolveInBOM** | 256 or 0x100; True to dissolve the configuration in the BOM and promote all of its child components up one level, false to not |
| **swConfigOption\_DontActivate** | 128 or 0x80; True to not activate the configuration, false to activate the configuration |
| **swConfigOption\_DontShowPartsInBOM** | 2 or 0x2; True to show sub-assemblies in the Bill of Materials, false to list child components in the Bill of Materials |
| **swConfigOption\_HideByDefault** | 8 or 0x8; True to hide newly added components, false to not |
| **swConfigOption\_InheritProperties** | Obsolete |
| **swConfigOption\_LinkToParent** | 64 or 0x40; True to link component to parent configuration, false to not |
| **swConfigOption\_MinFeatureManager** | 16 or 0x10; True to suppress new components, false to not |
| **swConfigOption\_SuppressByDefault** | 4 or 0x4; True to suppress newly added features and mates in this configuration, false to not |
| **swConfigOption\_UseAlternateName** | 1 or 0x1; True to use an alternate configuration name, false to not |
| **swConfigOption\_UseDescriptionInBOM** | 512 or 0x200; True to use the description in the BOM, false to not |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)
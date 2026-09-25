<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.sw3DInterconnectImportErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| sw3DInterconnectImportErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : sw3DInterconnectImportErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

3D Interconnect import errors.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum sw3DInterconnectImportErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As sw3DInterconnectImportErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum sw3DInterconnectImportErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class sw3DInterconnectImportErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **sw3DInterconnectImportErrors\_AssemblyNotSaved** | 3 |
| **sw3DInterconnectImportErrors\_BreakLinkUnavailable** | 4 = Break link is not available for the selected 3D Interconnect feature; break link is only available for top-level assemblies |
| **sw3DInterconnectImportErrors\_Disabled** | 1 = 3D Interconnect is not enabled; to enable set **Tools > Options > System Options > Import > Enable 3D Interconnect** or call calling ISldWorks::SetUserPreferenceToggle([swUserPreferenceToggle\_e](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swUserPreferenceToggle_e.html).swMultiCAD\_Enable3DInterconnect, True) |
| **sw3DInterconnectImportErrors\_IncompatibleType** | 2 = Specified file type is not correct |
| **sw3DInterconnectImportErrors\_None** | 0 |
| **sw3DInterconnectImportErrors\_ParametersUnavailable** | 5 = Only top-level 3D Interconnect features can be edited |
| **sw3DInterconnectImportErrors\_TransferOptionNeeded** | 6 = One or more import options need to be specified for this import |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)
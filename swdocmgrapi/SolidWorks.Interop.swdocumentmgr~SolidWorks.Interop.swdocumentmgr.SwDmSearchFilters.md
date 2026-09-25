<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.SwDmSearchFilters.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| SwDmSearchFilters Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) : SwDmSearchFilters Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Search filters. Bitmask.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum SwDmSearchFilters     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As SwDmSearchFilters ``` | |

| C# |  |
| --- | --- |
| ``` public enum SwDmSearchFilters : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class SwDmSearchFilters : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **SwDmSearchExternalReference** | 16 = Search for simple assembly references to parts and subassemblies |
| **SwDmSearchForAssembly** | 8 = Search for assemblies |
| **SwDmSearchForDrawing** | 4 = Search for drawings |
| **SwDmSearchForPart** | 2 = Search for parts |
| **SwDmSearchInContextReference** | 32 = Search for base parts for derived parts, mirrored parts, derived component parts, and in-context assembly references |
| **SwDmSearchRootAssemblyFolder** | 64 = Search all the way to the assembly's root folder |
| **SwDmSearchSubfolders** | 1 = Recursively search all of the subfolders. This is only applicable when used with [ISwDMDocument::WhereUsed](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDocument~WhereUsed.html) and [ISwDMComponent4::GetDocument2](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMComponent4~GetDocument2.html) |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html)
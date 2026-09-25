<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsSaveeDrawingsErrorCode_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsSaveeDrawingsErrorCode\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsSaveeDrawingsErrorCode\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Result plots error codes when saving results as eDrawings files

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsSaveeDrawingsErrorCode_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsSaveeDrawingsErrorCode_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsSaveeDrawingsErrorCode_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsSaveeDrawingsErrorCode_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsSaveeDrawings\_CosworksViewNotPresent** | 1 = There is no view present |
| **swsSaveeDrawings\_DatabaseNotFound** | 4 = Database not found |
| **swsSaveeDrawings\_NoError** | 0 = No error |
| **swsSaveeDrawings\_NoPlots** | 9 = There are no plots |
| **swsSaveeDrawings\_NotAvailableForCurrentMesh** | 7 = Cannot save plot as an eDrawings file for current mesh type |
| **swsSaveeDrawings\_PlotNotActive** | 6 = There is no active plot |
| **swsSaveeDrawings\_PlotNotFoundError** | 2 = The specified plot is not present |
| **swsSaveeDrawings\_PlotSaveError** | 10 = An error occurred when saving the plot as an eDrawings file |
| **swsSaveeDrawings\_PostDataFilesNotPresent** | 9 = The post data files are not available |
| **swsSaveeDrawings\_PostFilesNull** | 5 = The objects for the post files are not instantiated |
| **swsSaveeDrawings\_ResultFolderNotFound** | 3 = The results folder is not available |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)
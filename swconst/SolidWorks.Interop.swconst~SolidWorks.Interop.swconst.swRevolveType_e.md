<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swRevolveType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swRevolveType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swRevolveType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Revolve feature types.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swRevolveType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swRevolveType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swRevolveType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swRevolveType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swRevolveTypeMidPlane** | 1 = Mid-plane revolution |
| **swRevolveTypeMidPlane360Degrees** | 4 = Create revolve: mid-plane revolution with a 360-degree angle - or - Edit revolve: mid-plane revolution with a 360-degree angle; if you use IRevolveFeatureData2::SetRevolutionAngle, then the 360-degree angle is overwritten |
| **swRevolveTypeOneDirection** | 0 = One-direction revolution |
| **swRevolveTypeOneDirection360Degrees** | 3 = Create revolve: one direction revolution with a 360-degree angle - or - Edit revolve: one direction revolution with a 360-degree angle; if you use IRevolveFeatureData2::SetRevolutionAngle, then the 360-degree angle is overwritten |
| **swRevolveTypeTwoDirection** | 2 = Two direction revolution |
| **swRevolveTypeTwoDirection360Degrees** | 5 = Create and edit revolves: two direction revolution |

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| To... | Use... |
| Create revolve | IFeatureManager::FeatureRevolve  IFeatureManager::FeatureRevolveCut  IFeatureManager::FeatureRevolveThin  IFeatureManager::FeatureRevolveThinCut |
| Edit revolve | IRevolveFeatureData2::Type |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)
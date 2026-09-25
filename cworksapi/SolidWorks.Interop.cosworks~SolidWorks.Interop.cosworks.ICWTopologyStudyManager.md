<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWTopologyStudyManager Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWTopologyStudyManager Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows you to manage topology studies.
**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ICWTopologyStudyManager ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyStudyManager ``` | |

| C# |  |
| --- | --- |
| ``` public interface ICWTopologyStudyManager ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ICWTopologyStudyManager ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyStudyManager.

# ![](dotnetimages/collapse.gif)Example

[Create Topology Study (VBA)](Create_Topology_Study_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

A topology study:

* seeks to optimize the material layout of parts by redistributing material, subject to all applied loads, fixtures, and manufacturing constraints.* consists of optimization goals, constraints, preserved regions, and manufacturing controls. A topology constraint defines, for example, how much material to remove (mass constraint) or how far to displace a component (displacement constraint) to satisfy a given topology optimization goal (e.g., minimize maximum displacement).* is available with SOLIDWORKS Simulation Professional and Premium licenses only.

See the **Topology Study** topic in the Simulation user-interface help for more information.

# ![](dotnetimages/collapse.gif)Accessors

[ICWStudy::TopologyStudyManager](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~TopologyStudyManager.html)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyStudyManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager_members.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)
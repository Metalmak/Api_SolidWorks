<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSensorType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swSensorType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swSensorType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Types of sensor.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swSensorType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swSensorType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swSensorType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swSensorType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSensorDimension** | 2 = Measurement (dimension) sensor |
| **swSensorInterfaceDetection** | 3 = Interference detection sensor; Obsolete |
| **swSensorMassProperty** | 1 = Obsolete |
| **swSensorProximity** | 5 = Obsolete |
| **swSensorSimulation** | 0 = Obsolete |

# ![](dotnetimages/collapse.gif)Remarks

As of SOLIDWORKS 2009 SP02, only sensors of type swSensorDimension are supported. Non-dimension measurement sensors (=4) and all of the other sensor types are no longer supported.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)
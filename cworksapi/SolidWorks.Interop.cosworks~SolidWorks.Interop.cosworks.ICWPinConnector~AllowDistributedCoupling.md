<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector~AllowDistributedCoupling.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AllowDistributedCoupling Property (ICWPinConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPinConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector.html) : AllowDistributedCoupling Property (ICWPinConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [ICWPinConnector::AllowDistributedCoupling2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector~AllowDistributedCoupling2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property AllowDistributedCoupling As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPinConnector Dim value As System.Integer   value = instance.AllowDistributedCoupling ``` | |

| C# |  |
| --- | --- |
| ``` System.int AllowDistributedCoupling {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int AllowDistributedCoupling {    System.int get(); } ``` | |

#### Property Value

True if distributed coupling is allowed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPinConnector::AllowDistributedCoupling.

# ![](dotnetimages/collapse.gif)Remarks

If this property is true, you can set [ICWPinConnector::ConnectionType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector~ConnectionType.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPinConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector.html)

[ICWPinConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2020 SP0
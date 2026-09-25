<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkConnector~LinkConnectorBeginEdit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| LinkConnectorBeginEdit Method (ICWLinkConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLinkConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkConnector.html) : LinkConnectorBeginEdit Method (ICWLinkConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Starts editing a link connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub LinkConnectorBeginEdit() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLinkConnector   instance.LinkConnectorBeginEdit() ``` | |

| C# |  |
| --- | --- |
| ``` void LinkConnectorBeginEdit() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void LinkConnectorBeginEdit(); ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLinkConnector::LinkConnectorBeginEdit.

# ![](dotnetimages/collapse.gif)Remarks

To start editing a link connector, you must call this method. You must call [ICWLinkConnector::LinkConnectorEndEdit](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWLinkConnector~LinkConnectorEndEdit.html) to end editing a link connector. Changes are not applied unless you call both methods.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLinkConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkConnector.html)

[ICWLinkConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkConnector_members.html)
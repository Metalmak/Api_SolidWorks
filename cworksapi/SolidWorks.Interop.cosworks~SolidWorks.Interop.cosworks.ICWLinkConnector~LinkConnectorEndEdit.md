<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkConnector~LinkConnectorEndEdit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| LinkConnectorEndEdit Method (ICWLinkConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLinkConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkConnector.html) : LinkConnectorEndEdit Method (ICWLinkConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Ends editing a link connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function LinkConnectorEndEdit() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLinkConnector Dim value As System.Integer   value = instance.LinkConnectorEndEdit() ``` | |

| C# |  |
| --- | --- |
| ``` System.int LinkConnectorEndEdit() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int LinkConnectorEndEdit(); ``` | |

#### Return Value

Error as defined in [swsLinkConnectorEndEditError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinkConnectorEndEditError_e.html)

# ![](dotnetimages/collapse.gif)Remarks

You must call [ICWLinkConnector::LinkConnectorBeginEdit](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWLinkConnector~LinkConnectorBeginEdit.html) to start editing a link connector. To end editing a link connector, you must call ICWLinkConnector::LinkConnectorEndEdit. Changes are not applied unless you call both methods.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLinkConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkConnector.html)

[ICWLinkConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkConnector_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0
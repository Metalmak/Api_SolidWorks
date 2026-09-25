<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWElasticConnector~ElasticConnectorEndEdit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ElasticConnectorEndEdit Method (ICWElasticConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWElasticConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWElasticConnector.html) : ElasticConnectorEndEdit Method (ICWElasticConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Ends editing an elastic support fixture.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ElasticConnectorEndEdit() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWElasticConnector Dim value As System.Integer   value = instance.ElasticConnectorEndEdit() ``` | |

| C# |  |
| --- | --- |
| ``` System.int ElasticConnectorEndEdit() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ElasticConnectorEndEdit(); ``` | |

#### Return Value

Error as defined in [swsElasticConnectorEndEditError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsElasticConnectorEndEditError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWElasticConnector::ElasticConnectorEndEdit.

# ![](dotnetimages/collapse.gif)Example

See the [ICWElasticConnector](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWElasticConnector.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

You must call [ICWElasticConnector::ElasticConnectorBeginEdit](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWElasticConnector~ElasticConnectorBeginEdit.html) to start editing an elastic support fixture. To end editing this fixture, you must call ICWElasticConnector::ElasticConnectorEndEdit. Changes are not applied unless you call both methods.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWElasticConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWElasticConnector.html)

[ICWElasticConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWElasticConnector_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0
<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinBroker~GetSelectedObjectsBBox.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| GetSelectedObjectsBBox Method (ISwAddinBroker) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwAddinBroker Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinBroker.html) : GetSelectedObjectsBBox Method (ISwAddinBroker) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pDoc*
:   SOLIDWORKS document

*Option*
:   Option as defined in swAddinBrokerBBoxOption\_e

*BoxCorners*
:   Array of six doubles of the points of the bounding box

Gets the selected entities bounding box from an add-in.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetSelectedObjectsBBox( _    ByVal pDoc As System.Object, _    ByVal Option As System.Integer, _    ByRef BoxCorners As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwAddinBroker Dim pDoc As System.Object Dim Option As System.Integer Dim BoxCorners As System.Object   instance.GetSelectedObjectsBBox(pDoc, Option, BoxCorners) ``` | |

| C# |  |
| --- | --- |
| ``` void GetSelectedObjectsBBox(     System.object pDoc,    System.int Option,    out System.object BoxCorners ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetSelectedObjectsBBox(  &   System.Object^ pDoc, &   System.int Option, &   [Out] System.Object^ BoxCorners ) ``` | |

#### Parameters

*pDoc*
:   SOLIDWORKS document

*Option*
:   Option as defined in swAddinBrokerBBoxOption\_e

*BoxCorners*
:   Array of six doubles of the points of the bounding box

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwAddinBroker::GetSelectedObjectsBBox.

# ![](dotnetimages/collapse.gif)Remarks

The order of the points follows the same convention as all SOLIDWORKS bounding boxes.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwAddinBroker Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinBroker.html)

[ISwAddinBroker Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinBroker_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0
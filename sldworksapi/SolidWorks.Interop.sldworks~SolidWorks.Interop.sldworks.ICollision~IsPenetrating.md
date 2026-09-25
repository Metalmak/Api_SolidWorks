<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollision~IsPenetrating.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IsPenetrating Method (ICollision) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICollision Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollision.html) : IsPenetrating Method (ICollision) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether the components involved in this collision penetrate one another.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IsPenetrating() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICollision Dim value As System.Boolean   value = instance.IsPenetrating() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsPenetrating() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IsPenetrating(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

True if components penetrate one another, false if they are only in contact

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Collision::IsPenetrating.

# ![](dotnetimages/collapse.gif)Example

See the [ICollisionDetectionManager](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollisionDetectionManager.html) example.

# ![](dotnetimages/collapse.gif)See Also

####

[ICollision Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollision.html)

[ICollision Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollision_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0
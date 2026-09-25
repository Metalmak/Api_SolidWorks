<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollision~GetComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetComponents Method (ICollision) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICollision Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollision.html) : GetComponents Method (ICollision) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the components involved in this collision.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetComponents() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICollision Dim value As System.Object   value = instance.GetComponents() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetComponents() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetComponents(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of [IComponent2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Collision::GetComponents.

# ![](dotnetimages/collapse.gif)See Also

####

[ICollision Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollision.html)

[ICollision Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICollision_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0
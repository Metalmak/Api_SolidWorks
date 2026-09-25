<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwScene~AspectRatio.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AspectRatio Property (ISwScene) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISwScene Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwScene.html) : AspectRatio Property (ISwScene) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the aspect ratio of the scene floor.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property AspectRatio As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwScene Dim value As System.Double   value = instance.AspectRatio ``` | |

| C# |  |
| --- | --- |
| ``` System.double AspectRatio {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double AspectRatio {    System.double get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Aspect ratio

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwScene::AspectRatio.

# ![](dotnetimages/collapse.gif)Remarks

To change the aspect ratio, set [ISwScene::FixedAspectRatio](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwScene~FixedAspectRatio.html) to false and specify:

* [ISwScene::FloorDepth](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwScene~FloorDepth.html)* [ISwScene::FloorWidth](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwScene~FloorWidth.html)

# ![](dotnetimages/collapse.gif)See Also

####

[ISwScene Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwScene.html)

[ISwScene Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwScene_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0
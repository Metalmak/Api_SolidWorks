<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~CreateBlendSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateBlendSurface Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : CreateBlendSurface Method (IBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Surface1*

*Range1*

*Surface2*

*Range2*

*StartVec*

*EndVec*

*HaveHelpVec*

*HelpVec*

*HaveHelpBox*

*HelpBox*

Obsolete. Superseded by [IBody2::CreateBlendSurface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~CreateBlendSurface.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateBlendSurface( _    ByVal Surface1 As System.Object, _    ByVal Range1 As System.Double, _    ByVal Surface2 As System.Object, _    ByVal Range2 As System.Double, _    ByVal StartVec As System.Object, _    ByVal EndVec As System.Object, _    ByVal HaveHelpVec As System.Integer, _    ByVal HelpVec As System.Object, _    ByVal HaveHelpBox As System.Integer, _    ByVal HelpBox As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim Surface1 As System.Object Dim Range1 As System.Double Dim Surface2 As System.Object Dim Range2 As System.Double Dim StartVec As System.Object Dim EndVec As System.Object Dim HaveHelpVec As System.Integer Dim HelpVec As System.Object Dim HaveHelpBox As System.Integer Dim HelpBox As System.Object Dim value As System.Object   value = instance.CreateBlendSurface(Surface1, Range1, Surface2, Range2, StartVec, EndVec, HaveHelpVec, HelpVec, HaveHelpBox, HelpBox) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateBlendSurface(     System.object Surface1,    System.double Range1,    System.object Surface2,    System.double Range2,    System.object StartVec,    System.object EndVec,    System.int HaveHelpVec,    System.object HelpVec,    System.int HaveHelpBox,    System.object HelpBox ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateBlendSurface(  &   System.Object^ Surface1, &   System.double Range1, &   System.Object^ Surface2, &   System.double Range2, &   System.Object^ StartVec, &   System.Object^ EndVec, &   System.int HaveHelpVec, &   System.Object^ HelpVec, &   System.int HaveHelpBox, &   System.Object^ HelpBox ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Surface1*

*Range1*

*Surface2*

*Range2*

*StartVec*

*EndVec*

*HaveHelpVec*

*HelpVec*

*HaveHelpBox*

*HelpBox*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::CreateBlendSurface.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)
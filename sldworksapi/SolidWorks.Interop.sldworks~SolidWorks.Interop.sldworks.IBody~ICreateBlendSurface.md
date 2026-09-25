<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~ICreateBlendSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateBlendSurface Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : ICreateBlendSurface Method (IBody) |

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

Obsolete. Superseded by [IBody2::ICreateBlendSurface](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ICreateBlendSurface.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateBlendSurface( _    ByVal Surface1 As Surface, _    ByVal Range1 As System.Double, _    ByVal Surface2 As Surface, _    ByVal Range2 As System.Double, _    ByRef StartVec As System.Double, _    ByRef EndVec As System.Double, _    ByVal HaveHelpVec As System.Integer, _    ByRef HelpVec As System.Double, _    ByVal HaveHelpBox As System.Integer, _    ByRef HelpBox As System.Double _ ) As Surface ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim Surface1 As Surface Dim Range1 As System.Double Dim Surface2 As Surface Dim Range2 As System.Double Dim StartVec As System.Double Dim EndVec As System.Double Dim HaveHelpVec As System.Integer Dim HelpVec As System.Double Dim HaveHelpBox As System.Integer Dim HelpBox As System.Double Dim value As Surface   value = instance.ICreateBlendSurface(Surface1, Range1, Surface2, Range2, StartVec, EndVec, HaveHelpVec, HelpVec, HaveHelpBox, HelpBox) ``` | |

| C# |  |
| --- | --- |
| ``` Surface ICreateBlendSurface(     Surface Surface1,    System.double Range1,    Surface Surface2,    System.double Range2,    ref System.double StartVec,    ref System.double EndVec,    System.int HaveHelpVec,    ref System.double HelpVec,    System.int HaveHelpBox,    ref System.double HelpBox ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Surface^ ICreateBlendSurface(  &   Surface^ Surface1, &   System.double Range1, &   Surface^ Surface2, &   System.double Range2, &   System.double% StartVec, &   System.double% EndVec, &   System.int HaveHelpVec, &   System.double% HelpVec, &   System.int HaveHelpBox, &   System.double% HelpBox ) ``` | |

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

See Body::ICreateBlendSurface.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~SketchConvertIsoCurves.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchConvertIsoCurves Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : SketchConvertIsoCurves Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PercentRatio*

*VORuDir*

*DoConstrain*

*SkipHoles*

Obsolete. Superseded by [IModelDoc2::SketchConvertIsoCurves](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~SketchConvertIsoCurves.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SketchConvertIsoCurves( _    ByVal PercentRatio As System.Double, _    ByVal VORuDir As System.Boolean, _    ByVal DoConstrain As System.Boolean, _    ByVal SkipHoles As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim PercentRatio As System.Double Dim VORuDir As System.Boolean Dim DoConstrain As System.Boolean Dim SkipHoles As System.Boolean   instance.SketchConvertIsoCurves(PercentRatio, VORuDir, DoConstrain, SkipHoles) ``` | |

| C# |  |
| --- | --- |
| ``` void SketchConvertIsoCurves(     System.double PercentRatio,    System.bool VORuDir,    System.bool DoConstrain,    System.bool SkipHoles ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SketchConvertIsoCurves(  &   System.double PercentRatio, &   System.bool VORuDir, &   System.bool DoConstrain, &   System.bool SkipHoles ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PercentRatio*

*VORuDir*

*DoConstrain*

*SkipHoles*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::SketchConvertIsoCurves.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)
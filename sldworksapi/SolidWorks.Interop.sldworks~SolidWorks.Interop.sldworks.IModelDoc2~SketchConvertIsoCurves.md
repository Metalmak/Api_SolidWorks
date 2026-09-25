<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchConvertIsoCurves.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchConvertIsoCurves Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SketchConvertIsoCurves Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PercentRatio*
:   Value for percent ratio

*VORuDir*
:   True for V direction, false for UDirection

*DoConstrain*
:   True if you want to constrain these new sketch entities, false if not

*SkipHoles*
:   True if you want to skip the holes in this surface, false if not

Converts ISO-parametric curves on a selected surface into a sketch entity.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SketchConvertIsoCurves( _    ByVal PercentRatio As System.Double, _    ByVal VORuDir As System.Boolean, _    ByVal DoConstrain As System.Boolean, _    ByVal SkipHoles As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim PercentRatio As System.Double Dim VORuDir As System.Boolean Dim DoConstrain As System.Boolean Dim SkipHoles As System.Boolean   instance.SketchConvertIsoCurves(PercentRatio, VORuDir, DoConstrain, SkipHoles) ``` | |

| C# |  |
| --- | --- |
| ``` void SketchConvertIsoCurves(     System.double PercentRatio,    System.bool VORuDir,    System.bool DoConstrain,    System.bool SkipHoles ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SketchConvertIsoCurves(  &   System.double PercentRatio, &   System.bool VORuDir, &   System.bool DoConstrain, &   System.bool SkipHoles ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PercentRatio*
:   Value for percent ratio

*VORuDir*
:   True for V direction, false for UDirection

*DoConstrain*
:   True if you want to constrain these new sketch entities, false if not

*SkipHoles*
:   True if you want to skip the holes in this surface, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SketchConvertIsoCurves.

# ![](dotnetimages/collapse.gif)Example

[Divide Surface into 3D Sketches (VBA)](Divide_Surface_into_3D_Sketches_Example_VB.htm)

[Convert Curves into 3D Sketches (C#)](Convert_Curves_into_3D_Sketches_Example_CSharp.htm)

[Convert Curves into 3D Sketches (VB.NET)](Convert_Curves_into_3D_Sketches_Example_VBNET.htm)

[Convert Curves into 3D Sketches (VBA)](Convert_Curves_into_3D_Sketches_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~CreateEllipticalArc2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateEllipticalArc2 Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : CreateEllipticalArc2 Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CenterX*

*CenterY*

*CenterZ*

*MajorX*

*MajorY*

*MajorZ*

*MinorX*

*MinorY*

*MinorZ*

*StartX*

*StartY*

*StartZ*

*EndX*

*EndY*

*EndZ*

Obsolete. Superseded by [IModelDoc2::CreateEllipticalAr2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~CreateEllipticalArc2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateEllipticalArc2( _    ByVal CenterX As System.Double, _    ByVal CenterY As System.Double, _    ByVal CenterZ As System.Double, _    ByVal MajorX As System.Double, _    ByVal MajorY As System.Double, _    ByVal MajorZ As System.Double, _    ByVal MinorX As System.Double, _    ByVal MinorY As System.Double, _    ByVal MinorZ As System.Double, _    ByVal StartX As System.Double, _    ByVal StartY As System.Double, _    ByVal StartZ As System.Double, _    ByVal EndX As System.Double, _    ByVal EndY As System.Double, _    ByVal EndZ As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim CenterX As System.Double Dim CenterY As System.Double Dim CenterZ As System.Double Dim MajorX As System.Double Dim MajorY As System.Double Dim MajorZ As System.Double Dim MinorX As System.Double Dim MinorY As System.Double Dim MinorZ As System.Double Dim StartX As System.Double Dim StartY As System.Double Dim StartZ As System.Double Dim EndX As System.Double Dim EndY As System.Double Dim EndZ As System.Double Dim value As System.Object   value = instance.CreateEllipticalArc2(CenterX, CenterY, CenterZ, MajorX, MajorY, MajorZ, MinorX, MinorY, MinorZ, StartX, StartY, StartZ, EndX, EndY, EndZ) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateEllipticalArc2(     System.double CenterX,    System.double CenterY,    System.double CenterZ,    System.double MajorX,    System.double MajorY,    System.double MajorZ,    System.double MinorX,    System.double MinorY,    System.double MinorZ,    System.double StartX,    System.double StartY,    System.double StartZ,    System.double EndX,    System.double EndY,    System.double EndZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateEllipticalArc2(  &   System.double CenterX, &   System.double CenterY, &   System.double CenterZ, &   System.double MajorX, &   System.double MajorY, &   System.double MajorZ, &   System.double MinorX, &   System.double MinorY, &   System.double MinorZ, &   System.double StartX, &   System.double StartY, &   System.double StartZ, &   System.double EndX, &   System.double EndY, &   System.double EndZ ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CenterX*

*CenterY*

*CenterZ*

*MajorX*

*MajorY*

*MajorZ*

*MinorX*

*MinorY*

*MinorZ*

*StartX*

*StartY*

*StartZ*

*EndX*

*EndY*

*EndZ*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::CreateEllipticalArc2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~CreateEllipseVB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateEllipseVB Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : CreateEllipseVB Method (IModelDoc2) |

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

Obsolete. Superseded by [IModelDoc2::CreateEllipse2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~CreateEllipse2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateEllipseVB( _    ByVal CenterX As System.Double, _    ByVal CenterY As System.Double, _    ByVal CenterZ As System.Double, _    ByVal MajorX As System.Double, _    ByVal MajorY As System.Double, _    ByVal MajorZ As System.Double, _    ByVal MinorX As System.Double, _    ByVal MinorY As System.Double, _    ByVal MinorZ As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim CenterX As System.Double Dim CenterY As System.Double Dim CenterZ As System.Double Dim MajorX As System.Double Dim MajorY As System.Double Dim MajorZ As System.Double Dim MinorX As System.Double Dim MinorY As System.Double Dim MinorZ As System.Double Dim value As System.Boolean   value = instance.CreateEllipseVB(CenterX, CenterY, CenterZ, MajorX, MajorY, MajorZ, MinorX, MinorY, MinorZ) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateEllipseVB(     System.double CenterX,    System.double CenterY,    System.double CenterZ,    System.double MajorX,    System.double MajorY,    System.double MajorZ,    System.double MinorX,    System.double MinorY,    System.double MinorZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateEllipseVB(  &   System.double CenterX, &   System.double CenterY, &   System.double CenterZ, &   System.double MajorX, &   System.double MajorY, &   System.double MajorZ, &   System.double MinorX, &   System.double MinorY, &   System.double MinorZ ) ``` | |

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

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::CreateEllipseVB.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)
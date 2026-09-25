<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertAnnotationFavorite.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertAnnotationFavorite Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : InsertAnnotationFavorite Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BstrFileName*
:   Path and filename of favorites file

*X*
:   x coordinate where to insert the annotations

*Y*
:   y coordinate where to insert the annotations

*Z*
:   z coordinate where to insert the annotations

Inserts annotations from the specified favorite file at the specified location.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertAnnotationFavorite( _    ByVal BstrFileName As System.String, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double _ ) As Annotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim BstrFileName As System.String Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim value As Annotation   value = instance.InsertAnnotationFavorite(BstrFileName, X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` Annotation InsertAnnotationFavorite(     System.string BstrFileName,    System.double X,    System.double Y,    System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Annotation^ InsertAnnotationFavorite(  &   System.String^ BstrFileName, &   System.double X, &   System.double Y, &   System.double Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BstrFileName*
:   Path and filename of favorites file

*X*
:   x coordinate where to insert the annotations

*Y*
:   y coordinate where to insert the annotations

*Z*
:   z coordinate where to insert the annotations

#### Return Value

[Annotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::InsertAnnotationFavorite.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0
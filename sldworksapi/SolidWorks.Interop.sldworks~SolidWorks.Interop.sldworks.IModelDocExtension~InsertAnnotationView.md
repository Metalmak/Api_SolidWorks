<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertAnnotationView.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertAnnotationView Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : InsertAnnotationView Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AnnotationViewingDirection*
:   Defined by either any swStandardViews\_e enumerator or 0 for selection

*DirectionReference*
:   If 0 specified for AnnotationViewingDirection, then specifiy a [face](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) or [plane](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRefPlane.html) to define the direction of the annotation view

*FlipDirection*
:   True to flip the annotation view in the opposite direction, false to not

*HorizontalDirectionReference*
:   An [edge](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html), [sketch](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch.html), or [face](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

*AngleMadeWithHorizontal*
:   Angle used to make the annotation view horizontal

Inserts an annotation view in this part or assembly document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertAnnotationView( _    ByVal AnnotationViewingDirection As System.Integer, _    ByVal DirectionReference As System.Object, _    ByVal FlipDirection As System.Boolean, _    ByVal HorizontalDirectionReference As System.Object, _    ByVal AngleMadeWithHorizontal As System.Integer _ ) As AnnotationView ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim AnnotationViewingDirection As System.Integer Dim DirectionReference As System.Object Dim FlipDirection As System.Boolean Dim HorizontalDirectionReference As System.Object Dim AngleMadeWithHorizontal As System.Integer Dim value As AnnotationView   value = instance.InsertAnnotationView(AnnotationViewingDirection, DirectionReference, FlipDirection, HorizontalDirectionReference, AngleMadeWithHorizontal) ``` | |

| C# |  |
| --- | --- |
| ``` AnnotationView InsertAnnotationView(     System.int AnnotationViewingDirection,    System.object DirectionReference,    System.bool FlipDirection,    System.object HorizontalDirectionReference,    System.int AngleMadeWithHorizontal ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` AnnotationView^ InsertAnnotationView(  &   System.int AnnotationViewingDirection, &   System.Object^ DirectionReference, &   System.bool FlipDirection, &   System.Object^ HorizontalDirectionReference, &   System.int AngleMadeWithHorizontal ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AnnotationViewingDirection*
:   Defined by either any swStandardViews\_e enumerator or 0 for selection

*DirectionReference*
:   If 0 specified for AnnotationViewingDirection, then specifiy a [face](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) or [plane](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRefPlane.html) to define the direction of the annotation view

*FlipDirection*
:   True to flip the annotation view in the opposite direction, false to not

*HorizontalDirectionReference*
:   An [edge](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html), [sketch](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch.html), or [face](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html)

*AngleMadeWithHorizontal*
:   Angle used to make the annotation view horizontal

#### Return Value

Newly inserted [annotation view](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotationView.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::InsertAnnotationView.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0
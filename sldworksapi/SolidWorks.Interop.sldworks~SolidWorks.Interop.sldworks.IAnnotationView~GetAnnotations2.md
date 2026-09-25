<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~GetAnnotations2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetAnnotations2 Method (IAnnotationView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAnnotationView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView.html) : GetAnnotations2 Method (IAnnotationView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DimXpertOnly*
:   :   True to get only DimXpert annotations, false to get all annotations

*UnassignedInPlane*
:   True to get annotations on all planes, including annotations on unassigned planes; false to get annotations on all planes, except annotations on unassigned planes

Gets the annotations in this annotation view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetAnnotations2( _    ByVal DimXpertOnly As System.Boolean, _    ByVal UnassignedInPlane As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAnnotationView Dim DimXpertOnly As System.Boolean Dim UnassignedInPlane As System.Boolean Dim value As System.Object   value = instance.GetAnnotations2(DimXpertOnly, UnassignedInPlane) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetAnnotations2(     System.bool DimXpertOnly,    System.bool UnassignedInPlane ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetAnnotations2(  &   System.bool DimXpertOnly, &   System.bool UnassignedInPlane ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DimXpertOnly*
:   :   True to get only DimXpert annotations, false to get all annotations

*UnassignedInPlane*
:   True to get annotations on all planes, including annotations on unassigned planes; false to get annotations on all planes, except annotations on unassigned planes

#### Return Value

[Annotations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AnnotationView::GetAnnotations2.

# ![](dotnetimages/collapse.gif)Example

[Move Annotations to Notes Area Annotation View (C#)](Move_Annotations_to_First_Annotation_View_Example_CSharp.htm)

[Move Annotations to Notes Area Annotation View (VB.NET)](Move_Annotations_to_First_Annotation_View_Example_VBNET.htm)

[Move Annotations to Notes Area Annotation View (VBA)](Move_Annotations_to_First_Annotation_View_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IAnnotationView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView.html)

[IAnnotationView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView_members.html)

[IAnnotationView::AnnotationCount Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotationView~AnnotationCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 SP1, Revision number 23.1
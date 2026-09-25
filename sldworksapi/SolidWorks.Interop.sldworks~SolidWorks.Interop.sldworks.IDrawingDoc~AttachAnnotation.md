<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~AttachAnnotation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AttachAnnotation Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : AttachAnnotation Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Option*
:   Annotation attachment option as defined in swAttachAnnotationOption\_e

Attaches an existing annotation to a drawing sheet or view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AttachAnnotation( _    ByVal Option As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Option As System.Integer Dim value As System.Boolean   value = instance.AttachAnnotation(Option) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AttachAnnotation(     System.int Option ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AttachAnnotation(  &   System.int Option ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Option*
:   Annotation attachment option as defined in swAttachAnnotationOption\_e

#### Return Value

True if attachment is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::AttachAnnotation.

# ![](dotnetimages/collapse.gif)Example

[Attach Annotation (VBA)](Attach_Annotation_Example_VB.htm)

[Attach Annotation (VB.NET)](Attach_Annotation_Example_VBNET.htm)

[Attach Annotation (C#)](Attach_Annotation_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To attach an annotation to a drawing view:

1. Multi-select the annotation and drawing view.- Call this method with Option set to swAttachAnnotationOption\_e.swAttachAnnotationOption\_View.

To attach an annotation to a drawing sheet:

1. Select the annotation.- Call this method with Option set to swAttachAnnotationOption\_e.swAttachAnnotationOption\_Sheet.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::InsertModelAnnotations3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertModelAnnotations3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0
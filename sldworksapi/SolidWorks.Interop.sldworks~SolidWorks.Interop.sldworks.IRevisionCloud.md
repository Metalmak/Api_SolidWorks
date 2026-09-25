<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionCloud.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IRevisionCloud Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionCloud_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IRevisionCloud Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a revision cloud annotation.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IRevisionCloud ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRevisionCloud ``` | |

| C# |  |
| --- | --- |
| ``` public interface IRevisionCloud ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IRevisionCloud ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RevisionCloud.

# ![](dotnetimages/collapse.gif)Example

[Insert Revision Cloud into a Drawing (VBA)](Insert_Revision_Cloud_into_Drawing_Example_VB.htm)

[Insert Revision Cloud into a Drawing (VB.NET)](Insert_Revision_Cloud_into_Drawing_Example_VBNET.htm)

[Insert Revision Cloud into a Drawing (C#)](Insert_Revision_Cloud_into_Drawing_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To create a revision cloud in a drawing document, call:

1. [IDrawingDoc::InsertRevisionCloud](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~InsertRevisionCloud.html) or [IDrawingDoc::IInsertRevisionCloud](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~IInsertRevisionCloud.html).- [IRevisionCloud::GetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~GetAnnotation.html) or [IRevisionCloud::IGetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~IGetAnnotation.html) to get the annotation object for the revision cloud.- [IAnnotation::SetPosition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~SetPosition.html) to set the revision cloud position point on the drawing. If you eliminate this step, the revision cloud is rendered starting at the drawing origin of x=0, y=0, z=0. Set the revision cloud position point as follows:

       | For revision cloud shape... | Set the revision cloud position point to... |
       | --- | --- |
       | Ellipse | The center of the revision cloud. |
       | Rectangle | A corner of the revision cloud. |
       | Polygon | One of the points on the revision cloud. |
       | Freehand | One of the points on the revision cloud. |

       - [IRevisionCloud::ArcRadius](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~ArcRadius.html) to set the arc radius of the revision cloud.

         - [IRevisionCloud::SetPathPointAtIndex](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~SetPathPointAtIndex.html) one or more times with Index = -1 to create points on the revision cloud as follows:

           | For revision cloud shape... | Call IRevisionCloud::SetPathPointAtIndex... |
           | --- | --- |
           | Ellipse | Once, specifying the coordinates of a corner of the ellipse-inscribed rectangle. |
           | Rectangle | Once, specifying the coordinates of a corner opposite the revision cloud position point. |
           | Polygon | (Number of polygon sides + 1) times, such that the first and last points coincide with the revision cloud position point. |
           | Freehand | Indefinite number of times, such that the first and last points coincide with the revision cloud position point. |

           - [IRevisionCloud::Finalize](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~Finalize.html) to close the revision cloud path. Once the revision cloud path is closed, you can no longer add points to it.

             - IRevisionCloud::SetPathPointAtIndex to modify the position of an existing point on the revision cloud.

# ![](dotnetimages/collapse.gif)Accessors

[IDrawingDoc::InsertRevisionCloud](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~InsertRevisionCloud.html) and [IDrawingDoc::IInsertRevisionCloud](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~IInsertRevisionCloud.html)

[IRevisionCloud::GetNext](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~GetNext.html) and [IRevisionCloud::IGetNext](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~IGetNext.html)

[IView::GetFirstRevisionCloud](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetFirstRevisionCloud.html) and [IView::IGetFirstRevisionCloud](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetFirstRevisionCloud.html)

[IView::GetRevisionClouds](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetRevisionClouds.html) and [IView::IGetRevisionClouds](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetRevisionClouds.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[RevisionCloud](SWObjectModel.pdf#RevisionCloud)

# ![](dotnetimages/collapse.gif)See Also

####

[IRevisionCloud Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRevisionCloud_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)
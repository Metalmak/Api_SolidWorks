<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~InsertRevisionCloud.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertRevisionCloud Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : InsertRevisionCloud Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CloudShape*
:   Revision cloud annotation shape as defined in swRevisionCloudShape\_e

Inserts a revision cloud annotation with the specified shape into a view or sheet.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertRevisionCloud( _    ByVal CloudShape As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim CloudShape As System.Integer Dim value As System.Object   value = instance.InsertRevisionCloud(CloudShape) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertRevisionCloud(     System.int CloudShape ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertRevisionCloud(  &   System.int CloudShape ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CloudShape*
:   Revision cloud annotation shape as defined in swRevisionCloudShape\_e

#### Return Value

[IRevisionCloud](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::InsertRevisionCloud.

# ![](dotnetimages/collapse.gif)Example

[Insert Revision Cloud into a Drawing (VBA)](Insert_Revision_Cloud_into_Drawing_Example_VB.htm)

[Insert Revision Cloud into a Drawing (VB.NET)](Insert_Revision_Cloud_into_Drawing_Example_VBNET.htm)

[Insert Revision Cloud into a Drawing (C#)](Insert_Revision_Cloud_into_Drawing_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

After calling this method:

1. Call [IRevisionCloud::GetAnnotation](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~GetAnnotation.html) to get the annotation object for the revision cloud.- Call [IAnnotation::SetPosition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~SetPosition.html) to set the revision cloud position point on the drawing. If you eliminate this step, the revision cloud is rendered starting at the drawing origin of x=0, y=0, z=0. Set the revision cloud position point as follows:

     | For revision cloud shape... | Set the revision cloud position point to... |
     | --- | --- |
     | Ellipse | The center of the revision cloud. |
     | Rectangle | A corner of the revision cloud. |
     | Polygon | One of the points on the revision cloud. |
     | Freehand | One of the points on the revision cloud. |

     - Call [IRevisionCloud::ArcRadius](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~ArcRadius.html) to set the arc radius of the revision cloud.

       - Call [IRevisionCloud::SetPathPointAtIndex](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~SetPathPointAtIndex.html) with Index = -1 to create points on the revision cloud as follows:

         | For revision cloud shape... | Call IRevisionCloud::SetPathPointAtIndex... |
         | --- | --- |
         | Ellipse | Once, specifying the coordinates of a corner of the ellipse-inscribed rectangle. |
         | Rectangle | Once, specifying the coordinates of a corner opposite the revision cloud position point. |
         | Polygon | (Number of polygon sides + 1) times, such that the first and last points coincide with the revision cloud position point. |
         | Freehand | Indefinite number of times, such that the first and last points coincide with the revision cloud position point. |

         - Call [IRevisionCloud::Finalize](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRevisionCloud~Finalize.html) to close the revision cloud path. Once the revision cloud path is closed, you can no longer add points to it.

           - Call IRevisionCloud::SetPathPointAtIndex to modify the position of an existing point on the revision cloud.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IDrawingDoc::IInsertRevisionCloud Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~IInsertRevisionCloud.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0
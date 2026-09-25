<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertSplitLineProject.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSplitLineProject Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertSplitLineProject Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IsDirectional*
:   Whether to project in one direction:

    * 0 projects in both directions

      * 1 projects in one direction

*FlipDir*
:   Whether to project along the normal to the sketch plane; valid only when isDirectional = 1:

    * 0 projects in a direction opposite to the normal of the sketch plane

      * 1 projects along the normal of the sketch plane

Splits a face by projecting sketch lines onto the face.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertSplitLineProject( _    ByVal IsDirectional As System.Boolean, _    ByVal FlipDir As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim IsDirectional As System.Boolean Dim FlipDir As System.Boolean   instance.InsertSplitLineProject(IsDirectional, FlipDir) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertSplitLineProject(     System.bool IsDirectional,    System.bool FlipDir ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertSplitLineProject(  &   System.bool IsDirectional, &   System.bool FlipDir ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IsDirectional*
:   Whether to project in one direction:

    * 0 projects in both directions

      * 1 projects in one direction

*FlipDir*
:   Whether to project along the normal to the sketch plane; valid only when isDirectional = 1:

    * 0 projects in a direction opposite to the normal of the sketch plane

      * 1 projects along the normal of the sketch plane

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertSplitLineProject.

# ![](dotnetimages/collapse.gif)Example

[Create Projection Split Line Feature (VBA)](Create_Projection_Split_Line_Example_VB.htm)

[Create Projection Split Line Feature (VB.NET)](Create_Projection_Split_Line_Example_VBNET.htm)

[Create Projection Split Line Feature (C#)](Create_Projection_Split_Line_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

* The sketch to project must be selected using [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) with a mark value of 4.

  * The faces to split must be selected using IModelDocExtension::SelectByID2 with mark values of 1.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::InsertSplitLineSil Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertSplitLineSil.html)

[ISplitLineFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitLineFeatureData.html)

[IFeatureManager::InsertSplitLineIntersect Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSplitLineIntersect.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0
<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetVisibleEntityCount2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetVisibleEntityCount2 Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : GetVisibleEntityCount2 Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*LpViewComponent*
:   [Component](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) from which to get the visible EntityType

*EntityType*
:   Type of entity as defined in swViewEntityType\_e

Gets the number of visible entities of the specified type for the specified component in this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetVisibleEntityCount2( _    ByVal LpViewComponent As Component2, _    ByVal EntityType As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim LpViewComponent As Component2 Dim EntityType As System.Integer Dim value As System.Integer   value = instance.GetVisibleEntityCount2(LpViewComponent, EntityType) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetVisibleEntityCount2(     Component2 LpViewComponent,    System.int EntityType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetVisibleEntityCount2(  &   Component2^ LpViewComponent, &   System.int EntityType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*LpViewComponent*
:   [Component](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) from which to get the visible EntityType

*EntityType*
:   Type of entity as defined in swViewEntityType\_e

#### Return Value

Number of visible entities of EntityType in LpViewComponent

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::GetVisibleEntityCount2.

# ![](dotnetimages/collapse.gif)Example

[Hide and Show All Edges in Drawing View (C#)](Hide_and_Show_All_Ediges_in_Drawing_View_Example_CSharp.htm)

[Hide and Show All Edges in Drawing View (VB.NET)](Hide_and_Show_All_Ediges_in_Drawing_View_Example_VBNET.htm)

[Hide and Show All Edges in Drawing View (VBA)](Hide_and_Show_All_Edges_in_Drawing_View_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Visible entities are entities that are not completely obscured by other entities in the view.

Call this method to get the size of the array returned by [IView::IGetVisibleEntities2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetVisibleEntities2.html).

The difference between this method and the now obsolete IView::GetVisibleEntityCount method is that this method gets the correct number of silhouette edges (EntityType = swViewEntityType\_e.swViewEntityType\_SilhouetteEdge).

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetVisibleEntities2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetVisibleEntities2.html)

[IView::GetVisibleComponentCount Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetVisibleComponentCount.html)

[IView::GetVisibleComponents Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetVisibleComponents.html)

[IView::IGetVisibleComponents Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetVisibleComponents.html)

[IView::GetHiddenComponents Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetHiddenComponents.html)

[IView::EnumHiddenComponents2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~EnumHiddenComponents2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0
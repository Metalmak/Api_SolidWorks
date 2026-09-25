<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDependentViews.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetDependentViews Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : GetDependentViews Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AllViews*
:   True to get all of the dependent views in this view, false to get only the SpecificViewType views in this view

*SpecificViewType*
:   Type of dependent view as defined in swDrawingViewTypes\_e

Gets either all, or only the specified, dependent views in this view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDependentViews( _    ByVal AllViews As System.Boolean, _    ByVal SpecificViewType As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim AllViews As System.Boolean Dim SpecificViewType As System.Integer Dim value As System.Object   value = instance.GetDependentViews(AllViews, SpecificViewType) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetDependentViews(     System.bool AllViews,    System.int SpecificViewType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetDependentViews(  &   System.bool AllViews, &   System.int SpecificViewType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AllViews*
:   True to get all of the dependent views in this view, false to get only the SpecificViewType views in this view

*SpecificViewType*
:   Type of dependent view as defined in swDrawingViewTypes\_e

#### Return Value

Array of dependent [views](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::GetDependentViews.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetDependentViewCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDependentViewCount.html)

[IView::IGetDependentViews Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetDependentViews.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0
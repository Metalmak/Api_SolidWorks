<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDependentViewCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetDependentViewCount Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : GetDependentViewCount Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AllViews*
:   True to get the number of all of the dependent views in this view, false to get the number of SpecificViewType views in this view

*SpecificViewType*
:   Type of dependent view as defined in swDrawingViewTypes\_e

Gets the number of all, or only the specified, dependent views (i.e., alternate position, detail, section, etc.) in this view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDependentViewCount( _    ByVal AllViews As System.Boolean, _    ByVal SpecificViewType As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim AllViews As System.Boolean Dim SpecificViewType As System.Integer Dim value As System.Integer   value = instance.GetDependentViewCount(AllViews, SpecificViewType) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetDependentViewCount(     System.bool AllViews,    System.int SpecificViewType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetDependentViewCount(  &   System.bool AllViews, &   System.int SpecificViewType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AllViews*
:   True to get the number of all of the dependent views in this view, false to get the number of SpecificViewType views in this view

*SpecificViewType*
:   Type of dependent view as defined in swDrawingViewTypes\_e

#### Return Value

Number of dependent views

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::GetDependentViewCount.

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [IView::IGetDependentViews](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetDependentViews.html) to get the size of the array for that method.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetDependentViews Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDependentViews.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0
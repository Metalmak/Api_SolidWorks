<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ShowNamedView2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ShowNamedView2 Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : ShowNamedView2 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VName*
:   Name of the view to display or an empty string to use ViewId instead

*ViewId*
:   ID of the view to display as defined by swStandardViews\_e or -1 to use the VName argument instead; if you specify both VName and ViewId, then ViewId takes precedence if the two arguments do not resolve to the same view

Shows the specified view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowNamedView2( _    ByVal VName As System.String, _    ByVal ViewId As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim VName As System.String Dim ViewId As System.Integer   instance.ShowNamedView2(VName, ViewId) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowNamedView2(     System.string VName,    System.int ViewId ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowNamedView2(  &   System.String^ VName, &   System.int ViewId ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*VName*
:   Name of the view to display or an empty string to use ViewId instead

*ViewId*
:   ID of the view to display as defined by swStandardViews\_e or -1 to use the VName argument instead; if you specify both VName and ViewId, then ViewId takes precedence if the two arguments do not resolve to the same view

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::ShowNamedView2.

# ![](dotnetimages/collapse.gif)Example

[Add Component and Mate (C++)](Add_Component_and_Mate_Example_CPlusPlus_COM.htm)

[Change to Isometric and Zoom to Fit View Mode (VBA)](Change_to_Isometric_and_Zoom_to_Fit_View_Mode_Example_VB.htm)

[Create Revolve Features (VBA)](Create_Revolve_Features_Example_VB.htm)

[Get Sketch Points in Wizard Hole (VBA)](Get_Sketch_Points_in_Wizard_Hole_Example_VB.htm)

[Show Named View (VBA)](Show_Named_View_Example_VB.htm)

[Add Spring to Motion Study (C#)](Add_Spring_to_Motion_Study_Example_CSharp.htm)

[Add Spring to Motion Study (VB.NET)](Add_Spring_to_Motion_Study_Example_VBNET.htm)

[Add Spring to Motion Study (VBA)](Add_Spring_to_Motion_Study_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To set a named view to the active view in a drawing, the drawing view that contains the named view must be selected.

To orient the selected face to its Normal To view, specify **\*Normal To** for VName and **-1** for ViewId.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::NameView Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~NameView.html)

[IModelDoc2::DeleteNamedView Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~DeleteNamedView.html)

[IModelDocExtension::GetNamedViewRotation Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetNamedViewRotation.html)

[IModelDocExtension::IGetNamedViewRotation Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IGetNamedViewRotation.html)

[IModelDocExtension::ResetStandardViews Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ResetStandardViews.html)

[IModelDocExtension::UpdateStandardViews Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~UpdateStandardViews.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0
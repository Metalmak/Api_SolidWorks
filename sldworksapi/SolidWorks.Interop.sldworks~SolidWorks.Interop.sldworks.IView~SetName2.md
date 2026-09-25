<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~SetName2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetName2 Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : SetName2 Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   Name of drawing view

Sets the name of this drawing view, as displayed in the FeatureManager design tree.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetName2( _    ByVal Name As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim Name As System.String Dim value As System.Boolean   value = instance.SetName2(Name) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetName2(     System.string Name ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetName2(  &   System.String^ Name ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Name of drawing view

#### Return Value

True if the name of the drawing view is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::SetName2.

# ![](dotnetimages/collapse.gif)Remarks

The drawing view name that you specify:

* must be unique in the FeatureManager design tree.

  * not contain any of the SOLIDWORKS reserved special characters.

If either of these conditions is not met, then this method returns false and the name of the drawing view is not changed.

You cannot change the drawing view name for detail views and section views. If you attempt to do so, then false if returned and the drawing view name is not changed.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetName2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetName2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0
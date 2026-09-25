<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~TranslateBy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| TranslateBy Method (IModelView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html) : TranslateBy Method (IModelView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   Translation in X direction, in meters and relative to X,Y axes of the graphics area

*Y*
:   Translation in Y direction, in meters and relative to Windows X,Y axes of the graphics area

Translates the model view in the screen.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub TranslateBy( _    ByVal X As System.Double, _    ByVal Y As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelView Dim X As System.Double Dim Y As System.Double   instance.TranslateBy(X, Y) ``` | |

| C# |  |
| --- | --- |
| ``` void TranslateBy(     System.double X,    System.double Y ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void TranslateBy(  &   System.double X, &   System.double Y ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   Translation in X direction, in meters and relative to X,Y axes of the graphics area

*Y*
:   Translation in Y direction, in meters and relative to Windows X,Y axes of the graphics area

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelView::TranslateBy.

# ![](dotnetimages/collapse.gif)Example

[Set Viewports (VB.NET)](Set_Viewports_Example_VBNET.htm)

[Set Viewports (VBA)](Set_Viewports_Example_VB.htm)

[Set Viewports (C#)](Set_Viewports_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method lets you specify a vector by which to translate the current SOLIDWORKS graphics area. This vector is in meters and is relative to the X,Y axes of the graphics area. This vector has no relation to the SOLIDWORKS triad axis that is displayed in the graphics area. This method is equivalent to the user-interface panning of the graphics area.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html)

[IModelView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView_members.html)
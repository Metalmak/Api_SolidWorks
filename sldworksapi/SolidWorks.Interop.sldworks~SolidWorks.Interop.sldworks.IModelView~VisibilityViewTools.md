<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~VisibilityViewTools.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| VisibilityViewTools Property (IModelView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html) : VisibilityViewTools Property (IModelView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the visibility of the Heads-up View Toolbar for this model view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property VisibilityViewTools As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelView Dim value As System.Boolean   instance.VisibilityViewTools = value   value = instance.VisibilityViewTools ``` | |

| C# |  |
| --- | --- |
| ``` System.bool VisibilityViewTools {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool VisibilityViewTools {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True if the Heads-up View toolbar is visible, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelView::VisibilityViewTools.

# ![](dotnetimages/collapse.gif)Example

'-----------------------------------------

'

' Preconditions: Drawing document is open and

'                Heads-up View toolbar is visible.

'

' Postcondition: Heads-up View toolbar is hidden.

'

'------------------------------------------

Option Explicit

Dim swApp As SldWorks.SldWorks

Dim swModel As SldWorks.ModelDoc2

Dim swModelView As SldWorks.ModelView

Dim vRect as Variant

Sub main()

Set swApp = Application.SldWorks

Set swModel = swApp.ActiveDoc

Set swModelView = swModel.ActiveView

' Assume Heads-up View toolbar is visible (True)

Debug.Print "Heads-up View toolbar visible: " & swModelView.VisibilityViewTools

' Hide Heads-up View toolbar (False)

swModelView.VisibilityViewTools = False

Debug.Print "Hands-up View toolbar visible: " & swModelView.VisibilityViewTools

swModelView.GraphicsRedraw(vRect)

End Sub

# ![](dotnetimages/collapse.gif)Remarks

After setting this property to false, call [IModelView::GraphicsRedraw](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView~GraphicsRedraw.html) or [IModelView::IGraphicsRedraw](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView~IGraphicsRedraw.html) to repaint the entire graphics window.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html)

[IModelView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0
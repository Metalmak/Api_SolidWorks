<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~ObjectSizesAway.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ObjectSizesAway Property (IModelView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html) : ObjectSizesAway Property (IModelView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Helps define the perspective of the current model view by relating the size of a displayed object with the distance of the object from the observer.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ObjectSizesAway As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelView Dim value As System.Double   instance.ObjectSizesAway = value   value = instance.ObjectSizesAway ``` | |

| C# |  |
| --- | --- |
| ``` System.double ObjectSizesAway {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double ObjectSizesAway {    System.double get();    void set ( &   System.double value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Distance of the object from the observer, relative to the size of the object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelView::ObjectSizesAway.

# ![](dotnetimages/collapse.gif)Remarks

This property controls the same value as the view, display, perspective information dialog box. It gives the ratio of the distance of the object from the observer to the size of the object. The smaller the value, the greater the amount of perspective distortion.

You can only modify or get this property when the current model view has the perspective display enabled. See [IModelView::AddPerspective](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView~AddPerspective.html) and [IModelView::RemovePerspective](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelView~RemovePerspective.html). If perspective display is disabled, getting the property returns -1, and setting the property has no effect.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html)

[IModelView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView_members.html)

[IModelView::HasPerspective Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~HasPerspective.html)
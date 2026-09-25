<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D~Activate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Activate Method (IView3D) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView3D Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D.html) : Activate Method (IView3D) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SaveLastState*
:   True to back up the previous model state prior to activating this 3D View, false to not back up the previous model state prior to activating this 3D view

Activates this 3D View.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Activate( _    ByVal SaveLastState As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView3D Dim SaveLastState As System.Boolean   instance.Activate(SaveLastState) ``` | |

| C# |  |
| --- | --- |
| ``` void Activate(     System.bool SaveLastState ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Activate(  &   System.bool SaveLastState ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SaveLastState*
:   True to back up the previous model state prior to activating this 3D View, false to not back up the previous model state prior to activating this 3D view

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View3D::Activate.

# ![](dotnetimages/collapse.gif)Example

See the [IView3D](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView3D.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

The model state includes the model's:

* active configuration* display state* explode, section, or Model Break view state* view orientation, including pan and zoom

# ![](dotnetimages/collapse.gif)See Also

####

[IView3D Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D.html)

[IView3D Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D_members.html)

[IView3D::Deactivate Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D~Deactivate.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0
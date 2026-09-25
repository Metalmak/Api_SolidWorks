<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView~ISetStereoSeparation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISetStereoSeparation Method (IModelView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html) : ISetStereoSeparation Method (IModelView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DfSeparation*
:   Array of 2 doubles representing the stereo magnitude and stereo parallax balance settings

Obsolete and not superseded. Functionality no longer implemented.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ISetStereoSeparation( _    ByRef DfSeparation As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelView Dim DfSeparation As System.Double Dim value As System.Boolean   value = instance.ISetStereoSeparation(DfSeparation) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ISetStereoSeparation(     ref System.double DfSeparation ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ISetStereoSeparation(  &   System.double% DfSeparation ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DfSeparation*
:   Array of 2 doubles representing the stereo magnitude and stereo parallax balance settings

#### Return Value

True if changing the stereo-value settings is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelView::ISetStereoSeparation.

# ![](dotnetimages/collapse.gif)Remarks

This method only affects the model view's display if:

* Display window was set up to display stereoscopically

  * Application is currently set to display stereoscopically.

[ISldWorks::EnableStereoDisplay](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~EnableStereoDisplay.html) needs to be called to do these things.

There are two stereoscopic display values this method sets.

1. Settings[0] controls the magnitude of the stereoscopic effect by specifying the stereoscopic, virtual, camera separation. Appropriate values for this setting depend on the scale of the object, the distance from the virtual camera to the object center, the perspective field of view angle, and, perhaps, an adjustment factor that is available to the user.

   - Settings[1] controls the asymmetry of the projection frustums, thus, adjusting the parallax balance of the stereoscopic scene. It is desirable for any stereoscopic scene to comfortably balance the use of negative parallax (elements appearing to float in front of the display surface) and positive parallax (elements appearing to reside somewhere behind the display surface). Appropriate values for this setting should be arrived at experimentally.

If this method is not called, the default settings will equal 0.0, resulting in identical left-eye and right-eye renderings, and no visible stereo effect, even if stereoscopic display is currently enabled.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView.html)

[IModelView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelView_members.html)
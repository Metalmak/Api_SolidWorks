<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~StereoFocalLength.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| StereoFocalLength Property (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : StereoFocalLength Property (IEModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the distance between camera position and the stereo focal plane in terms of the camera eye distance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property StereoFocalLength As System.Single ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim value As System.Single   instance.StereoFocalLength = value   value = instance.StereoFocalLength ``` | |

| C# |  |
| --- | --- |
| ``` System.float StereoFocalLength {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.float StereoFocalLength {    System.float get();    void set ( &   System.float value); } ``` | |

#### Property Value

Distance between camera position and the stereo focal plane in terms of the camera eye distance; default stereo distance = 0

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::StereoFocalLength.

# ![](dotnetimages/collapse.gif)Remarks

A stereo distance of 0 corresponds to the stereo focal plane being set at the camera target.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

[IEModelViewControl::StereoEnabled Property ()](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~StereoEnabled.html)

[IEModelViewControl::StereoSeparation Property ()](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~StereoSeparation.html)

[IEModelViewControl::CameraNearClip Property ()](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~CameraNearClip.html)

[IEModelViewControl::CameraProjection Property ()](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~CameraProjection.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2014 SP1